# open-scholarship-project-2026
For the course Open Scholarship.
## Project description:
- In the data queried from Europeana, look into from which provider and/or country the data about World War 1 medals was gathered from. **(Outdated, see Research Step V)**
- ## The data was queried from the [Europeana](https://www.europeana.eu/en) database.
- Date accessed: 29.04.2026
- Licence: CC0
- The data was queried using 'Medal' or 'Medals' as keywords, with 'World War 1' and alternatives added to filter.
- The data was further cleaned to include only the relevant columns.
- The main flaw in the gathered [data](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/europeana_wwi_medals_29.04.2026.csv) is that the country of origin for some entries is simply 'Europe'.

## Workflow
Below is an image to visualize the workflow, i.e. what is done with the original raw data that was queried in order to transform it into a form that is more easy to interpret and from which to gather conclusions. The workflow steps are also included as steps in the research steps further below, this image is included for the sake of clarity.

<img width="2045" height="769" alt="workflow image" src="https://github.com/user-attachments/assets/47c5e8a8-1ba0-4a28-8c48-560f7aa78892" />


## Initial Research Steps (Reconstructed)
- 1. With the help of AI, the code provided for the course on Moodle was edited to query data about World War 1 medals from Europeana.
- 2. The code was further modified so the csv file obtained includes only the relevant columns including provider, country, and description among others. (More information [here](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/notebooks/README.md))
- 3. The code was run on Jupyter Notebooks and the [filtered data from 29.04.2026](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/notebooks/EuropeanaMedals.ipynb) was obtained.
## Research Steps
- 4. With the help of AI, additional code was added and run to gather statistical data from the previously linked file. This file includes metadata statistics on the provider of the queried data and the data's country of origin. The [statistical report](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/metadata_statistics_report.txt) was added to the data section of this project.
- 5. Research into the ['Europeana 1914-1918'](https://wayback.archive-it.org/12090/20241221132121/https://pro.europeana.eu/project/europeana1914-1918) provider, which is the provider of the majority of the data gathered that have "Europe" as their country of origin, resulted in the conclusion that in order to enrich the data entries, the column 'dcLanguageLangAware.def' that includes the default language of the entry could be used. This column has therefore been added to be included in the filtered version of the data. (Initial Research Step ii)
- 6. The following data visualisation was created in order to show the reasoning behind the previous step: <img width="1536" height="1024" alt="country statistics charts" src="https://github.com/user-attachments/assets/688790cc-7e9f-477f-ab8f-82a3bf5e7bb2" />
- 7. The following data visualisation was created to visualize the data providers included in the [data gathered](https://github.com/utku-ayan/open-scholarship-project-2026/blob/main/data/metadata_statistics_report.txt): <img width="1536" height="1024" alt="data provider statistics charts" src="https://github.com/user-attachments/assets/cf7c9be6-bc0e-4f43-8bba-957981f3ad7a" />

