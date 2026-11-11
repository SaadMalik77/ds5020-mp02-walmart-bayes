# Data

Put `Walmart.csv` in this folder. The notebook expects `data/Walmart.csv`.

**Option 1: browser.** Download from https://www.kaggle.com/datasets/yasserh/walmart-dataset,
unzip, and move `Walmart.csv` here.

**Option 2: Kaggle CLI** (needs an API token in `~/.kaggle/kaggle.json`; never put that file in the repo):

```bash
pip install kaggle
kaggle datasets download yasserh/walmart-dataset -p data --unzip
```

Expected: 6,435 rows, 8 columns, no missing values. The notebook's P1 cell checks this.

The CSV is ignored by git (see `.gitignore`), so each teammate downloads it once.
