# Approximation Algorithms — Visual Simulator

A college demo project featuring interactive step-by-step visualizations of three approximation algorithms.

## Project Files

| File | Description |
|------|-------------|
| index.html | Interactive visual simulator (open in any browser) |
| ApproximationAlgorithms.pptx | 10-slide presentation deck |
| speech.md | Full speech script for 3 presenters + Q&A |
| README.md | This file |

## How to Run

Open index.html in any modern browser (Chrome, Firefox, Edge). No installation needed.
Open ApproximationAlgorithms.pptx in Microsoft PowerPoint or Google Slides.

## Algorithms Covered

### 1. TSP — Nearest Neighbor
- Problem: Find shortest route visiting all N cities, return to start
- Algorithm: At each step, move to nearest unvisited city
- Complexity: O(n^2) | Approx Ratio: O(log n)
- Demo: Approx ~455, Optimal 380, Ratio 1.2x

### 2. Knapsack — Greedy by Value/Weight Ratio
- Problem: Maximize value packed within weight limit
- Algorithm: Sort by V/W ratio, pick greedily
- Complexity: O(n log n) | Approx Ratio: >= 0.5
- Demo: Greedy = 23, Optimal = 26, Ratio 0.88x

### 3. Vertex Cover — 2-Approximation
- Problem: Smallest vertex set covering all edges
- Algorithm: Pick any uncovered edge, add BOTH endpoints
- Complexity: O(V+E) | Approx Ratio: exactly 2
- Demo: Approx = 6 nodes, Optimal = 4, Ratio 1.5x

## Simulator Features

- Three algorithm tabs with independent controls
- Next / Prev step buttons + Auto-play with speed control
- Live SVG graph animation with glowing nodes and edges
- Step trace panel with done / current / pending status
- Input data table updating in real time
- Final Result Box with ratio and comparison bar chart

## Comparison Summary

| Algorithm | Approx | Optimal | Ratio | Complexity |
|-----------|--------|---------|-------|------------|
| TSP (Nearest Neighbor) | ~455 | 380 | 1.20x | O(n^2) |
| Knapsack (Greedy) | 23 val | 26 val | 0.88x | O(n log n) |
| Vertex Cover (2-Approx) | 6 nodes | 4 nodes | 1.50x | O(V+E) |

## Team Roles

| Role | Covers |
|------|--------|
| Person 1 | Introduction, TSP Problem & Demo (Slides 1-4) |
| Person 2 | Knapsack Problem & Demo (Slides 5-6) |
| Person 3 | Vertex Cover, Comparison, Conclusion (Slides 7-10) |

## Key Concept

An approximation algorithm runs in polynomial time and produces a solution guaranteed to be within a factor alpha of the optimal. For minimization: output <= alpha x OPT. For maximization: output >= alpha x OPT.

## References

1. Vazirani, V. V. (2001). Approximation Algorithms. Springer.
2. Cormen et al. Introduction to Algorithms (CLRS), Chapter 35.
3. Williamson & Shmoys. The Design of Approximation Algorithms. Cambridge.

## Tips for Demo

- Open simulator in full-screen browser before starting
- Use Auto mode for smooth animated demos
- Pause at each highlighted step and explain it
- Point at Result Box at the end to show the ratio
- Reset before each live demo
