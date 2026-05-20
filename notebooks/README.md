# This folder will store Jupyter Notebooks used for data processing.
## In the Notebook titled "EuropeanaMedals" the [code](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/notebooks/EuropeanaMedals.ipynb), written with the help of AI, creates the following 3 output files after querying the Europeana database for World War 1 medals: 
### - A sample file named "wwi_medals_sample_100" that only includes 100 entries.
### - The whole data queried with every column present in a file named "wwi_medals_high_precision."
### - A filtered file named ["wwi_medals_filtered"](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/wwi_medals_filtered_columns_20.05.2026.csv) that only includes the following columns:
  - "dcSubjectLangAware.en"
  - "dctermsSpatial"
  - "edmTimespanLabelLangAware.en"
  - "edmConceptPrefLabelLangAware.en"
  - "year"
  - "type"
  - "title"
  - "provider"
  - "dataProvider"
  - "country"
  - "completeness"
## In the next cell that includes code, the file ["wwi_medals_filtered"](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/wwi_medals_filtered_columns_20.05.2026.csv) is subjected to further statistical analysis. The following columns are analysed:
  - "provider"
  - "dataProvider"
  - "country"
### A [text file](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/metadata_statistics_report.txt) is created with the statistical data, which includes what exists in these columns and how many times each entry is repeated.
