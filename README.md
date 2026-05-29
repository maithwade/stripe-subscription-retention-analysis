# Stripe Subscription Retention Analysis

## Overview
This project analyzes how different pricing tiers affect customer retention 
and lifecycle behavior for a Stripe-style SaaS subscription business. 
The analysis surfaces churn patterns, revenue risk, and actionable retention 
strategies across Starter, Growth, and Enterprise tiers.

## Business Problem
How do different pricing tiers affect customer retention and lifecycle? 
The goal was to understand subscription-level churn patterns and surface 
actionable insights to refine pricing and retention strategy.

## Dataset
- 1,000 synthetic Stripe-style customer records generated in Python
- Time period: January 2023 – June 2024
- Fields: customer_id, tier, MRR, start_date, churn_date, churned, 
  payment_failures, feature_usage_score

## Tools Used
- **Python** (pandas, matplotlib, seaborn) — data generation & visualization
- **SQL** (pandasql) — retention and churn analysis
- **Looker Studio** — interactive dashboard
- **Jupyter Notebook** — analysis environment

## Key Findings
- Starter tier has a 40.5% churn rate — more than 4x Enterprise's 9.5%
- Growth tier represents the largest revenue risk at USD 6,162 MRR at risk
- 93% of churned customers experienced at least one payment failure
- Starter and Growth customers begin churning before day 50 vs Enterprise's 130 days

## Recommendations
- Prioritize Growth tier retention with targeted 60 and 90 day check-ins
- Implement a structured 30-day onboarding program for Starter and Growth
- Build a payment failure intervention system with smart retries and dunning emails

## Dashboard
View the Looker Studio Dashboard here: https://datastudio.google.com/reporting/fedda334-4cca-4700-aa86-afaf4f6077d4

## Project Structure
├── stripe_analysis.ipynb  # Main analysis notebook
├── stripe_subscription.csv  # Dataset
├── Analysis_Memo.pdf  # Full findings and recommendations
└── README.md
