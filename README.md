# 🚃 MassTrack: MBTA 🚃
Author: Tony Faller (af3370@columbia.edu)

## Description
MassTrack is a privacy project developed across two seminars at Columbia: COMS E6156 Topics in Software Engineering with Professor Gail Kaiser, and COMS E6998 Private Systems with Professor Roxana Geambasu. This repository contains the Jupyter notebook corresponding to COMS E6156.

In this class, I am examining publicly-available MBTA data for privacy vulnerabilities relating to pseudo-identifiers.

## Threat Model
Assume an adversary knows:
* The T station a person left from
* The timestamp at which this person departed the station
* How long this person spent in transit

It was hypothesized that this information, when used in conjunction with the public MBTA dataset, could be used to reconstruct a station-to-station journey. This would mean that the adversary could determine exactly where a person travelled to.

## Dataset
For simplicity, the scope of this project was limited to the MBTA's Green Line trains.

The data is located in a Zenodo repository located here: [https://zenodo.org/records/15121997](https://zenodo.org/records/15121997)

This is the same zip file available directly from the MBTA data repository (note: this also contains the data dictionary for this dataset): [https://mbta-massdot.opendata.arcgis.com/datasets/0b4dc16b8b984836962229865d5b573b/about
](https://mbta-massdot.opendata.arcgis.com/datasets/0b4dc16b8b984836962229865d5b573b/about
)
## Reproduction
The Jupyter notebook can be imported to Google Colab natively (there is a link within the notebook in this repository), or otherwise run locally. It is not advised to run locally; the target MBTA data is a .zip file which is already 1.3 GB large, and extracting this may overwhelm system RAM.

All findings and explanations are contained within the notebook. If one wishes to reproduce this project, one only needs to run all of the code cells contained in the notebook.
