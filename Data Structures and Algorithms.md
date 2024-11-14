**Data Structures** and **Algorithms** are fundamental concepts in computer science, playing a crucial role in building efficient and optimized software solutions. They enable the organization, manipulation, and retrieval of data in a structured way, allowing developers to solve problems efficiently.

### 1. **[[Data Structures]]**:

A **data structure** is a way of organizing and storing data so that it can be accessed and modified efficiently. Different data structures are suited for different tasks, and choosing the right one is critical to achieving optimal performance in an application.

#### Common Data Structures:

1. **[[Arrays]]**:
    
    - A collection of elements, typically of the same type, stored in contiguous memory locations. Arrays provide fast access to elements via their indices but can be inefficient when inserting or deleting elements, as this may require shifting elements.
    - **Time Complexity**:
        - Access: O(1)O(1)O(1)
        - Insertion/Deletion: O(n)O(n)O(n) (in the worst case for unsorted arrays)
2. **[[Linked List]]**:
    
    - A linear data structure where each element (node) contains a data part and a reference (pointer) to the next node in the sequence.
    - **Singly Linked List**: Each node points to the next node.
    - **Doubly Linked List**: Each node points to both the next and previous nodes.
    - **Time Complexity**:
        - Access: O(n)O(n)O(n)
        - Insertion/Deletion: O(1)O(1)O(1) (at the beginning or end)
3. **[[Stacks]]**:
    
    - A **Last In, First Out (LIFO)** data structure where elements are added and removed from the same end (the top). Stacks are often used in function call management and recursion.
    - Operations:
        - **Push**: Add an element to the top.
        - **Pop**: Remove an element from the top.
    - **Time Complexity**:
        - Push/Pop: O(1)O(1)O(1)
4. **[[Queues]]**:
    
    - A **First In, First Out (FIFO)** data structure where elements are added at the rear and removed from the front. Queues are useful for managing processes in scheduling systems.
    - Variants:
        - **Circular Queue**: The queue wraps around when it reaches the end.
        - **Priority Queue**: Elements are dequeued based on priority, not the order of insertion.
    - **Time Complexity**:
        - Enqueue/Dequeue: O(1)O(1)O(1)
5. **[[Hash Tables]] ([[Hash Maps]])**:
    
    - A data structure that maps keys to values using a hash function. Hash tables provide fast access, insertion, and deletion of elements.
    - **Time Complexity** (on average):
        - Access/Insertion/Deletion: O(1)O(1)O(1)
    - **Collision Handling**:
        - **Chaining**: Multiple elements are stored in the same index using a linked list.
        - **Open Addressing**: Find the next available slot if a collision occurs.
6. **[[Trees]]**:
    
    - A hierarchical data structure where each node has a value and references to its child nodes. Trees are used to represent hierarchical relationships, such as file systems or organizational structures.
    - **Binary Tree**: Each node has at most two children.
        - **Binary Search Tree (BST)**: A binary tree where the left child is less than the node, and the right child is greater.
    - **Balanced Trees**: Maintain height balance to ensure efficient operations (e.g., **AVL Trees**, **Red-Black Trees**).
    - **[[Time Complexity]]** (BST):
        - Search/Insertion/Deletion: O(log⁡n)O(\log n)O(logn) (in a balanced tree)
7. **[[Heaps]]**:
    
    - A specialized tree-based structure that satisfies the **heap property**:
        - **Max-Heap**: The parent node is greater than its children.
        - **Min-Heap**: The parent node is less than its children.
    - Heaps are used to implement priority queues and efficient algorithms like **Dijkstra's shortest path**.
    - **Time Complexity**:
        - Access max/min: O(1)O(1)O(1)
        - Insertion/Deletion: O(log⁡n)O(\log n)O(logn)
8. **[[Graphs]]**:
    
    - A collection of nodes (vertices) connected by edges. Graphs are used to represent networks like social media, maps, or circuits.
    - Types of Graphs:
        - **Directed**: Edges have a direction.
        - **Undirected**: Edges have no direction.
        - **Weighted**: Edges have weights representing costs.
    - **Time Complexity**:
        - BFS/DFS Traversal: O(V+E)O(V + E)O(V+E) where VVV is the number of vertices and EEE is the number of edges.

### 2. **[[Algorithms]]**:

An **algorithm** is a step-by-step procedure for solving a problem or performing a task. It is defined by a sequence of actions to achieve a goal, typically optimized for time and space efficiency.

#### Common Algorithmic Concepts:

