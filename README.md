# Java Data Structures & Algorithms

Four Java projects covering data structures, graph algorithms, machine learning, and game development.

---

## Projects

### Path Finding with Dijkstra
A tile-based path finding system built on a custom graph implementation using Dijkstra's algorithm. Supports three strategies:

- **ShortestPath** — minimizes total distance (edge count)
- **SafestShortestPath** — avoids high-risk tiles while minimizing distance
- **FastestPath** — minimizes total travel time, with special handling for metro tiles

Key classes: `Graph`, `GraphTraversal` (BFS), `PathFindingService`, `TilePriorityQ` (custom min-heap)

---

### Snake Game
An interactive snake/caterpillar game rendered with Java AWT. The caterpillar grows by consuming food items, changes color across evolution stages, and navigates a 20×20 grid.

Key classes: `Caterpillar` (linked segment list), `Position`, `EvolutionStage`, `GameColors`, `JerrysPlayground` (AWT game loop)

---

### Civilization Mini Game
A turn-based strategy game featuring a custom linked list of military units on a tile map. Units include Archers, Warriors, Settlers, and Workers, each with attack and movement logic.

Key classes: `MilitaryUnit`, `ListOfUnits` (custom linked list), `Tile`, `Archer`, `Warrior`, `Settler`, `Worker`

---

### Decision Tree
A binary decision tree classifier trained on numerical datasets. Splits nodes by selecting the attribute and threshold that maximize information gain (Gini impurity). Supports serialization for saving and loading trained models.

Key classes: `DecisionTree`, `DTNode` (recursive tree structure), `Datum`, `DataReader`

---

## Build & Run

Open any project folder in IntelliJ IDEA (`.iml` files are included) or compile manually:

```bash
javac -d out src/*.java
java -cp out Main
```
