#### Maximum Depth Of Binary Tree

**ALGO:** Recursively Solve
```python
def maxDepth(self, root: Optional[TreeNode]) -> int:
	if root is None:
		return 0
	return 1+max(self.maxDepth(root.left), self.maxDepth(root.right))
```

---

#### Subtree of Another Tree [Leetcode](https://leetcode.com/problems/subtree-of-another-tree/)

**ALGO:**
1. Recursively check if we can create from root.
2. If not then check in left and write.
3. Create a helper function which check current value of both the root node and recursively go to left and right.
4. If any fails return **False**.

**CODE:**
```python
    def isSubtree(self, root: Optional[TreeNode], subRoot: Optional[TreeNode]) -> bool:
        # Helper function to check if two trees are equal in value and structure
        def checkEqual(root1, root2):
            if not root1 and not root2:
                return True
            elif not root1 or not root2:
                return False
            elif root1.val != root2.val:
                return False
            else:
                return checkEqual(root1.left, root2.left) and checkEqual(root1.right, root2.right)
        
        # Traverse through the root tree and check if any subtree matches the subRoot tree
        if not root:
            return False
        elif checkEqual(root, subRoot):
            return True
        else:
            return self.isSubtree(root.left, subRoot) or self.isSubtree(root.right, subRoot)
```

---

#### Top view of binary tree.

**ALGO:**
1. We will do normal level order traversal.

```python
def topView(root):
    # * keeping two values 1. hd (horizontal distance), 2. Node
    queue = [(0, root)]
    # ? Created dictionary to keep first value appear at horizantal distance
    dict = {}
    dict[0] = root.info
    while len(queue) > 0:
        hd, curr = queue.pop(0)

        # * add to our dict only if it not filled already for topview or replace for bottom view
        if hd not in dict:
            dict[hd] = curr.info

        if curr.left is not None:
            queue.append((hd-1, curr.left))

        if curr.right is not None:
            queue.append((hd+1, curr.right))

    # ? Print dictianary values in sorted dicr with key
    for key in sorted(dict):
        print(dict[key], end=" ")

```
