# 🧠 MST Algorithm Comparison: Kruskal vs Prim
This notebook compares two fundamental greedy algorithms—Kruskal's and Prim's—for solving the Minimum Spanning Tree (MST) problem in undirected weighted graphs. It includes:

Detailed implementations of both algorithms in Python.

Random graph generation for experimentation.

Runtime comparison using multi-threading.

Printed outputs of MSTs and execution times.

# 📌 Features
✅ Generate a complete weighted undirected graph with random weights.

✅ Implement both Kruskal's and Prim's algorithms from scratch.

✅ Use threading to compare performance in parallel.

✅ Print results and time taken for both algorithms.

# 📂 Project Structure
Graph Generator: Creates a set of vertices and all possible edges with random weights.

Prim’s Algorithm: Greedily grows MST by adding the minimum edge connecting the current tree to a new vertex.

Kruskal’s Algorithm: Sorts all edges and adds the shortest non-cycling edge using a disjoint-set data structure.

Performance Comparison: Executes both algorithms in parallel threads and compares their runtime and MST output.

# 🔧 Dependencies
Make sure to install the following libraries (if not already installed):

bash
Copy
Edit
pip install pandas numpy
# 🚀 How to Run
You can run the notebook in any Jupyter-compatible environment. No external datasets are required—graphs are generated dynamically.

# 📊 Sample Output
rust
Copy
Edit
Kruskal's Minimum Spanning Tree:
('A', 'C', 1)
('A', 'B', 2)
...

Prim's Minimum Spanning Tree:
('A', 'C', 1)
('C', 'B', 2)
...

Time taken by Kruskal's algorithm: 0.0005 seconds  
Time taken by Prim's algorithm: 0.0007 seconds  
# 🧠 Key Learning Points
Prim’s Algorithm is often more efficient for dense graphs when implemented with a priority queue.

Kruskal’s Algorithm is simpler for sparse graphs and uses union-find for cycle detection.

Execution time can vary based on graph size and density.

Threading allows for clean parallel performance benchmarking.

# 📎 Notes
This implementation is for educational purposes and may not be optimized for very large graphs.

All graph data is stored in a pandas.DataFrame for ease of manipulation and visualization.
