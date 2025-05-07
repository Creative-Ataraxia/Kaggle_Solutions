# My Kaggle Solutions

Here are my end-to-end solutions for selected **Kaggle featured competitions**. Codes in the notebook are carefully documented to show the thought process used in problem solving.

---

## Table of Contents

1. [LLMs – You Can't Please Them All (Silver Medal)](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/LLM_solution.ipynb)
2. [Santa 2024 – The Perplexity Permutation Puzzle (Bronze Medal)](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/santa2024_solution.ipynb)
3. [Jane Street Real-Time Market Forecasting (Bronze Range)](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/jane_street_solution.ipynb)
4. [House Prices – Advanced Regression Techniques](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/housing_price_solution.ipynb)

---

## 1. [LLMs – You Can't Please Them All 🥈](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/LLM_solution.ipynb)

**Goal:** Fool multiple LLM judges by generating adversarial essays tailored to their scoring metrics.
**Result:** Silver medal won.

### Data Handling
- Constructed synthetic essays from curated corpora (Brown, stopwords, negative wordlists).
- Controlled essay length to manipulate scoring metrics.
- Dynamically injected test topics with targeted attacks.

### Modeling & Strategy
- Reverse-engineered LLM judge behavior (Gemma, Llama, Qwen, Phi).
- Multi-language prompt attacks with model-specific token tailoring.
- Local verification code modules to approximate output matching expected LB scoring.

### Ensembling & Scoring
- Combined multi-attack strategies for specific score matrices (e.g. 099, 909, 990).
- Partitioned test indices for optimal LB positioning.
- Batched and validated generated essays for grading consistency.

### Unique Techniques
- LLM similarity metrics manipulation.
- Chat template engineering + token-length partitioning.
- A local eval pipeline to verify targeted LLM judge outcomes.

---

## 2. [Santa 2024 – The Perplexity Permutation Puzzle 🥉](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/santa2024_solution.ipynb)

**Goal:** Reorder holiday words to minimize perplexity and maximize LLM satisfaction.
**Result:** Bronze medal won.

### Big Data Handling
- Strategically partitioned stopwords, verbs, and content words for parallel processing.
- Prioritized words that maximize valid sequence length and syntactic coherence.

### Modeling & Optimization
- Built an Iterated Local Search framework with:
  - Beam search, insert optimization, shuffle/swap/move.
  - Custom simulated annealing and genetic algorithm approaches.
  - Restricted k-opt with heuristic-based move limits.

### Ensembling & Exploration
- Multi-start optimization with solution de-duplication.
- Weighted probabilistic insertions and operation scoring.

### Unique Techniques
- Alphabet-based inserts, variable-length permutations.
- Fixed-position testing (e.g. forcing a specific final word).
- Perplexity-weighted operation selection and cyclic SA cooling.

---

## 3. [Jane Street Real-Time Market Forecasting ](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/jane_street_solution.ipynb)

**Goal:** Forecast market signals using real-time structured features in a live leaderboard setup.

###  Focus Areas
- Strong emphasis on data preprocessing, feature leakage prevention, and volatility-aware modeling.
- Gated recurrent unit (GRU) and Long Short-Term Memory (LSTM) models tailored for financial time series with noise handling and feature normalization.

---

## 4. [House Prices – Advanced Regression Techniques ](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/housing_price_solution.ipynb)

**Goal:** Predict house prices using custom feature-engineered data and regression pipelines.
**Result:** Top 5 finish on public leaderboard.

###  Purpose
- Demonstrates full ML pipeline workflow: feature engineering → model selection → metrics tuning.

---

## 🧠 Core Skills Used

| Category              | Description                                              |
|-----------------------|----------------------------------------------------------|
| Data Handling         | Text preprocessing, synthetic generation, feature logic  |
| System Thinking       | Modular, testable pipelines for essay scoring and search |
| Algorithm Design      | Custom ILS, SA, and ensemble search strategies           |
| Model Engineering     | Prompt engineering, language targeting, evaluation loops |
| Code Quality          | Clean, explainable notebooks for replication and review  |

---

## 📬 Contact

[LinkedIn](https://www.linkedin.com/in/royma/)
[Kaggle](https://www.kaggle.com/alexmason11)
