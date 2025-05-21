# Analysis of the pharmacy register in Poland (EDA + FE)

The aim of this project is to conduct an exploratory data analysis and perform feature engineering on a dataset containing information about pharmacies operating in Poland. The analysis enables a better understanding of the data structure, identification of important variables, and preparation of the dataset for further modeling, including machine learning applications.

The project includes:

-   Preprocessing features to comply with ML standards
-   Aggregating data at the county (powiat) level
-   Applying K-Means clustering to reduce feature cardinality
-   Creating geographical and statistical visualizations to support analysis

## Data Sources

-   **Pharmacy register** (`rejestr_aptek.xls`) – data as of April 28, 2025, made available by the Center for e-Health via <https://dane.gov.pl>
-   **Population by county** (`ludnosc_powiat.csv`) – supplementary demographic data retrieved from the Local Data Bank (Bank Danych Lokalnych) of Statistics Poland: <https://bdl.stat.gov.pl/>
-   **County boundaries shapefiles** (`powiaty/`) – full administrative map of Poland with county divisions, downloaded from the Head Office of Geodesy and Cartography (GUGiK): <https://www.gugik.gov.pl/>

## Techniques Used

-   **Feature Engineering**:

    -   Handling missing values
    -   Transforming categorical features into binary variables
    -   Clustering counties based on aggregated characteristics
    -   Encoding categorical variables

-   **Exploratory Data Analysis**:

    -   Distribution analysis of variables
    -   Correlation analysis
    -   Data visualization

## Libraries Used

-   `pandas`, `numpy` – data manipulation and analysis
-   `matplotlib`, `seaborn` – statistical visualizations
-   `scipy.stats` – statistical analysis
-   `scikit-learn` – scaling, clustering (K-Means)
-   `geopandas` – spatial data analysis

## Key Findings

The project identified key factors influencing the characteristics of pharmacies in Poland. County-level clustering revealed distinct regional differences in the conditions under which pharmacies operate. The analysis highlighted important relationships, suggesting that factors such as population density, internet availability, email and phone contact, legal form of ownership, and the pharmacy's age may significantly affect their longevity and stability. The project offers valuable insights for further in-depth studies using advanced predictive models.

## Project Structure

-   `eda_fe_apteki_full.ipynb` – main notebook with code and analysis
-   `eda_fe_apteki_code.ipynb` – notebook with code only
-   `eda_fe_apteki_report.pdf` – PDF report with analysis
-   `rejestr_aptek.xls` – raw data from the pharmacy register
-   `ludnosc_powiat.csv` – supplementary demographic data
-   `powiaty/` – folder with counties shapefiles
