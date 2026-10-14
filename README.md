## Dataset

We use the **Garbage Detection** dataset (6 classes: BIODEGRADABLE, CARDBOARD,
GLASS, METAL, PAPER, PLASTIC) from Kaggle:
- Original dataset: https://www.kaggle.com/datasets/viswaprakash1990/garbage-detection
- Our re-split assignment: uploaded in the data folder

The original validation and test images were pooled and re-split into
validation (1,571 images) and test (1,569 images); the training set is unchanged.
The split is defined in `data/resplit_assignment.csv`.

To download (requires a Kaggle account):
​```python
import kagglehub
kagglehub.login()
ds = kagglehub.dataset_download("viswaprakash1990/garbage-detection")
rs = download it from data folder
​```
The evaluation notebook rebuilds the re-split automatically.
