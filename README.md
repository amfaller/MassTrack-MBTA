# 🚃 MassTrack: MBTA 🚃
Author: Tony Faller (af3370@columbia.edu)

## Description
MassTrack is a privacy project developed across two seminars at Columbia University:
* COMS E6156 Topics in Software Engineering (Professor Gail Kaiser)
* COMS E6998 Private Systems (Professor Roxana Geambasu)

This repository contains the Jupyter notebook corresponding to **COMS E6156**, focusing on examining privacy vulnerabilities in publicly-available MBTA (Massachusetts Bay Transportation Authority) data -- specifically, analyzing pseudo-identifiers which may compromise user privacy.

## Threat Model
This project assumes an adversary who knows:
* The T station a person left from
* The timestamp at which this person departed the station
* How long this person spent in transit

It was hypothesized that this information, when used in conjunction with the public MBTA dataset, could be used to reconstruct a station-to-station journey. This would mean that the adversary could determine exactly where a person travelled to.

## Dataset
The scope of this analysis is limited to the MBTA's Green Line trains.

The data is available via:
* Zenodo mirror [https://zenodo.org/records/15121997](https://zenodo.org/records/15121997)
* Official MBTA source (includes data dictionary): [https://mbta-massdot.opendata.arcgis.com/datasets/0b4dc16b8b984836962229865d5b573b/about
](https://mbta-massdot.opendata.arcgis.com/datasets/0b4dc16b8b984836962229865d5b573b/about)

Please note that this dataset is rather large (a 1.3GB .zip file). Extracting & processing locally may require significant system resources.

## Reproduction
The Jupyter notebook can be imported to Google Colab natively (there is a link within the notebook in this repository), or otherwise run locally. It is not advised to run locally unless sufficient memory resources are available.

Findings, explanation, and discussion are contained within the notebook itself. A link to the final report of this project will be provided once it is available.
