# 🌐 2D Array DSA Patterns

**Author: Rudrika Sharma**

A complete collection of essential 2D array (matrix) patterns to solve interview-level problems from 0 → 100.

---

## 🥉 2D ARRAY PATTERNS (with Examples)

### 1. 🔁 Matrix Traversal

> Use for printing rows, columns, diagonals, or snake-like patterns.

**🧠 Technique**:

* Use nested `for` loops
* Customize based on row-first or column-first traversal

**🔹 Examples**:

* Row-wise & column-wise traversal
* Print diagonals (left-to-right / right-to-left)
* Zigzag or snake pattern print
* Spiral Matrix (Leetcode 54)

---

### 2. 🔃 In-Place Rotation (90° / 180° / 270°)

> Used when rotating a square matrix without extra space.

**🧠 Technique**:

* Step 1: Transpose the matrix
* Step 2: Reverse rows (for 90° clockwise) or columns (for 90° anti-clockwise)

**🔹 Examples**:

* Rotate Image (Leetcode 48)
* Rotate Matrix Variants

---

### 3. ➕ 2D Prefix Sum (Matrix Sum Queries)

> For fast submatrix sum queries.

**🧠 Technique**:

* Preprocess matrix to build prefix sum `pre[i][j]`
* Query: `sum = pre[r2][c2] - pre[r1-1][c2] - pre[r2][c1-1] + pre[r1-1][c1-1]`

**🔹 Examples**:

* Range Sum Query 2D – Immutable (Leetcode 304)
* Matrix Block Sum (Leetcode 1314)

---

### 4. 🔲 Sliding Window on Matrix

> For fixed-size max/min/sum in a window (e.g., 3x3 sliding window).

**🧠 Technique**:

* Brute force or use a Deque
* Move window across matrix, compute sum/max

**🔹 Examples**:

* Maximum Sum Submatrix No Larger Than K (Leetcode 363)
* Max in Sliding Matrix Window

---

### 5. 🧱 DFS / BFS on Grids

> When exploring components (e.g., islands, regions, coloring).

**🧠 Technique**:

* Use DFS/BFS with visited matrix
* Track 4 or 8 direction movement using `dx[]` and `dy[]` arrays

**🔹 Examples**:

* Number of Islands (Leetcode 200)
* Flood Fill (Leetcode 733)
* Surrounded Regions
* Pacific Atlantic Water Flow (Leetcode 417)

---

### 6. 🤭 Directional Movement

> For grid traversal in 4 or 8 directions.

**🧠 Technique**:

```java
int[] dx = {-1, 0, 1, 0};
int[] dy = {0, 1, 0, -1}; // right, down, left, up
```

**🔹 Examples**:

* Path Finding
* Word Search (Leetcode 79)

---

### 7. 🚧 Boundary & Edge Handling

> Critical for avoiding `ArrayIndexOutOfBounds`.

**🧠 Technique**:

* Always check: `0 <= newX < rows` and `0 <= newY < cols`

**🔹 Examples**:

* Any DFS/BFS matrix problem
* Spiral Matrix traversal

---

### 8. 💣 Backtracking in Grid

> Use when you need to try all paths or combinations.

**🧠 Technique**:

* Recursively explore options
* Backtrack by undoing the move

**🔹 Examples**:

* Word Search (Leetcode 79)
* Unique Paths III (Leetcode 980)
* Rat in a Maze (classic)

---

### 9. 🧰 Dynamic Programming on 2D Grid

> For finding paths, minimum cost, obstacle handling.

**🧠 Technique**:

* Use `dp[i][j]` to store result at cell (i, j) based on subproblems
* Carefully handle edges, base cases

**🔹 Examples**:

* Unique Paths (Leetcode 62)
* Minimum Path Sum (Leetcode 64)
* Unique Paths II (Leetcode 63, with obstacles)

---

### 10. 🦄 Union-Find (Disjoint Set) in Grid

> For dynamic connectivity & island merging in grid-based problems.

**🧠 Technique**:

* Map each 2D cell to a 1D index → `row * n + col`
* Apply union-find (with path compression + union by rank)

**🔹 Examples**:

* Number of Islands II (Leetcode 305)
* Similar String Groups (grid-style logic)

--


---

## ✅ Ready-to-solve Problems (Practice Ladder)

* [ ] Rotate Image (Leetcode 48)
* [ ] Number of Islands (Leetcode 200)
* [ ] Word Search (Leetcode 79)
* [ ] Spiral Matrix (Leetcode 54)
* [ ] Flood Fill (Leetcode 733)
* [ ] Range Sum Query 2D (Leetcode 304)
* [ ] Maximum Sum Submatrix (Leetcode 363)
* [ ] Unique Paths (Leetcode 62)
* [ ] Minimum Path Sum (Leetcode 64)
* [ ] Unique Paths II (Leetcode 63)
* [ ] Spiral Matrix II (Leetcode 59)
* [ ] Number of Islands II (Leetcode 305)


---
