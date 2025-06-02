# 🌐 Graph Visualizer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Live Demo](https://img.shields.io/badge/Demo-Live-brightgreen)](https://your-demo-link.com)

A lightweight, web-based graph visualization tool that supports both **Adjacency List** and **Edge List** inputs. Visualize **directed** or **undirected** graphs with optional **weighted** edges in an interactive, user-friendly interface.


## ✨ Features

- 📊 **Dual Input Formats** - Support for both Adjacency List and Edge List
- 🎯 **Graph Types** - Toggle between directed and undirected graphs
- ⚖️ **Weighted Edges** - Optional edge weight visualization
- 🖱️ **Interactive Visualization** - Powered by [vis-network](https://visjs.github.io/vis-network/)
- 🎨 **Clean UI** - Intuitive interface with dynamic configuration options
- 🚀 **No Setup Required** - Works entirely client-side
- 📱 **Responsive Design** - Works on desktop and mobile devices

## 🚀 Quick Start

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- No server setup or installation required

### Usage

1. **Select Input Type** - Choose between Adjacency List or Edge List
2. **Enter Graph Data** - Input your graph using the appropriate format
3. **Configure Options** - Toggle directed/undirected and weighted options
4. **Visualize** - Click "Draw Graph" to render your visualization

## 📝 Input Formats

### Adjacency List Format

Maps each node to its connected neighbors with optional weights.

**Syntax:** `node: (neighbor1, weight1), (neighbor2, weight2), ...`

```
1: (2, 4), (3, 5)
2: (3, 2), (4, 1)
3: (4, 3)
4: (1, 2)
```

**Unweighted Example:**
```
A: B, C, D
B: C, E
C: D
D: E
```

### Edge List Format

JSON array where each edge is represented as `[from, to, weight?]`.

**Weighted Example:**
```json
[
  [1, 2, 4],
  [2, 3, 2],
  [3, 4, 3],
  [4, 1, 2]
]
```

**Unweighted Example:**
```json
[
  ["A", "B"],
  ["B", "C"],
  ["C", "D"],
  ["D", "A"]
]
```

## 🎮 Interactive Features

- **Drag & Drop** - Move nodes to customize layout
- **Zoom & Pan** - Navigate large graphs easily
- **Node Selection** - Click nodes and edges for details
- **Export Options** - Save visualizations as images


## 🌐 Deployment

Deploy instantly on any static hosting platform:

### GitHub Pages
1. Fork this repository
2. Enable GitHub Pages in repository settings
3. Access via `https://yourusername.github.io/graph-visualizer`

### Vercel
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
```

### Netlify
1. Drag and drop your project folder to [Netlify](https://app.netlify.com/)
2. Or connect your GitHub repository for automatic deployments

### Local Development
```bash
# Simply open the HTML file in your browser
open index.html

# Or serve with Python
python -m http.server 8000

# Or with Node.js
npx serve .
```

## 🔧 Technical Details

### Dependencies
- **vis-network** - Graph visualization library (loaded via CDN)
- **Pure HTML/CSS/JavaScript** - No build process required

### Browser Support
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Performance
- Handles graphs with 1000+ nodes efficiently
- Optimized rendering with WebGL acceleration
- Responsive performance on mobile devices

## 📚 Examples

### Social Network Graph
```
Alice: Bob, Charlie, David
Bob: Alice, Eve
Charlie: Alice, Frank
David: Alice, Bob
Eve: Bob, Frank
Frank: Charlie, Eve
```

### Weighted Road Network
```json
[
  ["CityA", "CityB", 150],
  ["CityB", "CityC", 200],
  ["CityC", "CityD", 100],
  ["CityA", "CityD", 300]
]
```

### Computer Network Topology
```
Router1: (Switch1, 100), (Switch2, 100)
Switch1: (PC1, 10), (PC2, 10), (PC3, 10)
Switch2: (Server1, 1000), (Server2, 1000)
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Development Guidelines
- Follow existing code style
- Add comments for complex logic
- Test with various graph sizes
- Update documentation as needed

## 🐛 Issue Reporting

Found a bug or have a feature request? Please check existing issues first, then create a new one with:

- Clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Browser and version information
- Sample graph data (if applicable)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## 🙏 Acknowledgments

- [vis-network](https://visjs.github.io/vis-network/) for the amazing graph visualization library
- Community contributors and testers
- Open source graph theory resources

## 📞 Support

- 📧 **Email:** sgr92111@gmail.com
- 🐙 **GitHub Issues:** [Report a bug](https://github.com/sabadusaiganeshreddy/graph-visualizer/issues)
- 💬 **Discussions:** [Join the conversation](https://github.com/sabadusaiganeshreddy/graph-visualizer/discussions)

---

<div align="center">

**⭐ Star this repo if you find it helpful!**

Made with ❤️ by [Sai Ganesh Reddy](https://github.com/sabadusaiganeshreddy)


</div>
