# Global COVID-19 Vaccination Uptake: A Longitudinal Cross-Country Analysis

## 📊 Project Overview

This project provides a comprehensive longitudinal analysis of COVID-19 vaccination uptake across countries worldwide, examining temporal trends and inter-country variability in vaccination coverage from December 2020 to March 2022.

### 🎯 Research Objective

To examine temporal trends in COVID-19 vaccination uptake across countries and assess inter-country variability in vaccination coverage.

### 📋 Study Design

**Type**: Observational, longitudinal analysis  
**Data**: Publicly available secondary data  
**Unit of Analysis**: Country-level daily vaccination records  
**Time Period**: December 2020 - March 2022  

## 📁 Repository Structure

```
COVID_19_vaccination/
├── COVID_19_vaccination.ipynb    # Main analysis notebook
├── COVID_19_vaccination.py       # Python script version
├── README.md                     # This file
└── data/                        # Downloaded from Kaggle (cache)
```

## 🗂️ Data Source

**Dataset**: [COVID-19 World Vaccination Progress](https://www.kaggle.com/datasets/gpreda/covid-world-vaccination-progress)  
**Platform**: Kaggle  
**Access**: Automated download via `kagglehub`  
**Update Frequency**: Regularly updated during the pandemic period  

### Key Variables Analyzed
- `country`: Country name
- `date`: Report date 
- `total_vaccinations`: Cumulative vaccination doses administered
- `people_vaccinated`: Number of people who received at least one dose
- `people_fully_vaccinated`: Number of fully vaccinated individuals
- `people_vaccinated_per_hundred`: Vaccination coverage rate (%)
- `daily_vaccinations`: Daily vaccination pace

## 🧹 Data Quality & Cleaning

### Initial Data Challenges
- **Missing Data**: 50-55% missing values in vaccination metrics
- **Temporal Missingness**: Countries started vaccination programs at different times
- **Reporting Inconsistencies**: Varying data collection practices across countries

### Cleaning Strategy
1. **Pre-vaccination Period Removal**: Excluded time periods before vaccination programs started
2. **Country Filtering**: Included only countries with substantial rollout (≥5% population coverage)
3. **Result**: Reduced missing data from 50-55% to 6.2%

### Final Dataset
- **Records**: 43,642 vaccination records
- **Countries**: 214 countries with robust data
- **Time Span**: Active vaccination periods only
- **Data Quality**: 93.8% completeness for key metrics

## 🔍 Analysis Components

### 1. **Descriptive Analysis**
- Dataset characteristics and structure
- Missing data assessment and handling
- Summary statistics of vaccination metrics

### 2. **Scale of Vaccination Programs**
- Top 10 countries by absolute vaccination numbers
- Comparison of national rollout scales
- Visualization of vaccination program magnitude

### 3. **Longitudinal Trends Analysis**
- Time-series visualization of vaccination coverage
- Representative country selection (US, UK, India, Nigeria, Brazil)
- Temporal patterns in vaccination uptake rates

### 4. **Cross-Country Comparison**
- Endpoint analysis of final vaccination coverage
- Ranking of best and worst performing countries
- Inter-country variability assessment

## 📈 Key Visualizations

1. **Bar Chart**: Top 10 countries by total vaccinations (rollout scale)
2. **Time Series Plot**: Vaccination coverage trends over time for selected countries
3. **Statistical Summary**: Distribution of final vaccination coverage across all countries

## 🔑 Key Findings

### Temporal Trends
- Countries showed diverse vaccination progression patterns
- Some achieved rapid early uptake while others demonstrated gradual adoption
- Clear evidence of varying policy approaches and infrastructure capabilities

### Inter-Country Variability  
- Substantial differences in final vaccination coverage across countries
- Wide range of vaccination rates reflecting healthcare infrastructure differences
- Evidence of global vaccination inequality

## ⚙️ Technical Requirements

### Dependencies
```python
pandas>=1.3.0
matplotlib>=3.3.0
kagglehub>=0.1.0
jupyter>=1.0.0
```

### Installation & Setup
```bash
# Clone repository
git clone <repository-url>
cd COVID_19_vaccination

# Install dependencies
pip install pandas matplotlib kagglehub jupyter

# Launch analysis
jupyter notebook COVID_19_vaccination.ipynb
```

## 🚀 Usage Instructions

### Option 1: Jupyter Notebook (Recommended)
1. Open `COVID_19_vaccination.ipynb` in Jupyter
2. Run cells sequentially from top to bottom
3. Data will be automatically downloaded on first run

### Option 2: Python Script
1. Run the script version: `python COVID_19_vaccination.py`
2. Outputs will be displayed in terminal

### Data Access
- First run automatically downloads latest data via Kagglehub
- Data cached locally for subsequent runs
- No manual download required

## 📊 Methodology

### Inclusion/Exclusion Criteria
**Included:**
- Countries with substantial vaccination programs (≥5% population coverage)
- Time periods after vaccination program initiation

**Excluded:**
- Pre-vaccination periods (before program start)
- Countries with minimal vaccination rollout (<5% coverage)

### Missing Data Handling
- Pre-vaccination periods excluded rather than imputed
- Program gaps treated as legitimate missing data
- No artificial imputation performed to preserve data integrity

### Country Selection for Longitudinal Analysis
Representative countries chosen to reflect:
- Geographic diversity (5 continents)
- Economic diversity (developed and developing nations)  
- Population diversity (large and medium-sized countries)

## 📋 Research Implications

### Public Health Insights
- Documents global variation in vaccination program success
- Provides evidence base for future pandemic preparedness
- Highlights importance of healthcare infrastructure investment

### Policy Relevance
- Informs understanding of vaccination program effectiveness
- Supports evidence-based pandemic response planning
- Demonstrates value of coordinated global health initiatives

## ⚠️ Limitations

1. **Data Availability**: Analysis limited to countries with sufficient reporting
2. **Temporal Scope**: Analysis ends March 2022 (pandemic mid-point)
3. **Country Selection**: Longitudinal analysis uses representative sample, not exhaustive
4. **Causality**: Observational design cannot establish causal relationships
5. **Data Quality**: Dependent on individual country reporting accuracy

## 📚 Future Directions

- **Extended Timeline**: Include booster vaccination data
- **Socioeconomic Analysis**: Correlate vaccination rates with development indicators
- **Policy Analysis**: Link vaccination success to specific policy interventions
- **Seasonal Patterns**: Investigate seasonal vaccination trends

## 👥 Contributing

Contributions welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request with clear description

## 📄 License

This project is open source. Data sourced from public Kaggle dataset under original licensing terms.

## 📞 Contact

For questions about the analysis or methodology, please open an issue in the repository.

---

**Last Updated**: February 2026  
**Analysis Period**: December 2020 - March 2022  
**Countries Analyzed**: 214 countries with robust vaccination data
