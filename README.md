# Airbnb DC Pricing & Revenue Optimization

## Overview
This project performs an end-to-end pricing and revenue optimization analysis of Airbnb listings in Washington, DC using Inside Airbnb data (March 13, 2025 archived snapshot).

The analysis combines demand modeling, price elasticity estimation, and LLM-assisted revenue simulation to identify pricing strategies that increase expected revenue while maintaining booking probability.

## Data
- Listings data (property & hsot attributes)
- Calendar data (daily prices & availability)
- Reviews data (guest feedback)

Source: Inside Airbnb (public data)

## Methodology
- CRIS-DM framework
- Time-based train/validation/test splits
- Lasso-regularized regression models:
  - Linear (stay length)
  - Exponential (stay length)
  - Constant Price Elasticity (stay length)
  - Logistic (booking probability)
- Neighborhood-level elasticity estimation
- LLM-assisted revenue optimization simulation

## Key Findings
- Demand across all DC neighborhoodsis **inelastic)
- Logistic model achieved strong predictive performance (AUC ~0.84)
- A simulated 5% price increase produced:
  - $5.07M increase in expected revenue
  - ~4.62% overall revenue lift
  - Positive gains in every neighborhood

## Repository Structure
  reports/-> Final report

  slides/-> Final presentation slides

  notebooks/-> Analysis notebooks (Python; run order prefixed)

  data/-> Inside Airbnb datasets (raw, compressed)
