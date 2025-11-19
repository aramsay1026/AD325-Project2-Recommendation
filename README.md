# Hash-Based Recommendation System

A Python recommendation system that uses a custom hash table and max heap to suggest items (games) to users based on purchase history.
It computes user-to-user similarity with Jaccard similarity and ranks candidate items by priority using a manually implemented max heap.

## What It Does

* Stores user → item interactions in a custom `HashTable`
* Supports **two collision avoidance techniques**:

  * `separate_chaining`
  * `double_hashing`
* Computes **Jaccard similarity** between a target user and all other users
* Aggregates similarity scores into **item scores** (items recommended by many similar users get higher priority)
* Uses a **MaxHeap** to keep the highest-scoring items at the top
* Generates **top-N recommendations** for each user
* Measures and prints:

  * Insertion time
  * Retrieval time per user
  * Number of collisions per technique
* Includes a UML diagram and Git branching/merging screenshots as required for the assignment

## Technologies Used

* **Python 3.x**
* **Jupyter Notebook** (`recommendation_system.ipynb` for all code, analysis, and output)

## How to Run

1. **Clone this repository:**

   ```bash
   git clone https://github.com/aramsay1026/AD325-Project2-Recommendation.git
   cd AD325-Project2-Recommendation
   ```

2. **Open the notebook in Jupyter (or VS Code with Jupyter support):**

   ```bash
   jupyter notebook recommendation_system.ipynb
   ```

3. **Run all cells from top to bottom:**


