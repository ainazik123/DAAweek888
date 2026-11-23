My solution uses recursion to calculate the sum of all nodes within the given range.
- First, I check if the current node is null. If it is null, I return 0.
- Then, I check if the current node's value is between low and high.
- If the value is inside the range, I add it to the sum.
- If the current value is greater than low, I search in the left subtree.
- If the current value is smaller than high, I search in the right subtree.
- Finally, I return the total sum.
The main advantage is that I don't visit unnecessary branches of the tree.
2. Time Complexity
- Average case: O(n)
- Worst case: O(n)
Why?

In the worst case, the algorithm may need to visit every node in the tree to calculate the correct sum.

However, because of the BST properties, some branches can be skipped when their values are outside the required range.
3. Space Complexity
- Average case: O(log n)
- Worst case: O(n)
The recursive calls use memory depending on the height of the tree.
4. Possible Improvement
The solution already uses BST properties to skip unnecessary branches. This makes it more efficient than simply traversing every node without checking the range.
