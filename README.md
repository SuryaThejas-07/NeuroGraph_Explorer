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

### 2D Graph Visualization

This figure shows the graph structure with nodes colored according to the model's predicted class during training.  
It demonstrates how the Graph Convolutional Network gradually learns meaningful node relationships.

#### Initial Epoch (2D)

![Initial Epoch 2D](https://raw.githubusercontent.com/SuryaThejas-07/NeuroGraph_Explorer/78285222ab596868b8800a8b37fa86ff11c58cfb/initial_epoch_2d.png)

#### Final Epoch (2D)

![Final Epoch 2D](https://raw.githubusercontent.com/SuryaThejas-07/NeuroGraph_Explorer/78285222ab596868b8800a8b37fa86ff11c58cfb/final_epoch_2D.png)

---

### 3D Embeddings Visualization

The 3D scatter plot represents node embeddings learned by the GCN.  
Each point corresponds to a node, and nodes belonging to the same class tend to cluster together.

#### Initial Epoch (3D)

![Initial Epoch 3D](https://raw.githubusercontent.com/SuryaThejas-07/NeuroGraph_Explorer/78285222ab596868b8800a8b37fa86ff11c58cfb/initial_epoch_3d.png)

#### Final Epoch (3D)

![Final Epoch 3D](https://raw.githubusercontent.com/SuryaThejas-07/NeuroGraph_Explorer/78285222ab596868b8800a8b37fa86ff11c58cfb/final_epoch_3d.png)

## Technologies Used

*   **Python**
*   **PyTorch**
*   **PyTorch Geometric (PyG)**
*   **NetworkX**
*   **Matplotlib**
*   **NumPy**
*   **Pandas**

## Project Workflow

1. Load the Karate Club dataset using PyTorch Geometric.
2. Preprocess graph data and assign labels.
3. Build a Graph Convolutional Network (GCN).
4. Train the model for node classification.
5. Store node embeddings at different epochs.
6. Visualize graph learning using 2D and 3D plots.

## Dataset

This project uses the **Karate Club Graph Dataset**, a classic benchmark in graph machine learning.

Features:
- 34 nodes (club members)
- 78 edges (relationships)
- Used for node classification tasks
- Popular dataset for testing Graph Neural Networks

## Model Architecture

The model used is a **Graph Convolutional Network (GCN)** consisting of:

- Input Layer
- Graph Convolution Layer
- ReLU Activation
- Graph Convolution Layer
- Softmax Output

The model learns node embeddings by aggregating information from neighboring nodes.

## Training Details

- Optimizer: Adam
- Loss Function: CrossEntropyLoss
- Epochs: 200
- Learning Rate: 0.01

During training, embeddings were stored at each epoch to visualize how node representations evolve.


## Author

**Surya Thejas**

Computer Science Student  
Interested in AI, Machine Learning, and Graph Neural Networks.
