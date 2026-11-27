# Tableau Dashboards

I created four Tableau dashboards for my capstone project, *Who Deserves the Next Retention Dollar?* The dashboards show what I learned about the retailer's customers, how well the repeat-purchase model worked, and how the results could help plan a retention campaign.

The analysis uses the Online Retail II dataset, with a customer snapshot taken on September 10, 2011.

## Dashboard 1: Customer Overview

This dashboard gives an overview of the 5,281 customers and their RFM segments. It shows the number of customers in each segment, their total historical gross spending, and their average spending per customer.

## Dashboard 2: Repeat-Purchase Prediction

This dashboard compares the logistic regression model with simpler models. It also shows how often customers in each prediction decile purchased again within 90 days. The model achieved a ROC AUC of 0.775, but it generally predicted lower repeat-purchase rates than what was observed.

## Dashboard 3: Retention Decision

This dashboard compares five targeting strategies, each selecting 529 customers. I used historical spending and non-repeat risk to understand the trade-offs between selecting valuable customers and selecting customers who may not purchase again.

## Dashboard 4: Retention Pilot and Financial Scenarios

This dashboard compares the projected margins for the proposed pilot audience and a random group of eligible customers. The results change depending on whether predicted or historically observed repeat rates are used. Because of this, I recommend testing the proposed audience in a controlled pilot before spending the full retention budget.

## View the Dashboards

- Tableau Public:(https://public.tableau.com/app/profile/pratima.gurung3511/viz/Retention_Scoring_Capstone/01-CustomerOverview)
- Screenshots are available in the `screenshots/` folder.

## Notes

Historical spending is based on purchases before returns are deducted. The financial scenarios are estimates, and a controlled pilot is needed to find out whether the retention offer actually increases profit.
