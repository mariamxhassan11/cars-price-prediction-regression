# Used Cars Market Price Regression

Automotive valuation regression pipeline estimating fair market resale prices from vehicle specifications and usage.

## Project Structure

```text
06_Cars_Price_Regression/
├── cars_price_regression_data.csv
├── cars_price_regression_pipeline.ipynb
├── app.py
├── best_model.pkl
├── model_metadata.json
├── requirements.txt
└── README.md
```

## Dataset & Features

- **Dataset File:** `cars_price_regression_data.csv`
- **Task Type:** `Regression`
- **Target Variable:** `selling_price`
- **Numerical Features (4):** `year, km_driven, engine_cc, max_power_bhp`
- **Categorical Features (4):** `brand, fuel, transmission, owner`

## Model Evaluation Summary

- **Selected Best Model:** `Ridge`

| Metric | Score |
| :--- | :--- |
| `r2` | `0.8908` |
| `mae` | `73219.37` |
| `rmse` | `95051.14` |

## Quickstart & Deployment

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the Streamlit web application:
   ```bash
   streamlit run app.py
   ```
