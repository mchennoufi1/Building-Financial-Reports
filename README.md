# Financial Ratio Analysis for Hedge Fund Portfolio

## 📊 Project Overview
Comprehensive financial analysis of companies across Technology, FMCG, and Real Estate sectors to evaluate leverage and profitability ratios for investment decision-making.

## 🎯 Objectives
- Calculate and compare leverage ratios (Debt-to-Equity) across industry sectors
- Analyze profitability ratios (Operating Margin) to identify sector performance
- Investigate correlation between leverage and profitability in real estate investments

## 🛠️ Technical Skills Demonstrated
- **Python Libraries**: pandas, numpy, seaborn, matplotlib
- **Data Processing**: Multi-source data merging, data cleaning, column standardization
- **Financial Analysis**: Ratio calculation, correlation analysis, sector comparison
- **Statistical Analysis**: Groupby aggregations, correlation coefficients

## 📈 Key Findings

### 1. Profitability Analysis
- **Lowest Operating Margin**: FMCG sector (20.71%)
- **Highest Operating Margin**: Real Estate sector (29.99%)
- **Tech Sector**: Moderate profitability (27.39%)

### 2. Leverage Analysis
- **Highest Debt-to-Equity**: Real Estate (3.88x)
- **Moderate Leverage**: FMCG (2.85x)
- **Lowest Leverage**: Technology (1.78x)

### 3. Real Estate Correlation
- **Strong positive correlation** (r = 0.825) between leverage and profitability
- Indicates successful use of debt to amplify returns in real estate investments

## 💡 Business Insights
1. **FMCG companies** operate on thin margins due to competitive pressures
2. **Tech companies** maintain high profitability with minimal debt dependency
3. **Real Estate firms** effectively leverage debt to maximize returns on capital

## 🔧 Technical Implementation

### Data Processing
```python
# Merged balance sheet and income statement data
df = pd.merge(balance_sheet, income_statement, 
              on=['Company', 'comp_type', 'Year'])

# Calculated key financial ratios
leverage_ratio = Total_Liabilities / Total_Stockholder_Equity
profitability_ratio = Operating_Income / Total_Revenue
```

### Analysis Methodology
- Grouped data by industry sector (comp_type)
- Calculated mean ratios for sector-level comparison
- Performed correlation analysis for real estate subset

## 🚀 How to Run
```bash
# Clone repository
git clone https://github.com/yourusername/financial-analysis-hedge-fund.git

# Install dependencies
pip install -r requirements.txt

# Run analysis
python src/analysis.py
```

## 📦 Requirements
```
pandas>=1.3.0
numpy>=1.21.0
seaborn>=0.11.0
matplotlib>=3.4.0
openpyxl>=3.0.0
```

## 🎓 Learning Outcomes
- Applied financial ratio analysis to real-world investment scenarios
- Developed proficiency in multi-source financial data integration
- Enhanced understanding of sector-specific capital structures
- Strengthened data manipulation and statistical analysis skills

```
