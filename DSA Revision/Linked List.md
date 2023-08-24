#### Reversing the linked list

**ALGO:**
> TODO

**CODE:**
```python
def reverseList(self, head: Optional[ListNode]) -> Optional[ListNode]:
	current = head
	prev = None
	
	while current is not None:
		next_node = current.next
		current.next = prev
		prev = current
		current = next_node
	
	head = prev
	return head
```

---

#### Detect Cycle and Find Starting Node

**ALGO:**
1. Run **slow** and **fast** pointers.
2. Slow pointer will run one node at a time.
3. Fast pointer will jump one node in between.
4. If Fast pointer reaches **NONE** than no cycle.
5. If Fast Pointer becomes equal to **slow** pointer then cycle exist.

**Starting Node of loop:**
1. Start a pointer from starting of the linked list.
2. Start a pointer from the merging point of the linked list.
3. A node at which these to meet will be our starting of the loop.

**CODE** :
```python
def hasCycle(self, head: Optional[ListNode]) -> bool:
	slow = head
	fast = head
	while fast and fast.next and fast.next.next:
		fast = fast.next.next
		slow = slow.next   
		if fast == slow:
			return True             
	return False
```
