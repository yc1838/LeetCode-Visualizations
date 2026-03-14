# Word Search Visualization: Hardcore Debugging Guide

Welcome to the **"FUCK YOU" Hardcore Edition** of Word Search! This visualization is designed for developers who want to see every single bone and muscle of a backtracking algorithm.

## 🚀 Quick Start

1. **Run**: Executes the algorithm at the speed set by the slider.
2. **Pause**: Freezes time instantly.
3. **Step Forward**: Moves the algorithm forward by exactly one decision point.
4. **Step Backward**: **[NEW]** Reverses time by one decision point using state snapshots.
5. **FUCK YOU MODE**: Loads a stress-test board for maximum chaos.

## 🛠 Hardcore Debugging Features

### 1. Dual-Footprint System

* **👣 Active Path (Cyan)**: Cells currently in the recursion stack. If the algorithm is at these cells, they are part of the `visited` set. They disappear when the algorithm backtracks.
* **🐾 Traversed (Faint)**: A permanent history of where the algorithm has ever been. These never disappear, showing you the full extent of the search area.

### 2. Logic Explainer

* **Narrator**: The top-right box tells you in plain Chinese what the algorithm is "thinking" (e.g., "Found 'A', looking for 'B' north...").
* **Pseudo-code**: The code block on the left highlights the EXACT line of code being executed in the underlying DFS function.

### 3. Decisions & Statistics

* **Decision Box (Center-Right)**: Shows the 4 directions (N, S, E, W) from the current focus cell. It lights up green for success, red for failure, and blue for active scanning.
* **Pruning Metrics**: Hard numbers on why branches were cut (Out of Bounds, Already Visited, or Mismatch).

### 4. Call Stack

* **Recursion Depth**: Monitor how deep the nested function calls go.
* **Status Labels**:
  * `[MATCH]`: Found a valid character.
  * `[FAIL]`: Hit a wall/mismatch.
  * `[BACKTRACK]`: All neighbors failed, retracting.

---

*Developed for hardcore debugging. Don't just solve it, understand why every branch failed.* 🤬🔥🚀
