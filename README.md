
# Recognizing Handwritten Digits with Neural Networks

## 📌 Project Overview

This project focuses on recognizing handwritten digits using a **Neural Network** and the **MNIST dataset**. The project explores how different training parameters such as **batch size, epochs, and optimization approach** affect model performance.

The MNIST dataset contains **70,000 handwritten digit images** representing digits from **0 to 9**. Each image is a grayscale image of **28 × 28 pixels**.

## 🎯 Objective

* Build a neural network for handwritten digit classification.
* Train the model using the MNIST dataset.
* Experiment with different batch sizes and epochs.
* Compare training and validation accuracy.
* Understand the effect of gradient descent and batch size on model performance.

## 📊 Dataset

**MNIST Dataset**

* Total images: 70,000
* Training images: 60,000
* Testing images: 10,000
* Image size: 28 × 28 pixels
* Image type: Grayscale
* Classes: Digits 0–9
* Pixel values: 0–255

The dataset is loaded directly using TensorFlow/Keras:

```python
(x_train, y_train), (x_test, y_test) = keras.datasets.mnist.load_data()
```

## 🛠️ Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

The notebook imports TensorFlow/Keras for neural-network development and NumPy, Pandas, Matplotlib and Seaborn for data processing and visualization.

## 🔄 Project Workflow

1. Install required libraries
2. Import Python libraries
3. Set random seeds
4. Load the MNIST dataset
5. Explore the dataset
6. Prepare training and validation data
7. Build the neural network
8. Compile the model
9. Train the model
10. Compare different configurations
11. Visualize training performance
12. Analyze accuracy and training time

## 🧠 Model

The project uses a **Sequential Keras neural network** with a Dense output layer and **Softmax activation** for classification into 10 digit classes.

One of the models contains **7,850 trainable parameters** and produces 10 output classes.

## ⚙️ Experiments

Different combinations of **epochs and batch sizes** were tested.

| Epochs | Batch Size | Training Accuracy | Validation Accuracy |       Time |
| -----: | ---------: | ----------------: | ------------------: | ---------: |
|     10 |     50,000 |            15.27% |              16.28% |  12.22 sec |
|     50 |     50,000 |            43.06% |              43.32% |  21.30 sec |
|     10 |         32 |            90.83% |              90.71% |  39.24 sec |
|     50 |         32 |            92.39% |              91.86% | 196.79 sec |

These results show that using a smaller batch size with more frequent parameter updates substantially improved the model's performance.

## 📈 Best Result

The experiment with **50 epochs and batch size 32** achieved:

* Training Accuracy: **92.39%**
* Validation Accuracy: **91.86%**
* Training Loss: **0.2722**
* Validation Loss: **0.2938**
* Training Time: **196.79 seconds**

## 💡 Key Learnings

* MNIST is a useful dataset for learning image classification.
* Batch size has a significant effect on model training.
* Smaller batch sizes allow model parameters to be updated more frequently.
* Increasing epochs can improve accuracy, but it also increases training time.
* The best configuration should consider both **accuracy and computational time**.
* A small improvement in accuracy may not always justify a large increase in training time.

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Open the notebook

Open:

```text
Recognizing_Handwritten_Digits_with_Neural_Networks.ipynb
```

using **Google Colab** or **Jupyter Notebook**.

### 3. Install dependencies

```bash
pip install tensorflow scikit-learn matplotlib seaborn numpy pandas
```

### 4. Run the notebook

Execute the cells sequentially to:

* Load the MNIST dataset
* Train the neural network
* Evaluate the models
* Compare accuracy and training time
* Visualize the results

## 📁 Project Structure

```text
Recognizing-Handwritten-Digits/
│
├── Recognizing_Handwritten_Digits_with_Neural_Networks.ipynb
└── README.md
```

## 🚀 Future Improvements

* Use Convolutional Neural Networks (CNN).
* Apply image preprocessing techniques.
* Tune learning rate and optimizers.
* Add a handwritten digit prediction interface.
* Deploy the trained model as a web application.

## 👨‍💻 Author

**Vasanthaprabhu G. T**

Aspiring Python Developer | Generative AI | SQL | Machine Learning | Full Stack Developer


