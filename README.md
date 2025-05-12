# Toximatics Towards Understanding Toxicity in Real-Life Social Situations

## Overview

Toximatics is a dataset and framework introduced to better understand how context shapes perceived toxicity in real-life and social conversations. Unlike traditional hate speech detection datasets, which operate on isolated sentences or keyword triggers, Toximatics provides utterance-context pairs with crowd-annotated toxicity scores. This allows researchers to explore pragmatic and perlocutionary dimensions of toxic language in nuanced settings.

## Methodology

Contextual Grounding: Contexts are not just thread replies, but full situational descriptors.

Augmentation Methods:

Direct Augment: Adds context to existing utterances.

Multistage Augment: Creates new utterance-context pairs through iterative generation.

N-iter Multistage: Further recursive extensions for counterfactual diversity.

Seed Utterances: From implicit hate datasets (e.g., ToxiGen) and socially neutral conversational topics.

Prompt Engineering: Custom-tailored prompts with in-context examples and polarity control.

## Benchmark Results (F1 Score)

| Model            | F1 Score |
| ---------------- | -------- |
| ChatGPT-4        | 0.67     |
| LLaMA-2-13B-Chat | **0.73** |
| T5-XXL           | 0.62     |
| RoBERTa (Jigsaw) | 0.07     |
| HateBERT (RAL-E) | 0.31     |



### Citation
Please use the following to cite this work:
```
@inproceedings{das2024toximatics,
  title={Toximatics: Towards Understanding Toxicity in Real-Life Social Situations},
  author={Mayukh Das and Wolf-Tilo Balke},
  booktitle={Proceedings of the 25th Annual Meeting of the Special Interest Group on Discourse and Dialogue (SIGDIAL)},
  year={2024},
  pages={770--785}
}
```

