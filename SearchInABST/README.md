My solution uses recursion to search for a value in a Binary Search Tree.
- First, I check if the current node is null or if it contains the target value.
- If the target value is smaller than the current node, I search in the left subtree.
- If the target value is greater, I search in the right subtree.
- The algorithm continues until it finds the value or reaches a null node.
Because a BST stores smaller values on the left and greater values on the right, I don't need to check every node.
2. Time Complexity
- Average case: O(log n)
- Worst case: O(n)
Why?

In a balanced BST, each step eliminates approximately half of the remaining nodes. Therefore, the algorithm takes O(log n) time.

In the worst case, the tree can be unbalanced, looking like a linked list. Then we may need to visit every node, which takes O(n) time.
3. Space Complexity
- Average case: O(log n)
- Worst case: O(n)
The space is used by recursive function calls. The number of calls depends on the height of the tree.
4. Possible Improvement
An iterative solution using a while loop can reduce extra memory usage because it does not use recursive function calls. Its time complexity remains the same.
