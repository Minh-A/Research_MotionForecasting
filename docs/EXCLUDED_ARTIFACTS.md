# Excluded Artifacts

This repository is intentionally lightweight. The original `/h0/next` directory
was about 352 GB, mostly due to datasets and processed artifacts.

## Excluded Categories

- Raw datasets
- Processed datasets
- Checkpoints and model weights
- Lightning logs and TensorBoard event files
- RealMotion output runs
- Submission files
- Python caches and compiled bytecode
- Nested Git histories from upstream repositories

## Size Reference

Approximate sizes in the original local folder:

| Path | Size | Reason excluded |
| --- | ---: | --- |
| `/h0/next/Data` | 212 GB | Raw Argoverse 1.1 and Argoverse 2 datasets |
| `/h0/next/ADAPT/predata` | 63 GB | ADAPT preprocessing lists |
| `/h0/next/QCNet/data` | 48 GB | QCNet processed Argoverse 2 data |
| `/h0/next/RealMotion/data` | 28 GB | RealMotion processed data and dataset symlinks |
| `/h0/next/QCNet/lightning_logs` | 445 MB | Training logs and checkpoints |
| `/h0/next/RealMotion/outputs` | 339 MB | Training/evaluation outputs and checkpoints |
| `/h0/next/HPNet/lightning_logs` | 302 MB | Training logs and checkpoints |
| `/h0/next/ADAPT/checkpoints` | 166 MB | Model checkpoints |
| `/h0/next/HiVT/lightning_logs` | 149 MB | Training logs and checkpoints |

## Restore Rule

To rerun experiments, restore datasets and checkpoints outside this GitHub
repository, then recreate the symlinks or root paths described in each
`sources/*/#Util.txt` note.
