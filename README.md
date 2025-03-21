# UNICEF Primary School Global Out-of-School Rates Analysis

## 📊 Project Overview

This data analysis project examines worldwide patterns of primary school exclusion using UNICEF's out-of-school rates dataset. The analysis explores educational disparities across regions, gender, geographic location, and wealth levels to identify where educational exclusion is most severe and which factors most strongly correlate with children being out of school.

The project supports SDG 4 (Quality Education) by providing data-driven insights to help target interventions where they're most needed.

### 🎯 Project Objectives

1. Clean and preprocess the UNICEF out-of-school rates dataset
2. Explore regional and demographic patterns in education access
3. Identify factors that correlate with higher out-of-school rates
4. Create UNICEF-aligned visualizations to communicate key findings
5. Provide actionable recommendations for UNICEF programming and policy advocacy

## 📋 Dataset

The analysis uses UNICEF's global dataset on primary school out-of-school rates containing information across:
- Regional classifications (SSA, MENA, SA, LAC, EAP, ECA, NA)
- Gender breakdowns (female and male percentages)
- Rural/urban divides
- Wealth quintiles (poorest to richest)
- Population data for different demographic groups

**Source**: UNICEF Global Databases - Out of School Rate, 2022  
https://data.unicef.org/wp-content/uploads/2019/09/Out_of_school_rate_2022_formatted.xlsx

## 🔍 Methodology

### Data Preprocessing
- Cleaned and standardized column names
- Handled missing values through appropriate imputation techniques
- Converted string variables to numeric types
- Implemented data validation checks

### Analysis Approach
- **Population-weighted metrics**: All key statistics are weighted by population to accurately represent impact on children
- **Regional analysis**: Patterns examined across UNICEF regions
- **Disparity analysis**: Calculation of gender gaps, rural-urban divides, and wealth-based inequalities
- **Comparative visualizations**: Implementation of appropriate visualization types for different analysis needs

## 📈 Key Findings

### 1. Regional Disparities
Sub-Saharan Africa (SSA) has the highest out-of-school rates (~22%), far exceeding the global average (~11%), highlighting the combined impact of poverty, conflict, and infrastructure challenges.

### 2. Gender Analysis
Gender disparity patterns vary considerably by region:
- Girls are more disadvantaged in SSA, SA, and parts of MENA
- Boys are disadvantaged in regions like LAC, EAP, and ECA
- The global gender gap is approximately 0.8 percentage points (higher for girls)

### 3. Rural-Urban Divide
Rural children consistently have higher out-of-school rates than urban children across all regions, with rural rates typically 1.5-2x higher than urban rates, reflecting infrastructure challenges and teacher shortages in rural areas.

### 4. Wealth-Based Inequality
The wealth gap in education access is the most consistent and extreme form of disparity:
- Children from the poorest quintile are 3-5x more likely to be out of school than those from the richest quintile
- The poorest quintile has out-of-school rates of 20-40% in the most affected regions
- Even in high out-of-school regions, the richest quintile often has rates below 5%

### 5. Scale of the Challenge
- Approximately 11% of primary school-aged children globally are out of school
- This translates to millions of children without access to basic education
- SSA accounts for nearly 60% of all out-of-school children globally

## 💻 Setup and Usage

### Prerequisites
- Python 3.6+
- Jupyter Notebook
- Required libraries (pandas, numpy, matplotlib, seaborn)

### Installation

```bash
# Clone this repository
git clone https://github.com/yourusername/unicef-education-analysis.git
cd unicef-education-analysis

# Create a virtual environment (optional but recommended)
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Running the Analysis

```bash
# Launch Jupyter Notebook
jupyter notebook

# Open the main analysis notebook
# unicef-final-analysis.ipynb
```

## 📦 Repository Structure

```
unicef-education-analysis/
│
├── data/
│   ├── raw/                        # Original dataset
│   │   └── Out_of_school_rate_2022_formatted.xlsx
│   └── processed/                  # Cleaned data
│       └── Primary-Table 1.csv
│
├── notebooks/
│   └── unicef-final-analysis.ipynb # Main analysis notebook
│
├── visualizations/                 # Generated charts and graphs
│   ├── regional_disparities.png
│   ├── gender_analysis.png
│   ├── rural_urban_divide.png
│   ├── wealth_inequality.png
│   └── oos_distribution.png
│
├── requirements.txt                # Python dependencies
└── README.md                       # Project documentation
```

## 🔮 Conclusions and Recommendations

### Conclusions
1. Education access disparities follow clear patterns related to wealth, gender, and geography, requiring systematic policy responses.
2. The predominance of wealth-based inequality suggests that economic barriers remain the most persistent obstacle to education access.
3. Progress toward SDG targets is uneven, with many countries in SSA facing particularly challenging trajectories.
4. The varying patterns of disadvantage across regions suggest that context-specific interventions are necessary rather than one-size-fits-all approaches.

### Recommendations for UNICEF
1. **Targeted Investment Strategies**: Prioritize resources toward SSA and conflict-affected areas with highest out-of-school rates

2. **Gender-Specific Programs**: Implement girl-focused education initiatives in regions with significant gender gaps

3. **Rural Education Enhancement**: Improve school infrastructure and teacher incentive programs in rural areas

4. **Economic Support for Low-Income Families**: Implement conditional cash transfer programs tied to school attendance

5. **Policy Advocacy**: Advocate for education policies that specifically target wealth-based inequality through school fee elimination and school feeding programs

## 📝 Limitations and Future Work

### Limitations
- Data recency varies by country, making direct comparisons challenging
- Some countries lack complete data across all dimensions
- Additional factors not captured include conflict situations, disability status, and education quality

### Future Work
- Include time-series analysis to track progress over multiple years
- Develop a Multidimensional Vulnerability Index to identify areas of highest need
- Create an SDG trajectory analysis to assess progress toward 2030 targets
- Build an interactive dashboard for exploring the data across multiple dimensions

## 🙏 Acknowledgments

- UNICEF for making this data publicly available
- The global education community working to ensure all children have access to quality education

---
