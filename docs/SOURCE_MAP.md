# Source Map

This document maps the curated archive back to `/h0/next`.

| Archive path | Original local path | Upstream remote | Local clone / first evidence | Notes |
| --- | --- | --- | --- | --- |
| `sources/realmotion` | `/h0/next/RealMotion` | `https://github.com/fudan-zvg/RealMotion.git` | 2025-05-09 | Argoverse 2 continuous motion forecasting |
| `sources/qcnet` | `/h0/next/QCNet` | `https://github.com/ZikangZhou/QCNet.git` | 2025-05-13 | Argoverse 2 baseline and processed data pipeline |
| `sources/hivt` | `/h0/next/HiVT` | `https://github.com/ZikangZhou/HiVT.git` | 2025-05-15 | Argoverse 1.1 baseline |
| `sources/adapt` | `/h0/next/ADAPT` | `https://github.com/gorkaydemir/ADAPT.git` | 2025-05-19 | Argoverse 1.1 preprocessing and training |
| `sources/hpnet` | `/h0/next/HPNet` | `https://github.com/XiaolongTang23/HPNet.git` | 2025-05-20 | Argoverse and INTERACTION-capable baseline |

## Local Command Notes

The original folder had per-project `#Util.txt` notes with commands for dataset
symlinks, conda environments, preprocessing, training, validation, and testing.
Those notes are preserved inside each `sources/*` folder because they document
how the local experiments were run.

## Excluded Local Paths

The following original paths were intentionally not copied:

- `/h0/next/Data`
- `/h0/next/ADAPT/predata`
- `/h0/next/ADAPT/checkpoints`
- `/h0/next/HPNet/lightning_logs`
- `/h0/next/HPNet/test_output`
- `/h0/next/HPNet/visualization`
- `/h0/next/HiVT/lightning_logs`
- `/h0/next/QCNet/data`
- `/h0/next/QCNet/lightning_logs`
- `/h0/next/RealMotion/data`
- `/h0/next/RealMotion/outputs`
- `/h0/next/RealMotion/submission`
