# 📊 Readahead Delay Prediction using Neural Networks and Decision Trees

## 📘 Overview

This project predicts **readahead delay** based on sequential read/write operations stored in text files. The data is processed into labeled **pandas DataFrames**, visualized using **t-SNE**, and then used to train predictive models. The project includes a **4-layer neural network** and a **Decision Tree Classifier** for making predictions.

## ✨ Key Features

- 📄 **Data Preprocessing**: Reads from input text files, labels the data into **Second**, **Ino**, and **Transactions**, and stores it in **pandas DataFrames** for further processing.
  
- 📊 **Data Visualization**: Implements **t-SNE** (t-distributed Stochastic Neighbor Embedding) to visualize the relationships between different features in the dataset.

- 🧠 **Neural Network**: A **4-layer neural network** is used to predict the readahead delay with high accuracy, making use of dense layers and activation functions for complex pattern recognition.

- 🌲 **Decision Tree Classifier**: An alternative model using a **Decision Tree Classifier** for making predictions, which offers a different approach based on feature splits and decision rules.

## 🛠️ Project Workflow

### 1. **Data Ingestion and Labeling**
   - The program reads text files containing sequential operations.
   - The data is labeled into **Second**, **Ino** (inode), and **Transactions** fields.
   - These labels are then loaded into **pandas DataFrames** for further manipulation.

### 2. **Data Visualization**
   - **t-SNE** is used to visualize high-dimensional data in a lower-dimensional space, offering insights into the distribution and relationships of the input features.
   
### 3. **Neural Network for Prediction**
   - A **4-layer neural network** is trained to predict readahead delay based on the labeled data:
     - **Input Layer**: Processes the pandas DataFrame inputs.
     - **Hidden Layers**: Three dense hidden layers with activation functions to learn complex patterns.
     - **Output Layer**: Provides the predicted readahead delay.
   
### 4. **Decision Tree Classifier**
   - A **Decision Tree Classifier** is trained as an alternative predictive model, offering a simpler, rule-based approach to prediction.


## 📈 Models Used

### Neural Network
- **Architecture**: 4-layer dense neural network.
- **Activation Functions**: Utilizes activation functions like ReLU for hidden layers and softmax or linear activation for the output layer.

### Decision Tree Classifier
- **Splitting Criteria**: Uses entropy or Gini index for splitting the nodes.
- **Tree Depth**: Limited to a specific depth to avoid overfitting.
