# 🔍 Maze Solver using BFS and DFS
This project aims to implement an AI agent that utilizes **Breadth-First Search (BFS)** and **Depth-First Search (DFS)** algorithms to solve mazes and compare their performances based on different criteria such as execution time, memory usage, and path optimality.

---

## 📌 Algorithms Overview

### 🟦 Breadth-First Search (BFS)
- Explores nodes level by level.
- Uses a **Queue** (FIFO).
- Guarantees the **shortest path** in unweighted graphs.
- May consume **more memory** due to storing multiple paths at each level.
- Time Complexity: `O(V + E)`

### 🟪 Depth-First Search (DFS)
- Explores as deep as possible before backtracking.
- Uses a **Stack** (or recursion).
- Does **not guarantee** the shortest path.
- Consumes **less memory** in sparse graphs.
- Time Complexity: `O(V + E)`

---

## 🔁 Difference Between BFS and DFS (Points-wise)

- **Traversal Approach:**
  - BFS: Level-wise
  - DFS: Depth-wise

- **Data Structure Used:**
  - BFS: Queue
  - DFS: Stack / Recursion

- **Shortest Path:**
  - BFS: Finds shortest path (in unweighted graphs)
  - DFS: No guarantee of shortest path

- **Memory Usage:**
  - BFS: Higher (stores many nodes at once)
  - DFS: Lower (stores single path)

- **Performance on Sparse Graphs:**
  - BFS: May use more memory
  - DFS: More efficient

- **Cycle Detection:**
  - DFS: Very useful
  - BFS: Can be used but less common

- **Implementation:**
  - DFS: Simpler with recursion
  - BFS: Requires careful queue management

- **Applications:**
  - **BFS**: Shortest path, social networking, AI pathfinding
  - **DFS**: Maze solving, cycle detection, topological sort

---

## 📊 Performance Comparison Criteria

| Metric           | BFS                        | DFS                        |
|------------------|-----------------------------|-----------------------------|
| Path Optimality  | ✅ Always finds shortest path | ❌ May return longer path  |
| Execution Time   | ⚖️ Depends on maze size       | ⚖️ Depends on maze depth   |
| Memory Usage     | ❗ Higher                     | ✅ Lower in most cases     |

---

## 🧰 Libraries Used

- **PyMaze** – For maze generation and visualization
- **Timeit** – For accurate execution time measurement

---

## 🚀 How to Run

Make sure you have Python installed and the required libraries (`pymaze`, `timeit`) available.

### ▶️ Step-by-step:

 **Run BFS Demo**
 
 python bfsdemo.py
   

### **Run DFS Demo**

python dfsdemo.py


###**Run Final Comparison (BFS vs DFS)**

python DFSvsDFS.py

This will show outputs and performance comparison between the two algorithms.

## 🖼️ Sample Outputs

### 🔷 BFS Output (from `bfs.py`)
- Path: (example) [(1,1), (1,2), (1,3), ..., (4,5)]
- Time Taken: X.XXX seconds
- Path Length: XX
- Nodes Visited: XX

![BFS Output](assets/bfs_output.png)

---

### 🔶 DFS Output (from `dfs.py`)
- Path: (example) [(1,1), (2,1), (3,1), ..., (4,5)]
- Time Taken: X.XXX seconds
- Path Length: XX
- Nodes Visited: XX

![DFS Output](assets/dfs_output.png)

---

### 🔁 BFS vs DFS Comparison (from `DFSvsDFS.py`)
- BFS Time: X.XXX seconds | DFS Time: X.XXX seconds  
- BFS Nodes: XX | DFS Nodes: XX  
- BFS Path Length: XX | DFS Path Length: XX

![Comparison Output](assets/comparison_output.png)



📂 Project Structure
maze-quest/
├── bfs.py           # BFS implementation and demo
├── dfs.py           # DFS implementation and demo
├── DFSvsDFS.py      # Final comparison file
├── dfs.csv          # (if any helpers used)
├── maze.py          # Maze generation and logic (PyMaze)
└── README.md        # You're here!


👩‍💻 Team Members
Khushi Pardhi 
Madhura Nilawar
Saloni Chavhan 
Vedika Welukar
Anjali Sune 

🙌 Thank You!
This project demonstrates how classical search algorithms can be applied to solve real-world problems like pathfinding. By comparing BFS and DFS, we can choose the right algorithm depending on the problem's needs.
