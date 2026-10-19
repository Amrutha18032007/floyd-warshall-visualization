# Floyd–Warshall Algorithm Visualization

 Project Overview

The **Floyd–Warshall Algorithm Visualization** is an interactive web-based project that demonstrates how the Floyd–Warshall algorithm calculates the shortest distances between every pair of vertices in a weighted graph.

The project visually represents the distance matrix at each iteration, helping users understand how shortest paths are updated using intermediate vertices.

 Objectives

- Understand the working of the Floyd–Warshall algorithm.
- Visualize distance matrix updates step by step.
- Identify how intermediate vertices improve shortest paths.
- Learn the All-Pairs Shortest Path problem interactively.

 Features

- **Interactive Visualization:** View the distance matrix at every iteration.
- **Step-by-Step Updates:** Move forward and backward through the algorithm.
- **Distance Highlighting:** Changed distances are highlighted in green.
- **Reset Option:** Restart the visualization from the initial matrix.
- **Final Shortest-Path Matrix:** View the computed shortest distances between all vertex pairs.
- **Browser-Based Application:** Runs directly in a web browser without additional software libraries.

 Algorithm Used

The project implements the **Floyd–Warshall Algorithm**, a dynamic programming algorithm used to find the shortest paths between all pairs of vertices in a weighted graph.

The distance update formula is:

`D[i][j] = min(D[i][j], D[i][k] + D[k][j])`

Where:

- `D[i][j]` represents the current shortest known distance from vertex `i` to vertex `j`.
- `D[i][k]` represents the distance from vertex `i` to intermediate vertex `k`.
- `D[k][j]` represents the distance from vertex `k` to vertex `j`.

The algorithm checks whether travelling through an intermediate vertex provides a shorter path.

 Technologies Used

- **HTML5** – Structures the web page.
- **CSS3** – Styles the interface and distance matrix.
- **JavaScript** – Implements the algorithm and interactive controls.
- **Git and GitHub** – Version control and project hosting.

 How to Run the Project

1. Clone this repository:

   ```bash
   git clone https://github.com/Amrutha18032007/floyd-warshall-visualization.git
   ```

2. Open the project folder in Visual Studio Code.

3. Open `index.html` in your browser, or use the Live Server extension in VS Code.

4. Click **Next Step** to observe the distance matrix updates.

5. Use **Previous** to revisit earlier iterations and **Reset** to restart the algorithm.

 Example

The example graph contains four vertices: A, B, C, and D.

Initial distance matrix:

| From / To | A | B | C | D |
|---|---:|---:|---:|---:|
| A | 0 | 5 | ∞ | 10 |
| B | ∞ | 0 | 3 | ∞ |
| C | ∞ | ∞ | 0 | 1 |
| D | ∞ | ∞ | ∞ | 0 |

Final shortest-distance matrix:

| From / To | A | B | C | D |
|---|---:|---:|---:|---:|
| A | 0 | 5 | 8 | 9 |
| B | ∞ | 0 | 3 | 4 |
| C | ∞ | ∞ | 0 | 1 |
| D | ∞ | ∞ | ∞ | 0 |

Here, `∞` indicates that no path exists between the corresponding vertices in the directed graph.

 Time and Space Complexity

- **Time Complexity:** O(V³)
- **Space Complexity:** O(V²)

Where `V` represents the number of vertices in the graph.

 Learning Outcomes

This project demonstrates the application of dynamic programming, matrix manipulation, graph algorithms, and interactive web development. It provides a visual and practical way to understand the All-Pairs Shortest Path problem.

 Author

**Amrutha Varshini**

GitHub: [@Amrutha18032007](https://github.com/Amrutha18032007)

