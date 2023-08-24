#### Valid Palindrome
> Check if given string is an palindrome

Algo:
1. Two pointers **start(0)** and **end(len(arr))**.
2. Come inside one by one checking equality.
3. Until **start == end**

#### Is Subsequence
> Check if a the given **str1** is a subsequence of **str2**.

Algo:
1. Take two pointers **ptr1** and **ptr2** with both starting at **0**
2. Increase **ptr2** if `str1[ptr1] != str2[ptr2]` and increase both if matching.
3. If we reach at the end of str1 means it is subsequence.

#### Two Sum
> Check if any two values from the given array make up the **target** sum.

1. Sort the array.
2. Take **2 pointers** `left` and `right`.
3. If there sum is smaller than the target, increase the `left`
4. If there sum is greater than the target, decrease the `right`.
5. Do this until `left == right`.
6. Return answer if sum becomes equal to **target**.

#### Container with most water
> Given array of heights find the two points where most water area can occur.![[Pasted image 20230824120513.jpg]]

`height = [1,8,6,2,5,4,8,3,7]`

Algo:
1. 2 Pointer **startPtr** and **endPtr**.
2. Loop until `strartPtr < endPtr`
3. Each Iteration calculate total area of water update the max answer.
4. Now if **startPtr** height is smaller increase it by one `startPtr+=1`
5. If **endPtr** is smaller decrease it by one `endPtr-=1`

```python
def maxArea(self, height: List[int]) -> int:
	l = 0
	r = len(height)-1
	max_area = 0
	while l < r:
		max_area = max(max_area, min(height[l], height[r])*(r-l))
		if height[l] > height[r]: r-=1
		elif height[l] < height[r]: l+=1
		else: r, l = r-1, l+1
	return max_area
```

--- 

#### Next Permutation
![[Next Permutation]]

**ALGO**
1. First from then end we will find a pivot 
which is smaller then the next element.
2. So that we can know which element to replace it with.
3. Now find a just bigger element to it from the last of the string.
4. Now replace that just bigger element to our pivot.
5. Because we know from pivot to end our number is sorted in desc.
6. Just reverse it to make ascending

**CODE**:
```python
    def nextPermutation(self, nums: List[int]) -> None:
        """
        Do not return anything, modify nums in-place instead.
        """
        # find a pivot
        n = len(nums)
        pivot = 0
        flag = 0
        for i in range(n-2,-1,-1):
            if nums[i] < nums[i+1]:
                pivot = i
                flag=1
                break

        next_idx = n-1
        for i in range(n-1, -1, -1):
            if nums[i] > nums[pivot]:
                next_idx = i
                break
        
        nums[pivot], nums[next_idx] = nums[next_idx], nums[pivot]
        # Instead of soerting we can just reverse it

        nums[pivot+1:] = sorted(nums[pivot+1:])
      
```