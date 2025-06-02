# Graph Visualizer

A simple web-based graph visualizer that lets you input a graph as either an **Adjacency List** or an **Edge List**, supporting **directed/undirected** and **weighted/unweighted** graphs.

---

## Features

- Input graphs as:
  - **Adjacency List**  
    Format example:  
    ```
    1: (2, 4), (3, 5)
    2: (3, 2)
    ```
    Each target node optionally has a weight `(node, weight)`.

  - **Edge List** (JSON array)  
    Format example:  
    ```
    [[1, 2, 4], [2, 3], [3, 1, 1]]
    ```
    Each edge is an array `[from, to, weight?]` — weight is optional.

- Toggle between **directed** and **undirected** edges.
- Toggle **weighted** to show or hide edge weights.
- Visual graph rendering with [vis-network](https://visjs.github.io/vis-network/).

---

## How to Use

1. Choose input type: **Adjacency List** or **Edge List**.
2. Enter your graph data in the text area.
3. Check the **Directed** box if your graph is directed.
4. Check the **Weighted** box to display edge weights.
5. Click **Draw Graph** to visualize.

---

## Deployment

1. Save the `index.html` file.
2. Upload it to any static hosting service (GitHub Pages, Vercel, Netlify, etc.).
3. Open the page in a modern browser.

---

## Dependencies

- [vis-network](https://visjs.github.io/vis-network/) loaded via CDN.

---

## Example Inputs

**Adjacency List (weighted):**
```
1: (2, 4), (3, 5)
2: (3, 2)
```

**Edge List:**
```json
[[1, 2, 4], [2, 3], [3, 1, 1]]
```

---


Feel free to contribute or report issues!
