# ♻️ Waste to Value
### Garbage Detection · Organic Waste Identification

Identify waste objects in images across six categories, with a focus on **biodegradable waste**.

---

## 📦 Dataset

This project uses the **Garbage Detection** dataset from Kaggle, with bounding box annotations for six waste categories:

| Class | Waste category |
|---|---|
| 🌱 BIODEGRADABLE | Organic waste |
| 📦 CARDBOARD | Cardboard |
| 🫙 GLASS | Glass |
| 🔩 METAL | Metal |
| 📄 PAPER | Paper |
| 🧴 PLASTIC | Plastic |

🔗 **[View the original dataset on Kaggle](https://www.kaggle.com/datasets/viswaprakash1990/garbage-detection)**

## 🔀 Dataset Split

The original validation and test images were pooled and redistributed into two evaluation sets. The training set was retained unchanged.

| Split | Images |
|---|---:|
| Training | 7,324 |
| Validation | 1,571 |
| Test | 1,569 |

> **Shared evaluation:** All models use the same split assignment for consistent comparison.

The split assignment is available in [`data/resplit_assignment.csv`](data/resplit_assignment.csv).

## 🚀 Download the Dataset

Install the download package:

```bash
pip install kagglehub
```

Download the original dataset:

```python
import kagglehub

kagglehub.login()

dataset_path = kagglehub.dataset_download(
    "viswaprakash1990/garbage-detection"
)

print("Dataset downloaded to:", dataset_path)
```

## 🛠️ Reproduce the Evaluation Split

1. Download the original dataset.
2. Use the shared assignment file in the `data/` folder.
3. Run the evaluation notebook to reconstruct the validation and test splits automatically.
