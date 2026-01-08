# Headline-Engagement-Analysis
Analyzed millions of randomized Upworthy headline A/B tests (2013–2015) to identify textual drivers of click-through rate. Evaluated numbers, questions, length, sentiment, and replication validity using z-tests and chi-square tests. Demonstrates rigorous experimentation and exploratory vs confirmatory analysis.

# Headline Engagement Analysis  
**Validating Content Strategies with Large-Scale A/B Testing**

## Overview
This project analyzes large-scale randomized A/B experiments conducted by **Upworthy** to identify which headline characteristics drive higher engagement, measured via click-through rate (CTR). The analysis emphasizes statistical rigor, experimental design, and replication rather than surface-level metrics.

The experiments span **2013–2015** and include millions of impressions across exploratory, confirmatory, holdout, and undeployed tests.

---

## Business Objective
The editorial and growth teams aim to answer:

> Which headline features reliably increase engagement, and do exploratory findings hold up under confirmatory testing?

---

## Datasets Used
Four curated datasets from the Upworthy Research Archive:

- **Exploratory experiments** – hypothesis generation  
- **Confirmatory experiments** – hypothesis validation  
- **Holdout data** – robustness and sanity checks  
- **Undeployed experiments** – non-production tests  

Each dataset includes the following key fields:
- `headline` – text of the tested headline  
- `impressions` – number of times shown  
- `clicks` – number of clicks received  
- `eyecatcher_id` – image identifier  
- `clickability_test_id` – experiment ID  

---

## Research Questions
1. Do headlines containing numbers perform better than those without?
2. Does framing a headline as a question increase engagement?
3. Are shorter headlines more effective than longer ones?
4. Do emotionally charged headlines perform differently from neutral ones?
5. When the same image is used, do textual differences alone drive engagement?
6. Do exploratory findings replicate in confirmatory experiments?

---

## Methodology
- Computed **click-through rate (CTR)** from impressions and clicks  
- Applied **two-proportion z-tests** to compare headline variants  
- Used **chi-square tests** for categorical comparisons  
- Performed **sentiment analysis** with TextBlob  
- Conducted **exploratory vs confirmatory**

