"Züri Wie Neu"-Project (SDS210)

This repository contains an analysis of the "Züri Wie Neu" data. There are 4 spatial questions to be answered: 
1a: Which is the category with the highest number of reports?
1b: Which are the top 3 'Quartiere'/'Kreise' with the most reports?
2: Is the density of reports higher around the lake (in 'Kreise' 1,2 and 8) than elsewhere?
3: How does the report density around the lake differ between august (summer) and january (winter)?
4: Which trend does the august (summer) and january (winter) data around the lake show within the report period?

The data is obtained from the following databases: 
- Züri Wie Neu: https://data.stadt-zuerich.ch/dataset/geo_zueri_wie_neu
- 'Kreise' and 'Quartiere': https://data.stadt-zuerich.ch/dataset/geo_statistische_quartiere
- Data on the area of districts: https://data.stadt-zuerich.ch/dataset/bev_jahr_flaechen_bodenbedeckungsart_od5803

The software and libraries required to run the code successfully can be found in the environment.yml, see SDS210-PROJECT/environment.yml.

To successfully execute the project, the jupyter notebook can be run from top to bottom, code block per code block. 
The code is structured in the following way:
- data imports for all 4 subparts are done at the beginning of the project
- each question is answered in a separate code block which comes with a markdown title including the question
- display(data.head()), print(data.head()) are deleted from the code as means of clarity, but can be inserted (and were conducted to check integrity of previous actions, check dtypes and crs, ...) where necessary
- not every line is commented, but some important comments are given