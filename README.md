# BanglaTOD---A-tri-lingual-benchmark-for-Bangla-task-oriented-dialogue-understanding

A multi-domain dataset for intent classification and slot filling in Bangla task-oriented dialogue. Every utterance is written in three parallel forms: Bangla (Bengali script), English, and Banglish (Romanized Bangla), to support cross-lingual and code-mixed NLU research.

Paper: https://arxiv.org/abs/2610.18060

## Overview

| Property | Value |
|---|---|
| Total dialogues | 209 |
| Languages | 3 (Bangla, English, Banglish) |
| Domains | 9 |
| Intents | 64 |

## Domain coverage

| Domain | Dialogues | Intents |
|---|---|---|
| Education | 50 | 9 |
| Government Service | 32 | 19 |
| Healthcare | 25 | 5 |
| Mobile Financial Service | 25 | 5 |
| E-commerce | 25 | 10 |
| Restaurant | 16 | 5 |
| Tourist | 14 | 5 |
| Travel | 12 | 4 |
| Hotel | 10 | 2 |
| **Total** | **209** | **64** |

## Data format

Each file is JSON Lines, one dialogue per line:

| Field | Description |
|---|---|
| `dialogue_id` | Unique identifier for the dialogue |
| `domains` | List of domain(s) of the dialogue |
| `intent` | The dominant user goal |
| `turns` | Ordered list of conversational turns |

## Usage

```python
from datasets import load_dataset
ds = load_dataset("afri7here/BanglaTOD", "healthcare")
```

## Citation

```bibtex
@misc{banglatod2026ewu,
      title={A Benchmark for Bangla Task-Oriented Dialogue Understanding},
      author={Afrina Alam Lamia and Sumiaya Sharif and Prottoy Modak and Ohiduzzaman Rayhan and Nafis Sadeq},
      year={2026},
      eprint={2610.18060},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2610.18060},
}
```
