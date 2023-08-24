#### Coin Change

**ALGO**
1. Run a BFS at every point and use all coins to reach next value.
2. After running the loop our answer will be at the end.
---

#### Longest Increasing Subsequence

**ALGO :**
1. Run a loop from back.
2. Run another loop from current to end inside it.
3. Check if we can include current if we can update the the index.

```python
def lengthOfLIS(self, nums: List[int]) -> int:
	lis = [1]*len(nums)
	for i in range(len(nums)-2, -1, -1):
		for j in range(i+1, len(nums)):
			if nums[i] < nums[j]:
				lis[i] = max(lis[i], lis[j]+1)
	return max(lis)
```

---

#### Word Break

**ALGO:**

```python
    def wordBreak(self, s: str, wordDict: List[str]) -> bool:
        data = set(wordDict)
        array = [-1]
        for idx, ch in enumerate(s):
            for j in array:
                if s[j+1: idx+1] in data:
                    array.append(idx)
                    break
        return array[-1] == len(s)-1
```

---

#### House Robber

**Input:** `nums = [1,2,3,1]`
**Output:** `4`
**Explanation:** Rob house 1 (money = 1) and then rob house 3 (money = 3).
Total amount you can rob = 1 + 3 = 4.

**ALGO:**

```python
def dpSolve(arr):
	dp = [0]*(len(arr)+1)
	
	dp[1] = arr[0]
	
	for i in range(2, len(dp)):
		dp[i] = max(dp[i-1], dp[i-2]+arr[i-1])
	return dp[len(arr)]

return dpSolve(nums)
```

--- 

#### Min Jumps To End

**CODE:**

```python
n = len(nums)
	if n < 2: return 0
	dp = [n+1] * n
	dp[0] = 0
	for idx,num in enumerate(nums):
		for i in range(idx+1, min(idx+num+1,n)):
			dp[i] = min(dp[idx]+1, dp[i])
	return dp[-1]
```
