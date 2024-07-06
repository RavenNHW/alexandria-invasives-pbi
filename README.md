# Visualizing Invasive Species in Alexandria 
Project by Raven Welch | [LinkedIn](https://www.linkedin.com/) | [Email](mailto:ravennhwelch@gmail.com)

---

### ReadMe Navigation
[Sources](#Sources) | [Overview](#overview) | [Goals](#goals) | [Reproduction](#reproduction) | [To-do](#to-do) 

### Repo Navigation
```
├── images: contains all images used in the project
├── gbif_data.zip: ZIP download from GBIF.org
│   └── verbatim.txt - Data used
│
├── data_cleaning.ipynb
│
├── cleaned_inat_data.csv
│
├── README.md
│
└── AlexandriaInvasiveSpecies.pbix
```
---

## Sources
This data is pulled from the [iNaturalist Occurence Dataset](https://doi.org/10.15468/ab3s5x), using data from [iNaturalist](https://www.inaturalist.org/) and distributed by [GBIF](https://doi.org/10.15468/ab3s5x)

iNaturalist is a nonprofit organization that helps provide an avenue for citizen science by allowing users to upload images or soundbytes of any living thing on earth, with the community being able to help identify those lifeforms to the best of their ability. Once a certain criteria has been met - enough consensus on what the observation is - it gets marked as research grade, which can then be used by organizations to help ensure a higher likelyhood that the data is as accurate as possible. While it's not reccomended to download large amounts of data directly from iNaturalist, you can use sources like GBIF which keeps an up to date record of research-grade observations from iNaturalist.

## Overview

This project was inspired multiple factors - that Alexandria lacks programs to help properly manage invasive species spread, the fact that many people may be unaware of the extent of the problem, my own interest in native and invasive plants, and my own interest in the actual data. I felt it would be interesting to see the distribution of a few key invasive plants. While there are many to choose from, I selected three plants with similar issues. Porcelain berry, English Ivy, and Kudzu are all vining plants that have a tendency to completely smother native plants and spread aggressively. 

## Goals

As I expand this project, I want to hit a few goals while doing so:
- Better inform people about the different invasive species presented, and why they should care
- Encourage more people to sign up for iNaturalist and help contribute to the ever-expanding dataset
- Focus on accessibility - Ideally this should be readable by many people, with consideration taken towards multiple types of color blindness, screen readers, and other eyesight issues.

## Reproduction
If you just want to run the .pbix locally as-is, open [AlexandriaInvasiveSpecies.pbix](AlexandriaInvasiveSpecies.pbix), edit the query by going to "Transform Data" on the ribbon, and editing the "source" step in the "inaturalist" query with the full filepath containing [cleaned_inat_data.csv](cleaned_inat_data.csv)

If you want to run the full project including cleaning the data, you will need to be able to run jupyter notebooks and have pandas installed in your python environment. 
Unzip [gbif_data](gbif_data.zip), open [data_cleaning.ipynb](data_cleaning.ipynb) in jupyter, and then follow the same steps above. The python will automatically save the cleaned data in the gbif_data folder. 

## To-Do
This to-do list is not exhaustive and will evolve as I complete further analysis and incorporate feedback

- [ ] Set tab order for main page
- [ ] Create Alt Text for all visuals
- [ ] Create in depth individual pages explaining each invasive plant 
	- [ ] English Ivy
    - [ ] Kudzu
    - [ ] Porcelain Berry
- [ ] Create detailed writeup of process 
    - [ ] The problem at hand
    - [ ] Chart Selection, Colors, and More 
    - [ ] Considerations, Data Accuracy, and Gaps in Data
    - [ ] How could this be used, how is it helpful?
