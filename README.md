# SDG 3: Predicting Malaria Outbreaks with Machine Learning

This project is a machine learning solution to address **UN Sustainable Development Goal 3 (Good Health and Well-being)**. It uses a regression model to forecast malaria cases based on climate data, providing an early-warning tool for public health officials.

## 1. The SDG Problem
Malaria, a climate-sensitive disease, poses a significant burden in Sub-Saharan Africa. Public health agencies face challenges in allocating limited resources (like medicine and bed nets) efficiently. This project provides a data-driven tool to help them move from a *reactive* to a *proactive* response.

## 2. The ML Solution
We used a **Supervised Learning (Linear Regression)** model in Python (via Google Colab) to find the relationship between:
* **Features (X):** Average Temperature & Total Rainfall
* **Target (y):** Number of Reported Malaria Cases

## 3. Results & Demo
The model was trained on 80% of the data and tested on 20%.
* **R-squared:** **0.81** (This means 81% of the change in malaria cases can be explained by the climate data).
* **Mean Absolute Error (MAE):** **108,928** (Our predictions are, on average, off by this many cases).

### Model Performance
![Model Performance Plot](plot.png)

## 4. Ethical Considerations
The primary risk is **data bias**. Health data from remote regions is often under-reported. This model could learn to *under-predict* risk in these vulnerable areas. It should be used to *supplement* expert knowledge, not replace it.
