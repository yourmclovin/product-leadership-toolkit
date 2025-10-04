# SU-RICE Prioritization Framework

> **SaaS-focused prioritization framework**

## 📥 Download

**Excel Template:** [Download XLSX](https://res.cloudinary.com/dimqqmfx6/raw/upload/v1759549640/su-rice-prioritization_wok31z.xlsx)

---

## Overview

An enhanced version of the RICE framework, specifically designed for SaaS products. Adds **Satisfaction** and **Urgency** to the traditional RICE model.

## Formula

```
SU-RICE Score = (Satisfaction × Urgency × Reach × Impact × Confidence) / Effort
```

---

## Scoring Components

### 1. Satisfaction (S)
**Question:** How much will this improve user satisfaction?

- **5** - Massive positive impact
- **4** - Significant improvement
- **3** - Moderate improvement
- **2** - Slight improvement
- **1** - Minimal or no impact

### 2. Urgency (U)
**Question:** How time-sensitive is this?

- **5** - Critical/Immediate (this quarter)
- **4** - High urgency (next quarter)
- **3** - Moderate urgency (this year)
- **2** - Low urgency (next year)
- **1** - No urgency (nice to have)

### 3. Reach (R)
**Question:** How many users will this affect per time period?

- Enter the **number of users** affected per quarter
- Example: 10,000 users/quarter = 10,000

### 4. Impact (I)
**Question:** How much will this impact each user?

- **3** - Massive impact
- **2** - High impact
- **1** - Medium impact
- **0.5** - Low impact
- **0.25** - Minimal impact

### 5. Confidence (C)
**Question:** How confident are you in your estimates?

- **100%** - High confidence (backed by data)
- **80%** - Medium confidence (some data)
- **50%** - Low confidence (mostly assumptions)

### 6. Effort (E)
**Question:** How much work is required?

- Enter **person-months** of work
- Example: 2 engineers × 3 months = 6 person-months

---

## Example Calculation

**Feature:** AI-powered search
- Satisfaction: 4
- Urgency: 4
- Reach: 5,000 users/quarter
- Impact: 2
- Confidence: 80%
- Effort: 3 person-months

```
SU-RICE Score = (4 × 4 × 5,000 × 2 × 0.8) / 3
              = 128,000 / 3
              = 42,667
```

---

## How to Use

### Step 1: List Features
Create a row for each feature or initiative

### Step 2: Score Each Component
Rate each feature across all 6 dimensions

### Step 3: Calculate SU-RICE Score
The template automatically calculates the score

### Step 4: Sort by Score
Higher scores = higher priority

### Step 5: Review & Adjust
Use scores as input, not absolute truth

---

## When to Use SU-RICE vs Other Frameworks

### Use SU-RICE when:
- ✅ Working on SaaS products
- ✅ Need to balance user satisfaction with business urgency
- ✅ Have quantitative data on reach
- ✅ Want objective, data-driven prioritization

### Use Product Hypothesis Scoring when:
- ✅ Evaluating early-stage ideas
- ✅ Need broader strategic assessment
- ✅ Less quantitative data available

---

## 📚 Related Resources

- [Product Hypothesis Scoring](./product-hypothesis-scoring.xlsx)
- [Decision Matrix Template](./decision-matrix-template.xlsx)
- [Product Roadmap Strategy](../01-product-strategy/)

---

*Part of the [Product Leadership Toolkit](https://github.com/yourmclovin/product-leadership-toolkit) by Owen McLoughlin*