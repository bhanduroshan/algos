For this problem, I have created a priority queue using a linked list. For priority queue, the append function has to look for proper position to insert the element. So it has complexity of O(n). The pop function has O(1) complexity. The huffman_encoding takes constructs of list of dictionaries with alphabet as key and its frequency as value. This takes O(n) complexity. This list is then used to construct priority queue which is O(n) complexity. Finally once a tree is constructed, we then traverse the tree using recursion to find the huffman encoding for each unique alphabet.  The traverse_tree_get_encoding function used to find encoding for each alphabet, uses recursion. For each node in the tree it recursively finds the solution for left child and right child. This way, it has to travel all the nodes once. Hence the overall complexity of this function is, O(n). Finally using a dictinory of encoding for each alphabet, we then encode the string bit by bit and this operation has to make get query in the dictonary, which also takes O(n) for n alphabets. Hence the overall compelxity of this program is O(n).