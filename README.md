# ⚽ FIFA World Cup: Men's vs. Women's Goal Scoring Analysis

This repository contains an end-to-end statistical hypothesis testing pipeline analyzing official FIFA World Cup matches held after **January 1, 2002**. 

The goal is to answer a single core question: **Are more goals scored in women's international soccer matches than in men's matches?**

---

## 🎯 Research Hypotheses & Methodology

* **Null Hypothesis ($H_0$):** The mean distribution of goals scored in official Women's FIFA World Cup matches is the **same** as in Men's matches.
* **Alternative Hypothesis ($H_1$):** The mean distribution of goals scored in official Women's FIFA World Cup matches is **greater** than in Men's matches.
* **Significance Level ($\alpha$):** `0.10` (10%)
* **Statistical Test:** One-tailed Mann-Whitney U Test (Wilcoxon Rank-Sum Test).

> **Why Non-Parametric?** Goal distributions in soccer are discrete and heavily right-skewed, violating the normality assumption required for a two-sample Student's t-test.

---

## 📁 Repository Structure

```text
├── data/
│   ├── men_results.csv        # Historical men's match data
│   └── women_results.csv      # Historical women's match data
├── main.py                    # Main hypothesis testing pipeline
├── requirements.txt           # Required Python packages
└── README.md                  # Project overview and reproduction steps
# -gender-soccer-goals-hypothesis-testing
Statistical hypothesis testing to determine if more goals are scored in official FIFA World Cup women's soccer matches than men's using non-parametric inference (Mann-Whitney U Test).  
