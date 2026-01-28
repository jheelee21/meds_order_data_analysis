## Data Quality

- Although there exist entries that are future-dated (as of Jan 24th, 2026), I assume that all entries are valid and should be included in the analysis. This could represent pre-scheduled orders.

- The dataset is assumed to be complete with no missing transactions. All successful and failed orders are captured in the data.

## Business 

- The weight loss injectable pen was first introduced on January 1st, 2025. Any sales prior to this date are not related to this product line and are excluded from the analysis.

- Based on the median inter-order interval of ~30 days observed in the data, I assume the medication supply lasts approximately 30 days, and thus customers are expected to reorder around this interval.

- A customer is considered "churned" if they have not placed an order in the last 45 days (30 days expected reorder interval + 15 days grace period) as of the analysis date.

- A customer is "retained" if they place at least one additional order within 45 days of their initial order. This definition may limit the ability to capture returning customers who reorder after a longer interval, yet it is chosen as the date range of the data collection is only an year.

## Analysis

- The analysis does not account for external factors such as marketing campaigns, seasonality, or competitor actions that may influence customer behaviour.
