# A/B Test Analysis: Email Campaign Subject Lines

> Statistical A/B test analysis of email campaign performance, comparing a 
> generic promotional subject line against a personalized one using 
> Chi-Squared testing and conversion rate comparison.

---

## Project Overview

E-retail marketing teams constantly test messaging strategies to improve 
campaign performance. This project simulates and analyzes an A/B test 
comparing a generic promotional subject line (Group A) against a 
personalized subject line (Group B).

**Business questions:**
- Does personalization significantly increase open rates?
- Does a higher open rate translate to more conversions?
- Was our sample size sufficient to detect the effect?

**Data source:** simulated data based on realistic e-retail benchmarks

---

## Tech Stack

`Python` · `pandas` · `numpy` · `scipy` · `matplotlib` · `seaborn`

---

## Methodology

| Step | Description |
|------|-------------|
| Data simulation | Binomial distribution, realistic e-retail benchmarks |
| Statistical test | Chi-Squared test |
| Significance level | α = 0.05 |
| Power analysis | Cohen's h, 80% power threshold |
| Confidence intervals | 95% CI for open rate & conversion rate |

---

## Key Results

<img width="989" height="495" alt="image" src="https://github.com/user-attachments/assets/acce96fc-8222-4620-b9bc-de249d776a39" />

| Metric | Group A | Group B | Lift |
|--------|---------|---------|------|
| Open Rate | 21.9% | 26.3% | +20.2% |
| Conversion Rate | 0.76% | 1.48% | +94.7% |
| Statistical significance | ✓ | ✓ | p < 0.05 |

---

## Key Findings & Recommendation

- Personalized subject lines significantly increase both open and conversion rates
- Recommendation: roll out personalised subject lines to the full send list
- At 10,000 users per campaign, this yields an estimated +72 additional 
  conversions per send at no additional cost

---

## Limitations

Data is simulated based on realistic industry benchmarks. In a real setting, 
results should be validated over multiple campaigns and across different 
customer segments before full rollout.

---

## Repository Structure

```
ab-test-email-campaign/
├── ab_test_email_campaign.ipynb   # Full analysis notebook
└── README.md
```

---

## Setup & Usage

### Prerequisites
```
pip install pandas numpy scipy matplotlib seaborn
```

### Running the Notebook
1. Clone this repository
2. Open and run `ab_test_email_campaign.ipynb` in Jupyter
