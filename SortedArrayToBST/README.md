My solution uses recursion and the divide-and-conquer approach to create a height-balanced Binary Search Tree.
- First, I find the middle element of the sorted array.
- I create a new tree node using this middle element.
- Then, I recursively build the left subtree using the elements before the middle.
- After that, I build the right subtree using the elements after the middle.
- The process continues until there are no elements left.
I choose the middle element because it helps distribute values evenly between the left and right subtrees.
Example
For the array:

[-10, -3, 0, 5, 9] 

2. Time Complexity
O(n)

Why?

Every element in the array is processed exactly once to create a tree node. Therefore, if the array contains n elements, the algorithm performs n node creations.
3. Space Complexity
O(n)

The resulting tree contains n nodes. Additionally, recursive calls require O(log n) stack space because the tree is balanced.

The total auxiliary space, excluding the output tree, is O(log n).
4. Possible Improvement
The solution already has optimal O(n) time complexity because every array element must be used to create a node.

There is no need for a more efficient time complexity.
