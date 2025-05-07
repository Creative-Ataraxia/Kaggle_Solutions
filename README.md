# 🧠 My Kaggle Solutions

This repository showcases my end-to-end solutions for selected **Kaggle featured competitions**, highlighting my skills in **data handling**, **algorithm design**, **systemic thinking**, and **solution optimization**. Each notebook is fully documented to demonstrate **problem-solving rigor** and **engineering maturity**—intended for both peer learners and potential recruiters.

---

## 🧩 Table of Contents

1. [LLMs – You Can't Please Them All (Silver Medal)](#1-llms--you-cant-please-them-all)
2. [Santa 2024 – The Perplexity Permutation Puzzle (Bronze Medal)](#2-santa-2024--the-perplexity-permutation-puzzle)
3. [Jane Street Real-Time Market Forecasting (Bronze Range)](#3-jane-street-real-time-market-forecasting)
4. [House Prices – Advanced Regression Techniques (Top 5%)](#4-house-prices--advanced-regression-techniques)

---

## 1. [LLMs – You Can't Please Them All 🥈](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/LLM_solution.ipynb)

**Goal:** Fool multiple LLM judges by generating adversarial essays tailored to their scoring quirks.

### 🧰 Data Handling
- Constructed synthetic essays from curated corpora (Brown, stopwords, negative wordlists).
- Controlled essay length to manipulate scoring metrics.
- Dynamically injected test topics with targeted attacks.

### 🧠 Modeling & Strategy
- Reverse-engineered LLM judge behavior (Gemma, Llama, Qwen).
- Multi-language prompt attacks (EN/JP/CH/KR) with model-specific token tailoring.
- Local verification systems to ensure output matched expected scoring.

### 🧪 Ensembling & Scoring
- Combined multi-attack strategies for specific score vectors (e.g. 099, 909, 990).
- Partitioned test indices for optimal leaderboard positioning.
- Batched and validated generated essays for grading consistency.

### 🧵 Unique Techniques
- Whitespace injection for `avg_s` manipulation.
- Chat template engineering + token-length clipping.
- A scoring pipeline to verify whether each essay matched targeted judge outcomes.

---

## 2. [Santa 2024 – The Perplexity Permutation Puzzle 🎄🥉](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/santa2024_solution.ipynb)

**Goal:** Reorder holiday words to minimize perplexity and maximize LLM satisfaction.

### 🧰 Data Handling
- Strategically separated stopwords, verbs, and content words.
- Prioritized words that maximize valid sequence length and syntactic coherence.

### 🧠 Modeling & Optimization
- Built an Iterated Local Search (ILS) framework with:
  - Beam search, insert optimization, shuffle/swap/move
  - Custom simulated annealing
  - Restricted k-opt with heuristic-based move limits

### 🧪 Ensembling & Exploration
- Multi-start optimization with solution deduplication.
- Weighted probabilistic insertions and operation scoring.

### 🧵 Unique Techniques
- Alphabet-based inserts, variable-length permutations.
- Fixed-position testing (e.g. forcing a specific final word).
- Perplexity-weighted operation selection and cyclic SA cooling.

---

## 3. [Jane Street Real-Time Market Forecasting 📉](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/jane_street_solution.ipynb)

**Goal:** Forecast market signals using real-time structured features in a live leaderboard setup.

### 📊 Status
- Final leaderboard still pending due to delayed real-world data validation.
- Current placement in **bronze medal range**.

### 🧠 Focus Areas
- Strong emphasis on data preprocessing, feature leakage prevention, and volatility-aware modeling.
- Techniques tailored for financial time series with noise handling and feature normalization.

---

## 4. [House Prices – Advanced Regression Techniques 🏠](https://github.com/Creative-Ataraxia/Kaggle_Solutions/blob/main/housing_price_solution.ipynb)

**Goal:** Predict house prices using structured data and regression pipelines.

### 📊 Result
- Top 5% finish on public leaderboard.

### 🔍 Purpose
- Demonstrates full ML pipeline: feature engineering → model selection → tuning.
- Used as a clean "starter project" for recruiters and learners alike.

---

## 🧠 Core Skills Demonstrated

| Category              | Description                                              |
|-----------------------|----------------------------------------------------------|
| Data Handling         | Text preprocessing, synthetic generation, feature logic |
| System Thinking       | Modular, testable pipelines for essay scoring and search |
| Algorithm Design      | Custom ILS, SA, and ensemble search strategies           |
| Model Engineering     | Prompt engineering, language targeting, evaluation loops |
| Code Quality          | Clean, explainable notebooks for replication and review  |

---

## 📬 Contact

If you're a recruiter or fellow ML engineer and would like to connect, feel free to reach out via GitHub or [LinkedIn](https://www.linkedin.com/in/your-profile).

---

Thanks for reading! 🎯
