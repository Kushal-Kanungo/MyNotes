#### Minimum Size Subarray Sum [Leetcode](https://leetcode.com/problems/minimum-size-subarray-sum/)
> Given an **array** find the minimum length of subarray whose sum greater than or equal to **target**.

**Input:** `target = 7`, `nums = [2,3,1,2,4,3]`
**Output:** `2`
**Explanation:** The subarray `[4,3]` has the minimal length under the problem constraint.

**ALGO**
1. Take **2 pointers** `l` & `r` both start from **0**.
2. Loop until **h** reach at the end of array.
3. Keep a running sum `currSum` during loop.
4. At every iteration add `arr[h]` to `curr_sum` and increase the **h+=1**.
5. Now until `curr_sum` is greater than increase our **l** one by one decrease the value from `curr_sum` and update the answer.

```python
def minSubArrayLen(self, target: int, nums: List[int]) -> int:
	# both pointers from 0
	l = h = 0
	ans = float('inf')
	# running sum
	curr = 0

	# running until h reaches end
	while l <= h and h < len(nums):
		curr += nums[h] # adding right pointers value to curr.
		h += 1 # increase the right pointer by one.

		# decreasing util curr sum is grater or equal to target.
		while curr >= target  and l <= h:
			ans = min(ans, h-l)
			curr -= nums[l]
			l+=1
	return ans if ans != float('inf') else 0
```

---

#### Longest Substring Without Repeating Characters [Leetcode](https://leetcode.com/problems/longest-substring-without-repeating-characters/)

**Input:** s = "abcabcbb"
**Output:** 3
**Explanation:** The answer is "abc", with the length of 3.

**ALGO**
1. Create a **lookup** table. Where we will keep last encountered position of a char.
2. Start with 2 pointers both at 0
3. Increase right pointer until we find that this **char** has be appeared before by using lookup.
4. Now check if that position lies between our **two pointers**.
5. If not then just update the position in lookup and update the length `r-l+1`.
6. But if it is between than we need to move left pointer one index more the the last appeared position.

```python
def lengthOfLongestSubstring(self, s: str) -> int:  
	lookup = {}
	l, r = 0, 0
	length = 0
	while r < len(s):
		if s[r] in lookup:
			l = max(lookup[s[r]]+1, l)
		lookup[s[r]] = r
		length = max(length, r-l+1)
		r+=1
	return length
```

---

#### Kadane's Algorithm / Max Sum of Subarray
> Used to find maximum sum of **subarray**
>  Applications:
> - Max Sum of subarray

**ALGO:**
1. take current sum as zero(0)
2. and maxsum as -infinity
3. now loop over every element in array
4. add this to currsum
5. now save the value of maximum of currsum and maxsum in maxsum
6. if currsum becomes less than **0** then make currsum=0 because that value should not be in our sub array
```python
def kadane_algo(arr, n):
    currsum = 0
    maxsum = float('-inf')
    for i in range(n):
        currsum = currsum+arr[i]
        maxsum = max(maxsum, currsum)
        # if our currsum become less than zero then we need to start new subarray as this will be always have sum negative to it.
        if currsum < 0:
            currsum = 0
    return maxsum
```