1. **[[Sorting Algorithms]]**:
    
    - Sorting is a fundamental operation to arrange elements in a specific order (ascending or descending).
    - **Bubble Sort**: Repeatedly swaps adjacent elements if they are in the wrong order. O(n2)O(n^2)O(n2)
    - **Selection Sort**: Finds the smallest element and places it at the beginning. O(n2)O(n^2)O(n2)
    - **Insertion Sort**: Builds the sorted array one element at a time. O(n2)O(n^2)O(n2)
    - **Merge Sort**: A divide-and-conquer algorithm that splits the array into halves and merges them in sorted order. O(nlog⁡n)O(n \log n)O(nlogn)
    - **Quick Sort**: Picks a pivot and partitions the array around it, recursively sorting subarrays. O(nlog⁡n)O(n \log n)O(nlogn) (average case)
    - **Heap Sort**: Uses a heap data structure to sort elements. O(nlog⁡n)O(n \log n)O(nlogn)
2. **[[Search Algorithms]]**:
    
    - **Linear Search**: Iterates through each element in a list to find the target. O(n)O(n)O(n)
    - **Binary Search**: Searches a sorted list by repeatedly dividing it in half. O(log⁡n)O(\log n)O(logn)
3. **[[Graph Algorithms]]**:
    
    - **Breadth-First Search (BFS)**: Explores all nodes at the present depth level before moving on to nodes at the next depth level. O(V+E)O(V + E)O(V+E)
    - **Depth-First Search (DFS)**: Explores as far as possible along each branch before backtracking. O(V+E)O(V + E)O(V+E)
    - **Dijkstra's Algorithm**: Finds the shortest path from a source node to all other nodes in a graph with non-negative weights. O(V2)O(V^2)O(V2) (with simple priority queues)
    - **Kruskal’s Algorithm**: Finds the minimum spanning tree of a graph. O(Elog⁡E)O(E \log E)O(ElogE)
    - **Prim’s Algorithm**: Another approach to finding the minimum spanning tree. O(V2)O(V^2)O(V2) (with simple adjacency matrix)
4. **[[Dynamic Programming]] (DP)**:
    
    - A method for solving complex problems by breaking them down into simpler overlapping subproblems and solving them recursively.
    - **Memoization**: Caching intermediate results to avoid redundant calculations.
    - **Fibonacci Sequence**: A classic DP example where each term is the sum of the previous two terms.
    - **Longest Common Subsequence**, **Knapsack Problem** are common DP problems.
    - Time Complexity: Varies depending on the problem but is generally more efficient than brute-force recursion.
5. **[[Greedy Algorithms]]**:
    
    - A technique that makes locally optimal choices at each step with the hope of finding a global optimum.
    - Example: **Activity Selection**, **Huffman Coding**, **Coin Change**.
6. **[[Divide and Conquer]]**:
    
    - A strategy that divides the problem into smaller subproblems, solves each subproblem independently, and combines the solutions.
    - Example: **Merge Sort**, **Quick Sort**, **Binary Search**.
7. **[[Backtracking]]**:
    
    - A technique used to solve problems by exploring all potential solutions and discarding ones that do not meet the criteria (pruning the search space).
    - Example: **N-Queens Problem**, **Sudoku Solver**.
8. **[[Hashing]]**:
    
    - Hashing is used to map data to fixed-size values using a hash function. It provides efficient lookups, insertions, and deletions in a hash table.
    - **Collision resolution** techniques, such as **chaining** or **open addressing**, are necessary to handle multiple values mapped to the same hash value.

### 3. **[[Big-O Notation]]**:

- **Big-O Notation** is a mathematical concept used to describe the **time complexity** or **space complexity** of an algorithm, giving an upper bound on how the runtime or memory usage grows as the input size increases.
    - **O(1)**: Constant time, regardless of input size.
    - **O(log n)**: Logarithmic time, reduces the problem size by a constant factor (e.g., binary search).
    - **O(n)**: Linear time, grows directly with input size (e.g., linear search).
    - **O(n log n)**: Linearithmic time, common in efficient sorting algorithms (e.g., merge sort).
    - **O(n^2)**: Quadratic time, common in algorithms with nested loops (e.g., bubble sort).
    - **O(2^n)**: Exponential time, typically associated with brute-force or combinatorial problems (e.g., recursive Fibonacci).

### 4. **[[Recursion]]**:

- A technique where a function calls itself to solve smaller instances of a problem. Recursion is fundamental in divide-and-conquer algorithms and dynamic programming.
- Key components:
    - **Base Case**: The condition that terminates the recursion.
    - **Recursive Case**: The part of the function that breaks down the problem into smaller instances.

### Summary:

- **Data Structures**: Efficient ways of organizing and storing data, such as arrays, linked lists, trees, and graphs.
- **Algorithms**: Well-defined sequences of steps to solve computational problems, including sorting, searching, graph traversal, dynamic programming, and more.
- Understanding the relationship between data structures and algorithms is crucial for designing efficient software solutions, optimizing both time and space complexity.