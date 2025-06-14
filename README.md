# CBG Demographic Analysis for Restaurant Location Planning

## Project Overview
This project analyzes Census Block Group (CBG) demographic data to identify optimal locations for restaurant expansion, with a specific focus on Wisconsin. The analysis combines demographic data, housing information, education levels, and income distribution to identify underserved areas that meet specific business criteria.

## Data Source
This project utilizes publicly available Census Block Group (CBG) demographic data from Google Cloud Platform's BigQuery public datasets. The data can be accessed for free through GCP's database marketplace and includes:
- Census Block Group demographics
- Area type classifications
- Brand and business information
- Visit patterns
- Geographic identifiers

## Key Findings

### Population Distribution
- Rural Areas: 66.9M population across 90,801 CBGs
- Suburban Areas: 178.3M population across 84,651 CBGs
- Urban Areas: 84.7M population across 66,883 CBGs

### Housing Characteristics
- Rural CBGs show higher rates of home ownership (≥75% in 25,900 CBGs)
- Urban areas have more diverse housing patterns with significant rental populations
- Suburban areas show balanced distribution between owned and rented properties

### Education Levels
- Rural areas show higher concentration of educated population (≥75% in 38,150 CBGs)
- Urban areas demonstrate strong education metrics with 20,568 CBGs having ≥75% educated population
- Suburban areas show balanced education distribution

### Income Distribution
- Rural areas show higher concentration of lower income brackets
- Urban areas demonstrate more diverse income distribution
- Suburban areas show strong middle-income presence

## Methodology

### Data Classification
1. **Area Classification**
   - Rural: Population ≤ 2,000 & Houses < 1,800
   - Suburban: 2,000 < Population ≤ 10,000 & Houses < 7,200
   - Urban: Population > 10,000

2. **Target Brand Analysis**
   - Analyzed 16 major restaurant brands including:
     - Cracker Barrel
     - Bob Evans
     - Perkins Restaurant & Bakery
     - IHOP
     - Denny's
     - And others

3. **Location Selection Criteria**
   - At least 30% of population with collegiate degrees
   - At least 10% of population with income over $100K
   - Underserved ratio of people to restaurants
   - Based on Brookfield, Wisconsin benchmarks

## Results
The analysis identified 24 potential CBGs across 16 counties in Wisconsin that meet the established criteria for restaurant expansion. These locations were selected based on:
- Demographic compatibility
- Market undersaturation
- Educational attainment
- Income levels
- Existing competition

## Project Structure
```
CBGDemographicAnalysis/
├── README.md
├── analysis/
│   ├── queries/               # SQL queries used for analysis
│   │   └── query_log.txt      # Detailed query log
│   └── results/               # Analysis results and findings
├── docs/
│   ├── report.pdf             # Detailed analysis report
│   └── presentation.pptx      # Project presentation
└── .gitignore                 # Git ignore file
```

## Technical Details
- Data Source: US Census Data via Google Cloud Platform BigQuery
- Analysis Tools: BigQuery SQL
- Key Metrics:
  - Population density
  - Housing patterns
  - Education levels
  - Income distribution
  - Restaurant density

## Future Work
- Real-time data updates
- Integration with additional demographic factors
- Expansion of analysis to other states
- Development of automated reporting tools

## Contributing
This project is open for contributions. Please follow these steps:
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request 