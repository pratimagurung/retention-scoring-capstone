# Who Deserves the Next Retention Dollar?
Scoring and targeting customers by repeat-purchase potential

## Question
Which customers should an online retailer prioritize for retention offers, based on repeat-purchase likelihood and customer value?

## Answer
Prioritize **high-value customers with a low predicted chance of repeat purchase** (501 "Retention pilot candidates" at the 10 Sep 2011 snapshot) as the audience for a **randomized offer vs. no-offer pilot**. Protect likely repeaters with non-discount loyalty actions and handle customers dormant over 365 days separately. This is a scoring framework, not proof that an offer causes repeat purchases.

## Data and method
- UCI Online Retail II (Dec 2009 to Dec 2011, £). Place `online_retail_II.xlsx` in `data/`.
- Spending is gross sales, not profit.
- Features: recency, frequency, and spend over 180 days. Outcome: a purchase within 90 days.
- Logistic regression with chronological train (Mar), validation (Jun), and test (10 Sep 2011) snapshots.

## Notebooks (run in order)
1. `01_data_cleaning_rfm`: cleaning and RFM segments
2. `02_repeat_purchase_model`: model, baselines, evaluation
3. `03_customer_targeting_margin`: targeting rules, treatment matrix, scenarios
