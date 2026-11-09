# Credit Card Fraud Detection

All of the project's work is in [fraud_detection.ipynb](fraud_detection.ipynb).

## Setup

Run these from the repo root. The pinned packages were tested on Python 3.14.

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -m notebook fraud_detection.ipynb
```

If you use VS Code instead, choose the `.venv` kernel. The notebook downloads the dataset into `data/raw/` the first time it runs.

## Rules

- Use `dev`, `test_a`, `test_b` and `folds` from Part 1, so everyone has identical splits.
- Never resample validation or test data.
- Keep each card on one side of every split.
- `cc_num` is only the grouping key for splits. Never use it as a model input.
