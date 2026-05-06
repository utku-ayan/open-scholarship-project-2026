# This folder will store Jupyter Notebooks used for data processing.
## In the Notebook titled "EuropeanaMedals" the [code](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/notebooks/EuropeanaMedals.ipynb), written with the help of AI, creates the following 3 output files after querying the Europeana database for World War 1 medals: 
### - A sample file named "wwi_medals_sample_100" that only includes 100 entries
### - The whole data queried with every column present in a file named "wwi_medals_high_precision"
### - A filtered file named ["wwi_medals_filtered"](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/europeana_wwi_medals_29.04.2026.csv) that only includes the following columns:
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
