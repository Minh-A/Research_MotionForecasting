# Datasets

The original `/h0/next` folder contained real trajectory prediction datasets.
They are documented here but not committed to GitHub.

## Argoverse Motion Forecasting v1.1

Local path:

```text
/h0/next/Data/Argoverse1.1
```

Used by:

- `sources/hivt`
- `sources/adapt`
- `sources/hpnet/HPNet-Argoverse`

Observed local structure:

```text
Data/Argoverse1.1/
├── forecasting_train_v1.1.tar.gz
├── forecasting_val_v1.1.tar.gz
├── forecasting_test_v1.1.tar.gz
├── argoverse-api/
├── train/
│   ├── data/*.csv
│   ├── processed/*.pt
│   └── processed_data/
├── val/
│   ├── data/*.csv
│   ├── processed/*.pt
│   └── processed_data/
└── test/
    ├── data/*.csv
    └── processed_data/
```

Observed file counts:

- `train/data`: 205,942 CSV files
- `val/data`: 39,472 CSV files
- `test/data`: 78,143 CSV files
- `train/processed`: 205,944 `.pt` files
- `val/processed`: 39,474 `.pt` files

Approximate local size: 96 GB.

## Argoverse 2 Motion Forecasting

Local path:

```text
/h0/next/Data/Argoverse2
```

Used by:

- `sources/qcnet`
- `sources/realmotion`

Observed local structure:

```text
Data/Argoverse2/
├── train.tar
├── val.tar
├── test.tar
├── train/<scenario_id>/*.parquet, *.json
├── val/<scenario_id>/*.parquet, *.json
└── test/<scenario_id>/*.parquet, *.json
```

Observed file counts:

- `train`: 399,816 files
- `val`: 49,976 files
- `test`: 49,968 files

Approximate local size: 117 GB.

## Processed Data

These processed datasets were present locally and excluded from GitHub:

```text
ADAPT/predata/
├── eval.ex_list
├── ex_list
└── extended_ex_list

QCNet/data/
├── train/processed/*.pkl
├── val/processed/*.pkl
└── test/processed/*.pkl

RealMotion/data/realmotion_processed/
├── train/*.pt
├── val/*.pt
└── test/*.pt
```

Approximate local sizes:

- `ADAPT/predata`: 63 GB
- `QCNet/data/train/processed`: 38 GB
- `QCNet/data/val/processed`: 4.8 GB
- `QCNet/data/test/processed`: 4.8 GB
- `RealMotion/data/realmotion_processed/train`: 23 GB
- `RealMotion/data/realmotion_processed/val`: 2.9 GB
- `RealMotion/data/realmotion_processed/test`: 2.2 GB

## INTERACTION Dataset

HPNet supports the INTERACTION dataset in its upstream project. No local
INTERACTION dataset copy was found under `/h0/next` during this cleanup.
