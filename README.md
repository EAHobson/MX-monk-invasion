# MX-monk-invasion

This repository contains the data we used in analyses in our paper "History of nonnative Monk Parakeets in Mexico", which will be published in PLOS ONE. Below, we summarize each of the datasets and provide information on how we accessed them.

Citation for published paper: Hobson, E., Smith-Vidaurre, G., Salinas-Melgoza, A. "History of nonnative Monk Parakeets in Mexico". [full citation to be updated on publication]

DOI for dataset: [![DOI](https://zenodo.org/badge/97489648.svg)](https://zenodo.org/badge/latestdoi/97489648)

## CITES International trade data (cites_imports.csv)

We requested data on importation of Monk Parakeets from CITES (the Convention on International Trade in Endangered Species of Wild Fauna and Flora) trade statistics derived from the CITES Trade Database, UNEP World Conservation Monitoring Centre, Cambridge, UK (data available at https://trade.cites.org/, accessed 2017-02-28).

We requested data for: 

Years = 1975-2016 (all available years)
Exporting countries = "All Countries"
Importing countries = "Mexico"
Source = "All Sources"
Purpose = "T - Commercial"
Trade terms = "LIV - live"
Search for genus = "Myiopsitta"

Please see https://trade.cites.org/cites_trade_guidelines/en-CITES_Trade_Database_Guide.pdf for a description of some of the idiosyncrasies and limitations of CITES trade data.

## Mexico DGVS trade data (dgvs_imports.csv)

Because of some of the idiosyncrasies of the CITES trade data, we also obtained data directly from the Mexican authorities on importation numbers for Monk Parakeets. We requested data from the Dirección General de Vida Silvestre (DGVS) through the Instituto Nacional de Transparencia, Acceso a la Información y Protección de Datos Personales with request number 0001600402116. DGVS data are reported at the shipment level and include import records from 2000-2015. 

## Citizen science observations (citizen_science_reports.csv)

This dataset includes observations of Monk Parakeets observed in Mexico, reported by citizen scientists, and aggregated on GBIF and eBird (see 'Methods' section in paper for more details). 

We cleaned these data and deleted obvious double-reporting events (i.e. if the same person reported an observation at the same location and date/time to more than one citizen science reporting databases). Based on the location of the observation, we assigned each report to a city/town. We excluded any reports without date/time or location information.

## Other supporting data files

cities.frLIT.csv = list of cities for which there are scientific reports of sightings

LIT_citationMASTER.csv = list of all sources of scientific reports of sightings

LIT_locationsXyears_citations_TRIMMED.csv = list of all scientific reports of sightings by city and year

MEX_adm1.rds = shape files for Mexican states (available here: http://www.gadm.org/download -- level 1)

mx.states.attributes.txt = attributes of Mexican states

state.names.csv = names of Mexican states, with and without accents (for matching to Mexican state shapefiles)

reg7.master.csv = attributes of each geographic region (for plotting by color, etc.)

Rmkd-final.rmd = R Markdown file of all analyses and plots for the paper

Rmkd-final.html = knitted output of Markdown file


