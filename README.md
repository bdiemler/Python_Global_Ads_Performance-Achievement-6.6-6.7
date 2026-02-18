# Global_ads_performance
This repository features a dual-phase analysis of digital advertising performance across Google, Meta, and TikTok. It combines a Tableau Storyboard for executive strategic insights with a Python Time-Series Analysis to test data stationarity and scalability.
## Project Objective
The primary goal was to identify "Efficiency Leaks" in a multi-channel advertising ecosystem. By analyzing the relationship between Ad Spend and ROAS, the project aims to move the brand from a volume-first strategy to an efficiency-first model, specifically identifying how seasonal trends and platform-specific behaviors impact the global bottom line.

## 1. Tableau Storytelling: Executive Strategy
The Tableau portion of this project focuses on translating raw performance data into a narrative for stakeholders.
### Key Visualizations and Analysis
The Macro Correlation: A dual-axis analysis of global spend vs. revenue to identify historical volatility.
The Stability Benchmark: Using distribution bands (60-80% of average) to categorize Google Ads as a Stability Anchor.
The Scalability Roadmap: A scatter plot with platform-specific trend lines proving TikTok as the primary growth engine.
Geographic Stress Test: A dual-axis map identifying "Red Zones" in North America during July, proving inflexible spend during seasonal slumps.

## 2. Python: Time-Series Analysis 
This phase involved rigorous statistical testing to determine if advertising performance data is stationary and suitable for forecasting.
### Technical Methodology
The analysis was executed end-to-end using the following technical workflow and tools:
Programming Language: Python 3
Environment: Jupyter Notebook / Anaconda
Core Libraries: pandas, NumPy, matplotlib, seaborn, os, statsmodels.api
Data Handling: Merging multiple Instacart datasets, robust data consistency checks, handling mixed-type columns, identifying and addressing missing/duplicate data, and deriving key variables (e.g., price ranges, loyalty status).
Visualization: Generated multiple data visualizations (e.g., bar charts, histograms, heatmaps) to clearly communicate purchasing habits across various customer segments.
Data Sourcing: Integrated campaign data with external time-series data from Kaggl.
Preprocessing: Cleaned data removing columns, checking for missing data and duplicates. Smoothing data to remove noise.
Time-Series Decomposition: Broke down data into Trend, Seasonality, and Noise/Residuals to analyze underlying patterns.
Stationarity Testing:Performed the Augmented Dickey-Fuller (ADF) Test. 

### Repository Structure
Global-Ads-Performance |-- 01_Importing_libraries_and_data/ |-- 02_Checking_the_data/ | |--03_Cleaning_data/  |-- 04 Linechart | Smoothing_the_data/ |--05_Time_series_analysis_decomposition/ |--06_Testing_for_stationary

### Data Citation
Main Dataset: Global Ads Performance (Google, Meta, TikTok) by Nudrat Abbas, accessed via Kaggle (CC0: Public Domain).
Note: This dataset was synthetically generated using probabilistic modeling to reflect realistic digital advertising performance patterns across platforms, industries, and regions.

Tableau Storytelling Link: https://public.tableau.com/views/Whereisournextdollarmosteffectivearesearchonmaincampaignchannels_/Intro?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link 
