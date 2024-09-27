# B-Tree
Implementation of a B-tree for the Data Structures II course

A B-tree is a self-balancing tree data structure that maintains sorted data and allows for efficient insertion, deletion, and search operations. It is commonly used in databases and file systems to store large amounts of data that can't fit into memory.

# Key Features: 
1. Balanced Structure: B-trees remain balanced, meaning all leaf nodes are at the same level. This ensures that the tree's height is logarithmic in the number of elements, keeping operations efficient.
2. Multiple Keys per Node: Unlike binary trees, where each node contains only one key and two children, a B-tree node can store multiple keys and have multiple children, depending on a parameter called "order."
3. Efficient Disk Access: B-trees are optimized for systems that read from and write to large blocks of data, like disks, because they minimize the number of disk accesses required by maintaining a wide, shallow structure.
4. Flexible Size: A B-tree's nodes are filled with a range of keys, and the number of children each node has can vary within a predefined range.

# Basic Properties:
- Every node can have at most m children (where m is the order of the B-tree).
- Every node (except the root) must have at least ⌈m/2⌉ children.
- The root node can have as few as two children, but all internal nodes must be partially filled.
- All leaf nodes appear on the same level, which means the tree is balanced.

# Operations:
- Search: Efficiently finds an element by traversing the tree, examining only a few nodes.
- Insertions and Deletions: Maintain balance by redistributing elements or splitting/merging nodes when necessary.
