#  Oil Field Profit Prediction

Predictive analysis to identify the most profitable oil wells across three regions using synthetic geological data. The model uses linear regression and bootstrapping to recommend the best region for oil field development under defined business constraints.

---

##  Objective

Help OilyGiant select 200 optimal oil wells to invest in, from 500 explored sites per region. Maximize profitability while managing business risks such as development costs and production uncertainty.

---

##  Dataset Description

Each region has a dataset with the following fields:

- `id`: Well identifier
- `f0`, `f1`, `f2`: Geological features (significance undisclosed)
- `product`: Target variable – volume of oil reserves (in thousand barrels)

---

##  Business Constraints

- Develop 200 oil wells per region
- Budget: $100 million
- Revenue per unit: $4.5K (unit = 1000 barrels)
- Minimum profitable reserve per well: 111.1 units
- Max risk threshold: 2.5%

---

##  Project Workflow

1. **Data Preparation**
   - Load and analyze datasets for each region

2. **Model Training**
   - Linear regression on 75% training / 25% validation split
   - Evaluate RMSE and average predicted production

3. **Profit Calculation**
   - Select top 200 wells by predicted volume
   - Estimate total profit for each region

4. **Risk Assessment**
   - Apply bootstrapping (1000 iterations)
   - Compute 95% confidence intervals
   - Evaluate risk of negative profit

5. **Region Recommendation**
   - Select region with highest expected return and acceptable risk

---

##  Key Insights

- Demonstrated how predictive modeling can support high-stakes investment decisions
- Incorporated real-world budget thresholds and probabilistic risk metrics
- Highlighted the power of bootstrapping to evaluate uncertainty

---

##  Project Structure

```
oil-well-profit-prediction/
│
├── oil_field_profit_prediction.ipynb
├── geo_data_0.csv
├── geo_data_1.csv
├── geo_data_2.csv
├── requirements.txt
└── README.md
```

---

##  Tools & Libraries Used

- Python
- pandas
- numpy
- scikit-learn

---

##  Status

✔️ Project completed as part of the **TripleTen Bootcamp** – Sprint: *Oil Field Profit Estimation & Risk Analysis*

---

##  Author

David Villanueva  
[LinkedIn](https://www.linkedin.com/in/david-villanueva-59659727)  
[GitHub](https://github.com/lolapaul)
