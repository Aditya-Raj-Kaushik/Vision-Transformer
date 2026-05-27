# Vision Transformer (ViT) for CIFAR-10 Classification

A PyTorch implementation of a **Vision Transformer (ViT)** model trained on the **CIFAR-10 dataset** for image classification.

This project demonstrates how Transformer architectures can be applied to computer vision tasks by splitting images into patches, embedding them, and processing them using self-attention mechanisms.

---

# 🚀 Overview

Traditional CNNs rely on convolution operations for feature extraction, whereas Vision Transformers treat an image as a sequence of patches similar to tokens in NLP.

This project includes:

- Custom Vision Transformer implementation
- Patch embedding mechanism
- Transformer encoder blocks
- Multi-head self-attention
- CIFAR-10 training pipeline
- Accuracy visualization
- Prediction visualization grid

---

# 🧠 Key Features

## 🔹 Vision Transformer Architecture

- Patch-based image representation
- Learnable positional embeddings
- Multi-head self-attention
- Transformer encoder layers
- MLP classification head

---

## 🔹 CIFAR-10 Image Classification

Classifies images into:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

---

## 🔹 Data Augmentation

Training transformations include:

- Random cropping
- Horizontal flipping
- Color jitter
- Normalization

---

## 🔹 Training & Evaluation

- CrossEntropyLoss
- Adam optimizer
- GPU support (CUDA)
- Accuracy tracking
- Evaluation on test dataset

---

## 🔹 Visualization

- Train vs Test accuracy graph
- Random prediction grid visualization

---

# 🏗️ Model Architecture

```text
Input Image
      ↓
Patch Embedding
      ↓
Positional Embedding
      ↓
Transformer Encoder Layers
      ↓
MLP Head
      ↓
Class Prediction
```

---

# ⚙️ Hyperparameters

```python
BATCH_SIZE = 128
EPOCHS = 10
LEARNING_RATE = 3e-4

PATCH_SIZE = 4
IMAGE_SIZE = 32
CHANNELS = 3

EMBED_DIM = 256
NUM_HEADS = 8
DEPTH = 6
MLP_DIM = 512
DROP_RATE = 0.1
```

---

# 🛠️ Tech Stack

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- tqdm

---

# 📂 Project Structure

```text
VisionTransformer/
│
├── Vision_Transformer.ipynb
├── data/
│   └── CIFAR-10 dataset
├── README.md
└── requirements.txt
```

---

# 📦 Installation

## 1️⃣ Clone Repository

```bash
git clone <your-repo-url>
cd VisionTransformer
```

---

## 2️⃣ Create Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate
```

---

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

Example dependencies:

```text
torch
torchvision
numpy
matplotlib
tqdm
```

---

# ▶️ Run the Notebook

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Vision_Transformer.ipynb
```

Run all cells sequentially.

---

# 📊 Dataset

The project uses the **CIFAR-10 dataset**.

### Dataset Information

- 60,000 color images
- 10 classes
- Image size: 32×32

Dataset is automatically downloaded using Torchvision.

---

# 🔍 Components Implemented

## ✅ Patch Embedding

Converts image patches into embedding vectors using convolution projection.

---

## ✅ Transformer Encoder Layer

Includes:

- Layer Normalization
- Multi-Head Attention
- Residual Connections
- Feed Forward MLP

---

## ✅ Multi-Head Self Attention

Allows the model to learn global relationships between image patches.

---

## ✅ Classification Head

Final MLP layer predicts image class probabilities.

---

# 📈 Training Workflow

1. Load CIFAR-10 dataset
2. Apply augmentations
3. Create patch embeddings
4. Pass through transformer encoder
5. Compute classification loss
6. Backpropagation & optimization
7. Evaluate on test dataset

---

# 📉 Accuracy Visualization

The notebook generates:

- Training accuracy curve
- Testing accuracy curve

to analyze model learning behavior across epochs.

---

# 🖼️ Prediction Visualization

A prediction grid is generated showing:

- Random test images
- Ground truth labels
- Model predictions

---

# 🧪 Example Output

```text
Epoch 1/10
Train Accuracy: 0.71
Test Accuracy: 0.68
```

---

# 📌 Future Improvements

- Pretrained Vision Transformer support
- DeiT implementation
- Mixed precision training
- Learning rate scheduling
- Model checkpointing
- TensorBoard integration
- Attention map visualization

---

# 🧠 Concepts Demonstrated

- Vision Transformers (ViT)
- Self-attention in computer vision
- Image patch embeddings
- Transformer encoder design
- Deep learning model training
- Image classification pipelines

---

# 📜 License

This project is open-source and available under the MIT License.

---

# 👨‍💻 Author

**Aditya Raj Kaushik**
