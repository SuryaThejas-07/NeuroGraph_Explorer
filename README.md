# NeuroGraph Explorer: Karate Club GCN with Animation

## Project Description

This project demonstrates a Graph Convolutional Network (GCN) applied to the classic Karate Club dataset. The primary goal is to illustrate how GCNs can learn meaningful representations from graph structures to perform node classification. We will load and preprocess the graph data, define and train a GCN model to classify nodes into distinct 'countries', and visualize the entire training process as well as the final learned node embeddings. The visualizations will include animated 2D graph representations and animated 3D scatter plots of node embeddings, showcasing how the model refines its understanding of node relationships over epochs.

## Setup and Installation

To run this project, you need to have the necessary Python libraries installed. You can install them using `pip`:

```bash
!pip install torch_geometric
!pip install optuna
```

## How to Run

1.  **Clone the repository (if applicable) or open the Colab Notebook.**
2.  **Install Dependencies:** Run the cell containing the `pip install` commands.
3.  **Load Data and Preprocess:** Execute the cells to load the Karate Club dataset and perform initial data transformations (e.g., converting to Pandas DataFrames, assigning synthetic labels).
4.  **Define and Initialize Model:** Run the cell that defines the `GCN` class and initializes the model.
5.  **Train the Model:** Execute the training loop cell. This will train the GCN and store intermediate embeddings, losses, and accuracies.
6.  **Visualize Results:** Run the cells for 2D and 3D visualizations to see the animated training process and final node embeddings.

## Visualizations

### 2D Graph Animation

This animation shows the graph structure with nodes colored according to the model's predicted class at different training epochs. It helps to understand how the GCN learns to cluster nodes with similar characteristics.

<!-- Attach your 2D visualization output here -->

### 3D Embeddings Visualization

This 3D plot displays the learned node embeddings, with each point representing a node and colored by its ground truth label. As the model trains, you can observe how nodes of the same class move closer together in the embedding space.

<!-- Attach your 3D visualization output here -->

## Technologies Used

*   **Python**
*   **PyTorch**
*   **PyTorch Geometric (PyG)**
*   **NetworkX**
*   **Matplotlib**
*   **NumPy**
*   **Pandas**
