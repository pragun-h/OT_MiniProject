#  Emergency Vehicle Path Optimization

An interactive **browser-based simulation** that demonstrates how **Dijkstra’s Shortest Path Algorithm** can optimize routes for emergency vehicles such as ambulances, fire trucks, and police units.

This project models a **city road network as a weighted graph**, where:

* **Nodes = intersections / locations**
* **Edges = roads**
* **Weights = travel cost (distance + traffic)**

The system dynamically finds the **fastest possible route** while adapting to:

* 🚦 Rush-hour traffic
* 🚧 Road blockages
* 🚑 Emergency cleared roads

---

##  Project Overview

Fast emergency response can save lives. This project simulates how graph optimization techniques can reduce response time by always selecting the **minimum-cost route**.

Using **Dijkstra’s Algorithm**, the simulation recalculates the best route in real time whenever:

* traffic changes,
* roads are blocked,
* a new city layout is selected.

It is built as a **pure HTML + JavaScript + Canvas project**, so it runs directly in the browser with no backend required.

---

##  Features

* 🗺️ **Interactive city graph simulation**
* ⚡ **Real-time shortest path calculation**
* 🚦 **Traffic modes**

  * Normal
  * Rush Hour
  * Clear Roads
* 🚧 **Road blockage rerouting**
* 🎯 **Optimal path visualization**
* 🔍 **Explored node highlighting**
* 🏙️ Multiple scenarios:

  * Grid City
  * Ring Roads
  * Random Map

---

##  Algorithm Used

### Dijkstra’s Shortest Path Algorithm

The algorithm works by:

1. Starting from the emergency station
2. Expanding the lowest-cost unexplored node
3. Updating neighboring road costs
4. Repeating until the destination is reached
5. Reconstructing the shortest route

### ⏱ Complexity

| Implementation             | Time Complexity |
| -------------------------- | --------------- |
| Array-based Priority Queue | O(V²)           |
| Binary Heap                | O((V+E) log V)  |

This project currently uses an **array-based implementation**, which is efficient for small city graphs.

---

##  Tech Stack

* **HTML5**
* **CSS3**
* **JavaScript (Vanilla JS)**
* **HTML5 Canvas API**

---

##  Project Structure

```text
OT_MiniProject/
│── index.html ── style.css ── script.js
│── README.md
```

---

##  How to Run

### Option 1: Live Demo

🔗 **Live Project:** [https://pragun-h.github.io/OT_MiniProject/](https://pragun-h.github.io/OT_MiniProject/)

### Option 2: Run Locally

```bash
git clone https://github.com/pragun-h/OT_MiniProject.git
cd OT_MiniProject
```

Then open `index.html` in your browser.

---

##  Results

* ⚡ Executes in **under 1 ms** for graphs up to 16 nodes
* 🚧 Successfully reroutes around blocked roads
* 🚦 Avoids congested routes during rush hour
* 🎯 Always guarantees the **provably shortest path**

---

##  Real-World Applications

This project reflects concepts used in:

* Google Maps
* Waze
* Ambulance dispatch systems
* Fire emergency routing
* Disaster management systems

---

##  Future Improvements

* 🌐 OpenStreetMap integration
* 📍 Real GPS-based routing
* 🤖 A* search comparison
* 🚓 Multi-vehicle coordination
* 📈 Better scalability with binary heap
* ⏱ Time-varying traffic weights

---

##  Authors

* **Kalyan Kumar N**
* **Pragun Hagaldivte**

