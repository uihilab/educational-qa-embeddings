## 🧠 Educational Semantic Pair Dataset

This repository provides a synthetically curated dataset of sentence pairs designed for training and evaluating embedding models in the educational domain. It includes both semantically similar (positive) and dissimilar (negative) sentence pairs, tailored for applications such as academic question answering, semantic retrieval, and educational chatbot development.
## 📦 Dataset Contents

The dataset is split into two files:

    positive_pairs.jsonl — Semantically similar pairs (label = 1)

    negative_pairs.jsonl — Semantically dissimilar pairs (label = 0)

## 🔍 Use Cases

This dataset can be used for fine-tuning embedding models for:

    Syllabus-based QA systems

    Retrieval-Augmented Generation (RAG) pipelines

    Educational chatbots

    LMS-integrated question answering tools

Supported training strategies include:

    Contrastive learning (e.g., MultipleNegativesRankingLoss)

    Supervised similarity alignment (e.g., CosineSimilarityLoss)

## 📊 Statistics

| Type     | # of Pairs |
| -------- | ---------- |
| Positive | 2,710      |
| Negative | 487        |


## 📁 File Descriptions
| File                   | Description                                     |
| ---------------------- | ----------------------------------------------- |
| `positive_pairs.jsonl` | Synonymous or paraphrased educational terms     |
| `negative_pairs.jsonl` | Structurally similar but semantically unrelated |

## 🔧 How to Use

Each `.jsonl` file contains line-separated JSON entries with the following schema:

- `sentence1`: First sentence in the pair
- `sentence2`: Second sentence in the pair
- `label`: 1 for semantically similar (positive), 0 for dissimilar (negative)
