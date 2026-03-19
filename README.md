# sycophantic-ai-illusion-of-learning

# Sycophantic AI Generates an Illusion of Learning

Data and code from manuscript: Duettmann, A. & Sharot, T. (in prep.). Sycophantic AI generates an illusion of learning.

---

## Overview

Two quantitative experiments examined how AI sycophancy influences subjective and objective aspects of human learning. Experiment 1 used a between-subjects experimental design in which participants interacted with either  sycophantic or non-sycophantic AI responses. Experiment 2 used a correlational design in which participants interacted with AI responses with natural variation in perceived AI sycophancy measured via participants’ ratings and related to learning outcomes. Control groups for each experiment completed the studies without AI interaction.

---

## Repository Structure

```
sycophantic-ai-illusion-of-learning/
│
├── data/
│   ├── data_experiment_1_causal_Main_vf.csv           # Exp. 1 main dataset (N = 213; sycophantic vs. non-sycophantic AI)
│   ├── data_experiment_1_causal_wControl_vf.csv        # Exp. 1 extended dataset including no-feedback control group (N = 102)
│   ├── data_experiment_2_correlational_Main_vf.csv     # Exp. 2 main dataset (N = 288; philosophy & art history combined)
│   └── data_experiment_2_correlational_wControl_vf.csv # Exp. 2 extended dataset including no-feedback control group (N = 201)
│
├── sycophancy_exp1_clean.R   # All analyses and figures for Experiment 1
├── sycophancy_exp2_clean.R   # All analyses and figures for Experiment 2
└── README.md
```

---

## Key Variables

| Variable in data | Label in paper |
|---|---|
| `condition` (positive/negative) | Sycophantic / Non-sycophantic AI |
| `accuracy_pre` | Initial exam performance |
| `accuracy_post` | Transfer exam performance |
| `happy_pre/post` | Baseline / post-interaction mood |
| `perceived_comp_pre/post` | Baseline / post-interaction perceived competence |
| `desire_learn_phil` | Desire to learn (Philosophy) — Exp. 1 |
| `desire_learn_arthistory` | Desire to learn (Art History) — Exp. 1 |
| `desire_learn` | Desire to learn — Exp. 2 |
| `sycophancy_score` | PC1 from PCA on five tone ratings — Exp. 2 |
| `domain` | Topic learned: `art` / `phil` — Exp. 2 |

---

## Requirements

R (≥ 4.3.1) with the following packages:

`tidyverse`, `readr`, `lme4`, `lmerTest`, `psych`, `ppcor`, `rsq`, `ggtext`, `BayesFactor`, `mediation`, `broom`, `gt`, `conflicted`

