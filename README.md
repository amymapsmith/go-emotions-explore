# GoEmotions Exploration

Interview-prep workspace for exploring human-labeled GoEmotions annotations.

## Data

The notebook downloads the full GoEmotions CSV shards from Google Research:

- `goemotions_1.csv`
- `goemotions_2.csv`
- `goemotions_3.csv`

It also includes setup for cloning the `google-research/bert` repository. As of this setup run, the historical Google Cloud Storage BERT zip URLs linked from the archived repository returned `AccessDenied`, so the repo includes instructions for using Hugging Face's `google-bert/bert-base-uncased` files as a practical fallback.

## Quick Start

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

Open `notebooks/go_emotions_explore.ipynb`.

## Current Local Assets

- GoEmotions CSV shards are downloaded under `data/full_dataset/`.
- `google-research/bert` is cloned under `models/bert/google-research-bert/`.
- The original BERT zip URL was not available anonymously during setup.
