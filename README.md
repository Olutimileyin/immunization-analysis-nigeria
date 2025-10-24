# Public Health Data Analysis: Immunization vs. Disease Cases in Nigeria (1974-2018)

**Overview:** This project uses World Health Organization (WHO) data to analyze the temporal trends and correlation between national childhood immunization coverage and the incidence of vaccine-preventable diseases in Nigeria. The primary goal was to quantify the effectiveness of vaccination programs.
## Tools and Technologies

| Category | Tool/Library | Purpose |
| :--- | :--- | :--- |
| **Language** | Python | Core programming language for analysis. |
| **Environment** | Google Colab / Jupyter Notebook | Interactive environment for data cleaning and execution. |
| **Data Manipulation** | Pandas | Loading, cleaning, transformation, and aggregation of data. |
| **Visualization** | Matplotlib, Seaborn | Creating high-quality time-series plots and scatter plots. |
| **Statistics** | Pearson Correlation | Quantifying the strength and direction of the relationship between variables. |

---

## Analysis Questions & Methodology

### Key Questions Addressed:

1.  How have the coverage rates for key vaccines (e.g., DTP3, Pol3) trended in Nigeria over time?
2.  What are the long-term trends for reported cases of common vaccine-preventable diseases (e.g., Pertussis, Measles)?

### Methodology:

1.  **Data Cleaning:** Initial raw data was cleaned by handling metadata rows, selecting relevant columns (`Indicator`, `Year`, `Numeric Value`), and converting the `Year` and `Value` fields to appropriate numeric data types. Missing values were dropped for time-series integrity.
2.  **Categorization:** Data was logically separated into two DataFrames: **Immunization Coverage** (percentage-based) and **Disease Cases** (count-based).
3.  **Time Series Analysis:** Line plots were generated to visualize long-term trends for the top 5 indicators in each category.

---

## Key Findings

### Time Series Insights:

* **Coverage Success:** Immunization rates for key vaccines like **DTP3** and **Polio (Pol3)** showed a significant and steady upward trend, rising from approximately 40% in the early 2000s to over 55% in recent years.
* **Disease Decline:** Cases for diseases like **Tetanus** and **Diphtheria** demonstrated a strong long-term decline, correlating visually with increased vaccination efforts.
* **Persistent Challenge:** Reported **Measles** cases showed the most volatility, with cyclical peaks in different years, indicating that despite rising coverage, achieving comprehensive herd immunity remains a challenge.


## Visualizations

The core findings are best illustrated through time-series plots.

### 1. Immunization Coverage Trend (1-Year-Olds)

Shows the success of national vaccine efforts over time.

![Time Series of Top 5 Immunization Coverage Indicators in Nigeria]
<img width="1892" height="547" alt="image" src="https://github.com/user-attachments/assets/881e2d89-d000-4e08-8122-2e421fb2b974" />


### 2. Vaccine-Preventable Disease Cases Trend

Illustrates the long-term burden of disease and the impact of intervention.

![Time Series of Top 5 Vaccine-Preventable Disease Cases in Nigeria]
<img width="1225" height="547" alt="image" src="https://github.com/user-attachments/assets/0602b523-0174-4ad8-b159-0c07ff24867f" />


---

## How to Run This Project

To replicate this analysis, follow these steps:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/](https://github.com/)Olutimileyin/immunization-analysis-nigeria.git
    ```
2.  **Open the Notebook:** Open the `Immunization_Analysis.ipynb` file in **Google Colab** or a local Jupyter environment.
3.  **Execute Cells:** Run the notebook cells sequentially to execute the data cleaning, analysis, and visualization code. The charts will be generated inline.

---

## Potential Future Work

This analysis could be extended by:
* Performing sub-national (state-level) analysis if more granular data were available.
* Applying advanced time series models (e.g., ARIMA or Prophet) to forecast future immunization rates and predict potential disease outbreaks.
* Including economic indicators (e.g., GDP per capita) to explore socio-economic factors influencing coverage rates.
