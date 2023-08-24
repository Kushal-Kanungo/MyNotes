#### Best time to buy and sell a stock [Leetcode](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/)
> Need to buy and sell only once

**Input:** `prices = [7,1,5,3,6,4]`
**Output:** `5`

**ALGO:**
1. Keep track of minimum price find upto an point.
2. And try to sell daily and find profit by using min so far `profit = arr[i] - minSoFar`
3. Update the answer

```python
def maxProfit(self, prices: List[int]) -> int:
	# we will keep the track of minimum price we appeared
	minSoFar = float('inf')
	ans = 0
	for val in prices:
		minSoFar = min(minSoFar, val)
		# every time we will check if I sell today what will be the profit.
		# profit will be today's price - minSoFar
		ans = max(ans, val-minSoFar)
	return ans
```

---

#### Activity Selection
**Input:** `activities = [(10,20), (12,25), (20,30)]`
**Output:** 0 2
>`activities[idx][start, end]`

**INTUTION :**
> If I have to select an activity which is overlapping then I will select that activity which has **finishing time smaller**. Because will maximize our answer.

**ALGO :**
1. First we **sort** according to finishing time.
2. Now we keep the track of from which time we can start.
3. Loop over the array and find total activities we can do.

**ALTERNATE :**
Instead of sorting we can use priority queue(min heap). The Top element will we of smallest final time.

```python
def maxActivity(activities):
    activities.sort(key = lambda x: x[1])
    starting = 0
    ans = 0
    for start_time, end_time in activities:
        if starting <= start_time:
            ans+=1
            starting = end_time
    return ans

print(maxActivity([[2,3], [1,4], [5, 8], [6, 10]]))
print(maxActivity([[1,3], [2,4], [3, 8], [10, 11]]))
```