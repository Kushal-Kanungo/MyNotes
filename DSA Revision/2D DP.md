
#### Unique Paths

**CODE:**
```python
def uniquePaths(self, m: int, n: int) -> int:
	dp = [[0 for _ in range(m)] for _ in range(n)]
	dp[0][0] = 1
	for i in range(n):
		for j in range(m):
			dp[i][j] += dp[i-1][j] if i > 0 else 0
			dp[i][j] += dp[i][j-1] if j > 0 else 0
	return dp[-1][-1]
```

#### Longest Commone Subsequence

![[Longest Common Subsequence]]

---

#### KNAPSACK

```python
def knapsack(capacity, weights, profits, idx=0):
    if idx == len(weights):
        return 0
    elif weights[idx] <= capacity:
        option1 = profits[idx] + \
            knapsack(capacity-weights[idx], weights, profits, idx+1)

        option2 = knapsack(capacity, weights, profits, idx+1)
        return max(option1, option2)
    else:
        return knapsack(capacity, weights, profits, idx+1)

```


**TABULAR :**
```python
def knapsack(weight: list, profit, capacity):
    dp = [[0 for i in range(capacity+1)] for j in range(len(weight)+1)]
    for i in range(len(weight)):
        wi = weight[i]
        pr = profit[i]

        row = i+1
        for col in range(capacity+1):
            if col-wi >= 0:
                dp[row][col] = max(dp[i][col], dp[i][col-wi]+pr)
            else:
                dp[row][col] = dp[i][col]

    return dp[len(weight)][capacity]

```

