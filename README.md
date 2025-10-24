# Analysis of Trader Behavior vs. Market Sentiment

## 1. Project Objective

This project performs an in-depth analysis of trader behavior to understand how it aligns or diverges from overall market sentiment (e.g., a "Fear & Greed" index).

The primary goal is to move beyond "average" behaviors and identify **hidden trends** and distinct **trader profiles**. By segmenting traders using K-Means clustering, we uncover specific, data-driven insights that can lead to smarter and more nuanced trading strategies.

## 2. Key Findings

The analysis reveals two main layers of insight:

1.  **Apparent Alignment:** At first glance, the "average" trader follows the herd. As market sentiment moves from 'Fear' to 'Greed', there is a clear, corresponding increase in **trading volume**, **leverage employed**, and **risk-taking** (P&L volatility).
2.  **Hidden Divergence & Profiles:** The "average" trader is a myth. A K-Means cluster analysis segments traders into distinct profiles with dramatically different behaviors:
    * **Conservative / Low-Risk:** This group is profitable, maintains low leverage, and largely ignores market sentiment, demonstrating a consistent and stable strategy.
    * **High-Leverage Gamblers:** This group uses extreme leverage, has a very low win rate, and loses significant money. Their behavior is amplified by market sentiment, leading to reckless decisions.
    * **High-Risk, High-Profit Whales:** This professional group takes on massive risk/volatility but does so with an extremely high win rate, resulting in massive profits.

The analysis proves that a "smarter strategy" is one that maintains a consistent risk profile, similar to the "Conservative" group, rather than letting market euphoria dictate behavior.


## 3. How to Run the Analysis

To reproduce the findings in this project, follow these steps:

1.  **Ensure all `.csv` files** are located inside the `csv_files/` directory. (The csv files are compressed to .gz format due to large size)
2.  **Open the `notebooks/notebook_1.ipynb` file** in a Jupyter environment (like Jupyter Lab, VS Code, or Google Colab).
3.  **Run the notebook cells** sequentially from top to bottom.
    * The notebook will load the data from `csv_files/`.
    * It will perform all data cleaning, feature engineering, and analysis.
    * It will automatically save all charts to the `outputs/` directory.
    * It will train and evaluate the clustering and predictive models.

## 4. Technologies Used

This analysis is built primarily in Python, using the following key libraries:

* **Pandas:** For data manipulation and aggregation.
* **Scikit-learn (sklearn):** For K-Means clustering and Random Forest predictive modeling.
* **Matplotlib & Seaborn:** For data visualization and generating all plots.
