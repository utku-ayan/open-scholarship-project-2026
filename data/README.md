# This folder contains raw and cleaned data files.
## As of 12.05.2026, the following data files are present from the data obtained from Europeana related to World War 1 medals:
- The filtered bulk of data as a [.csv file](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/wwi_medals_filtered_columns_20.05.2026.csv), which includes the following columns from the queried data (created on 29.04.2026):
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
- A [statistical report](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/metadata_statistics_report.txt) that was created by going through the previous file that includes statistical data on the following columns, which provides an analysis of which entries exist and how many times they come up (created on 12.05.2026):
  - "provider"
  - "dataProvider"
  - "country"
- A [statistical report](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/metadata_statistics_report_europe_only.txt) on the default languages of entries, in order to help determine the entries' origins.
  - Using this report, a [seperate report](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/language%20count.txt) was created manually, counting and adding up each languages occurance numbers. This was done manually because the default language data gathered from Europeana was not in a standard format across entries. 
