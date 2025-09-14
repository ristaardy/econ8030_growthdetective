# Growth Detective Project

## Project Structure

```
growthdetective/
├── group_project_1_growth_detective.ipynb # Main Jupyter Notebook with data collection, cleaning, analysis, and visualization
└── README.md # Project documentation

```

## Data Sources and Preprocessing Steps
- **Data Source**:
  Part 1, Part 2, Part 3: World Development Indicators (WDI), accessed via Google Sheets.
  Part 4: oecd.org, accessed via Google Sheets.

- **Countries Selected**: Indonesia (IDN), Nepal (NPL), and United States (USA).  

- **Variables Used**:
  **Part 1, Part 2, and Part 3**
  - `NY_GDP_PCAP_CD` → GDP per capita (US$), 1996-2018
  - `SP_POP_TOTL` → Population, total, 1996-2018
  - `SE_PRM_TENR` → Primary school enrollment (gross, %), 1996-2018  
  - `SH_MED_BEDS_ZS` → Hospital beds per 1,000 people, 1996-2018  
  - `SP_POP_TOTL` → Total population, 1996-2018
  
  **Part 4**
  - `GDP_GFCF_YEAR` → Years of GDP and GFCF growth data, 1996–2023
  - `WF_YEAR` → Years of workforce data, 1992–2019
  - `GFCF_GRWT` → Annual GFCF growth, 1996-2023, calculated from GFCF by assets, 1995-2023
  - `WF_GRWT` → Annual Workforce growth, 1992-2019, calculated from population aged 15–64, 1991-2019
  - `GDP_GRWT` → Annual GDP growth, 1996-2023

**Preprocessing Steps**:

**Part 1, Part 2, and Part 3**
1. Import data from Google Sheets using `pandas.read_csv`.  
2. Check data types and missing values (`df.info()`, `df.isna()`).  
3. Interpolate the missing data using both mean and polynomial interpolation.  
4. Prepare the cleaned dataset for descriptive analysis and visualization.  

**Part 4**
1. Import data from Google Sheets using `pandas.read_csv`.
2. Check data types and missing values (`df.info()`, `df.isna()`).
3. Handle missing values (drop or ignore depending on variable availability).
4. Prepare the cleaned dataset for descriptive analysis and visualization.

## Instructions for Replicating the Work
1. Clone this repository:
   ```
   git clone https://github.com/ristaardy/econ8030_growthdetective.git
   cd econ8030_growthdetective
   ```

2. Open the notebook in Jupyter or Google Colab:
   ```
   jupyter notebook group_project_1_growth_detective.ipynb
   ```

3. Make sure the required Python libraries are installed:
   ```
   pip install pandas matplotlib seaborn numpy statsmodels
   ```
4. Run all cells in the notebook to reproduce the workflow.

## Contributors
- [@ristaardy](https://github.com/ristaardy)  
- [@](https://github.com/username)

   ---
