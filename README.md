# Financial Sentiment Analysis: DOW30 10-K Filings

## Overview
This project investigates the relationship between corporate sentiment in 10-K filings and financial performance metrics, focusing on the DOW30 companies. Using Natural Language Processing (NLP) techniques and machine learning models, the project highlights how narrative disclosures can provide predictive insights into financial health.

The primary aim of this project is to explore how corporate sentiment, as expressed in textual disclosures like the Management's Discussion and Analysis (MD&A) sections of 10-K filings, correlates with key financial performance metrics. By leveraging advanced analytics and statistical models, the study uncovers patterns and relationships that can inform better financial decision-making and strategy.

## Objectives
1. **Sentiment Analysis:** To classify the sentiment (positive, negative, or neutral) of narrative sections in 10-K filings using NLP techniques.
2. **Financial Correlation:** To identify and analyze the relationship between sentiment scores and financial performance metrics, such as Return on Assets (ROA).
3. **Industry Segmentation:** To evaluate the variability in sentiment trends and their financial impact across different industries within the DOW30.
4. **Temporal Trends:** To investigate changes in corporate sentiment over time and their association with shifts in financial performance.
5. **Predictive Modeling:** To develop machine learning models that utilize sentiment scores for predicting financial success.

## Key Features
- **Sentiment Extraction:** Comprehensive NLP pipeline for processing and analyzing textual data.
- **Regression Modeling:** Application of Lasso regression for feature selection and predictive insights.
- **Industry-Specific Insights:** Analysis of sentiment trends and their financial implications for various industries.
- **Visualizations:** Rich visual outputs such as graphs, heatmaps, and charts to showcase findings.
- **Reproducible Workflows:** Includes notebooks and scripts for end-to-end reproducibility.

---

## Table of Contents
1. [Motivation](#motivation)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Results](#results)
5. [Repository Structure](#repository-structure)
6. [Usage Instructions](#usage-instructions)
7. [Future Scope](#future-scope)
8. [Contributions](#contributions)
9. [License](#license)

---

## Motivation
Narrative sections in 10-K filings, such as the Management Discussion and Analysis (MD&A), contain qualitative information often overlooked by traditional financial analysis. These narratives reveal corporate optimism, concerns, and strategic priorities. By analyzing these sentiments, this project aims to uncover their predictive power in financial performance, offering valuable insights to investors, researchers, and strategists.

---

## Dataset
### Source:
- **10-K Filings:** Collected from the Securities and Exchange Commission's EDGAR database.
- **Financial Metrics:** Extracted from credible financial databases and annual reports.

### Key Attributes:
- Sentiment scores (positive, negative, neutral).
- Financial performance metrics like ROA.
- Temporal data to analyze changes over time.
- Industry classifications for segmentation.

---

## Methodology
1. **Data Collection:**
   - Narrative sections (MD&A) extracted from 10-K filings.
   - Financial performance data sourced for all DOW30 companies.

2. **Data Preprocessing:**
   - Tokenization, stemming, and lemmatization applied to textual data.
   - Stop words removed to enhance sentiment extraction.

3. **Sentiment Analysis:**
   - Used financial-specific sentiment lexicons for accurate analysis.
   - Classified sentences into positive, negative, or neutral categories using NLP tools.

4. **Statistical Analysis:**
   - Correlation studies to link sentiment scores with ROA.
   - Lasso regression for feature selection and predictive modeling.

5. **Visualization:**
   - Graphs, heatmaps, and trend analysis charts created to visualize sentiment trends and financial correlations.

6. **Industry Segmentation:**
   - Grouped companies by industry to identify sentiment patterns specific to sectors like technology, healthcare, and finance.

7. **Temporal Analysis:**
   - Examined how sentiment evolved over multiple years and its relation to significant economic or market events.

---

## Results
- **Sentiment Impact:** Positive sentiment correlates strongly with higher ROA, while negative sentiment predicts lower financial performance.
- **Industry Variability:** Industries such as technology and healthcare show stronger sentiment-performance relationships compared to others.
- **Temporal Trends:** Sentiment changes over time can act as early warning signals for financial shifts.
- **Key Predictors:** Sentiment metrics often outperform traditional financial indicators in predicting short-term ROA.

---

## Repository Structure
```
├── data
│   ├── processed_data.csv      # Processed dataset used in analysis
│   └── raw_data/               # Raw 10-K filings (optional)
├── notebooks
│   ├── sentiment_analysis.ipynb  # NLP and sentiment extraction
│   ├── regression_modeling.ipynb # Predictive modeling
│   └── visualizations.ipynb      # Charts and graphs
├── src
│   ├── data_preprocessing.py     # Data cleaning scripts
│   ├── sentiment_extraction.py   # NLP pipeline
│   └── regression_analysis.py    # Lasso regression implementation
├── visualizations
│   └── key_findings.png          # Key visualizations
├── README.md
├── LICENSE
└── requirements.txt              # Python dependencies
```

---

## Usage Instructions
### Prerequisites:
- Python 3.8 or higher
- Libraries: pandas, numpy, sklearn, matplotlib, seaborn, nltk

### Steps to Run:
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/FinancialSentimentAnalysis.git
   cd FinancialSentimentAnalysis
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebooks in the `notebooks/` directory to reproduce the analysis.

4. Explore the visualizations in the `visualizations/` folder.

---

## Future Scope
- **Enhanced NLP Models:** Explore transformer-based models (e.g., BERT) for improved sentiment accuracy.
- **Broader Datasets:** Expand analysis to include other indices or international filings.
- **Real-Time Analysis:** Implement pipelines for real-time sentiment monitoring of 10-K filings.
- **Interactive Dashboards:** Develop dashboards for dynamic visualization of sentiment trends and financial correlations.

---

## Contributions
Contributions are welcome! If you'd like to improve this project, feel free to fork the repository and create a pull request. Suggestions for additional analyses, improved models, or expanded datasets are highly encouraged.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
