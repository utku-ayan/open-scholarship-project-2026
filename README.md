# Europeana Metadata Analysis
For the course Open Scholarship 2026.
## Project description:
- In the data queried from Europeana, look into from which country the data about World War 1 medals was gathered from. 
- ## The data was queried from the [Europeana](https://www.europeana.eu/en) database.
- Date accessed: 29.04.2026
- The data was queried using 'Medal' or 'Medals' as keywords, with 'World War 1' and alternatives added to filter.
- The data was further cleaned to include only the relevant columns.
- The main flaw in the gathered [data](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/wwi_medals_filtered_columns_20.05.2026.csv) is that the country of origin for some entries is simply 'Europe'.

## Workflow
Below is an image to visualize the workflow, i.e. what is done with the original raw data that was queried in order to transform it into a form that is more easy to interpret and from which to gather conclusions. The workflow steps are also included as steps in the research steps further below, this image is included for the sake of clarity.

<img width="2045" height="769" alt="workflow image" src="https://github.com/user-attachments/assets/47c5e8a8-1ba0-4a28-8c48-560f7aa78892" />


## Initial Research Steps (Reconstructed)
- 1. With the help of AI, the code provided for the course on Moodle was edited to query data about World War 1 medals from Europeana.
- 2. The code was further modified so the csv file obtained includes only the relevant columns including provider, country, and description among others. (More information [here](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/notebooks/README.md))
- 3. The code was run on Jupyter Notebooks and the [filtered data from 20.05.2026](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/wwi_medals_filtered_columns_20.05.2026.csv) was obtained.
## Research Steps
- 4. With the help of AI, additional code was added and run to gather statistical data from the previously linked file. This file includes metadata statistics on the provider of the queried data and the data's country of origin. The [statistical report](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/metadata_statistics_report.txt) was added to the data section of this project.
- 5. Research into the ['Europeana 1914-1918'](https://wayback.archive-it.org/12090/20241221132121/https://pro.europeana.eu/project/europeana1914-1918) provider, which is the provider of the majority of the data gathered that have "Europe" as their country of origin, resulted in the conclusion that in order to enrich the data entries, the column 'dcLanguageLangAware.def' that includes the default language of the entry could be used. This column has therefore been added to be included in the filtered version of the data. (Initial Research Step ii)
- 6. The following data visualisation was created in order to show the reasoning behind the previous step: <img width="290" height="397" alt="country-chart" src="https://github.com/user-attachments/assets/918911e1-2853-4e9c-ad52-b1b435dc238d" />
- 7. The following data visualisation was created to visualize the data providers included in the [data gathered](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/metadata_statistics_report.txt): <img width="293" height="455" alt="provider-chart" src="https://github.com/user-attachments/assets/54512011-6f8f-4cd9-a902-cd368594ee25" />
- 8. A new [metadata statistical analysis report](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/metadata_statistics_report_europe_only.txt) was created, that only analyses the entries with "Europe" in their country column. This report includes the frequency report of the default language column of these entries. The plan is to infer the country of entries from the default language in their 'dcLanguageLangAware.def' column. **Note that the missing value amount in the report here drops from 245 to only 6 when only entries with "Europe" in their country column are analysed.**
- 9. The reasoning behind the previous step is the fact that no other field was consistently filled or informative enough across entries even with the filtering. 
- 10. Another report was created from the previous file manually, since the metadata about the default languages was not standardised, and the default language counts of the entries that had "Europe" listed as their origin was finalized. Note that this does not answer the research question perfectly. Some issues with this approach are:
  - The fact that the default language of the entry not having to perfectly match the country of origin of said entry.
  - The fact that multiple countries share languages, for example Austria and Germany sharing German, and France and Belgium sharing French.
  - The existance of entries with multiple default languages. Even though this is a very small section of the entries present, it still could present an issue.
  - Some entries still had missing or undefined default language values. This is also a very small number, yet makes the data not fully complete nonetheless.
- 11. Below is a visualisation of the report created manually: <img width="566" height="349" alt="single-multi-language-charts" src="https://github.com/user-attachments/assets/fef311df-38d1-45ce-8262-ccdd865682db" />

## Conclusion
Looking into the metadata queried at the start of this project had already led to a change in the scope of this project from a statistical analysis to an enrichment of missing data values. Unfortunately, this hasn't resulted in much success, since the only field that was seen fit to analyse is problematic as stated above. The statistical analysis of what languages each entry provided by the 'Europeana 1914-1918' collection, although could be meaningful, was not useful in answering my research question.

In regards for a possible future outlook, I believe a project of a larger scope, analysing both the titles and contents in combination with the default languages of entries, it could be possible to infer the origin countries with hopefully good enough accuracy. This is only a theoretical statement however, as the titled and contents not being consistent enough might hinder any works in this area.

