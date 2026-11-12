# Fashion-MNIST Image Classification

This project compares two machine-learning approaches for classifying Fashion-MNIST clothing images into 10 categories:

- A K-Nearest Neighbors (KNN) classifier implemented from scratch with NumPy.
- A scikit-learn Random Forest classifier.

The notebook normalizes pixel values, evaluates both models with accuracy, macro-precision, macro-recall, and macro F1-score, and visualizes their performance.

## Project highlights

- Implemented batch-optimized KNN prediction using vectorized Euclidean-distance calculations, nearest-neighbor selection, and majority voting.
- Compared KNN with a 100-tree Random Forest using multiple classification metrics and a grouped performance chart.

## Repository structure

```text
.
├── data/
│   ├── fashion-mnist_train.csv
│   └── fashion-mnist_test.csv
├── notebooks/
│   └── fashion-mnist.ipynb
├── requirements.txt
└── .gitignore
```

## Setup

Python 3.10+ is recommended.

```bash
git clone <your-repository-url>
cd ML-Fashion-MNIST

python3 -m venv .venv
source .venv/bin/activate       # macOS/Linux
# .venv\Scripts\activate      # Windows PowerShell

python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m notebook
```

Open `notebooks/fashion-mnist.ipynb` and run the cells from top to bottom. The notebook expects the included CSV files to remain in the `data/` directory.

## Dataset

The project uses the Fashion-MNIST dataset in CSV format. The labels are integer class IDs mapped in the notebook to:

`T-shirt/top`, `Trouser`, `Pullover`, `Dress`, `Coat`, `Sandal`, `Shirt`, `Sneaker`, `Bag`, and `Ankle boot`.

## Results

The notebook prints full classification reports and a metric comparison for both models. Results can vary slightly with library versions and configuration; run the notebook to regenerate the current metrics and chart.
