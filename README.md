"Züri Wie Neu"-Project (SDS210)

# the project
This notebook analyzes spatial patterns within the data from the "Züri Wie Neu" platform (where city inhabitants can report damages at the cities infrastructure).

# the goal
This project aims to analyze spatial patterns in the report density following the shores of lake Zurich

# questions to be answered
This repository contains an analysis of the "Züri Wie Neu" data. There are 4 spatial questions to be answered: 
1a: Which is the category with the highest number of reports?
1b: Which are the top 3 'Quartiere'/'Kreise' with the most reports?
2: Is the density of reports higher around the lake (in 'Kreise' 1,2 and 8) than elsewhere?
3: How does the report density around the lake differ between august (summer) and january (winter)?
4: Which trend does the august (summer) and january (winter) data around the lake show within the report period?

# data sources
The data is obtained from the following databases: 
- Züri Wie Neu: https://data.stadt-zuerich.ch/dataset/geo_zueri_wie_neu
- 'Kreise' and 'Quartiere': https://data.stadt-zuerich.ch/dataset/geo_statistische_quartiere
- Data on the area of districts: https://data.stadt-zuerich.ch/dataset/bev_jahr_flaechen_bodenbedeckungsart_od5803

# input data
- 'meldungen_csv': "Züri wie Neu" data containing the reports
- 'quartiere_json' and 'quartiere_csv': the 'Kreise' from the city of Zurich
- 'fläche_csv': area of the 'Kreise'

# outputs
The output compounds 
- tables (questions 1a,b)
- a map to compare summer and winter data (question 3) ('visualization_reportdensity_august_vs_january')
- a time series graph (question 4) ('report_development_august_vs_january')

# macro-assumptions
The assumptions made are the following: 
- CRS = EPSG:2056
- "around the lake" or "lakeside" = Kreise 1, 2, 8

# reproducing the environment
The software and libraries required to run the code successfully can be found in the environment.yml, see SDS210-PROJECT/environment.yml.

# usage
To successfully execute the project, the jupyter notebook can be run from top to bottom, code block per code block. 

# notebook structure
The code is structured in the following way:
- data imports for all 4 subparts are done at the beginning of the project
- each question is answered in a separate code block which comes with a markdown title including the question
- display(data.head()), print(data.head()) are deleted from the code as means of clarity, but can be inserted (and were conducted to check integrity of previous actions, check dtypes and crs, ...) where necessary
- not every line is commented, but some important comments are given