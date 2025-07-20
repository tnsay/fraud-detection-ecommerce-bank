# fraud-detection-ecommerce-bank
Improved detection of fraud cases for e-commerce and bank transactions
## EDA 

This repository contains the EDA for a fraud detection project using two transaction datasets (`Fraud_Data.csv`, `creditcard.csv`) and one IP geolocation dataset (`IpAddress_to_Country.csv`).

## Summary

- **No missing values** were found across all datasets.
- Cleaned and preprocessed the `signup_time`, `purchase_time`, and IP fields.
- Engineered features like:
  - `time_since_signup`: Time difference between user sign-up and transaction.
  - `country`: Mapped from IP address using IP range matching.

## Key Insights

- The dataset has a **strong class imbalance**:  
  - **< 20,000** fraudulent transactions  
  - **> 120,000** legitimate transactions
- Fraudulent purchase values mostly fall between **85 and 120**, while legitimate purchases have a broader range.
- Source and browser types show different patterns across fraud classes.

## Requirements

To run the EDA, install the following packages:

```bash
pip install pandas numpy matplotlib seaborn ipython

