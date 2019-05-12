# Insight into AirBNB Boston Data

## Table of contents

- [Installation](#installation)
- [Motivation](#motivation)
- [Project Structure](#project-structure)
- [Results](#results)
- [References](#references)


## Installation

In order to execute the Jupyter Notebook you should have **Anaconda 4.5.11** and **python 3.6.6** installed. 
The notebook needs scikit-learn, matplotlib, numpy and pandas libraries. These are available as part of Anaconda installation and don't need any additional installation.

Clone the repo: `git clone https://github.com/kvsrohit/AirBNB-Boston.git`

## Motivation
A quick glance at [AirBnB Boston data][1]<sup>1</sup> arouse curiosity to see if following questions can be convincingly answered using data analysis.

- What are hot locations?
- What are peak seasons?
- Does number of properties in neighbourhood affect the occupancy?
- What are the factors affecting overall occupancy and review ratings?

## Project Structure

```text
AirBNB-Boston/
├── airbnb-boston-report.html
├── README.md
├── src/
|   └── airbnb-boston.ipynb
└── inputs/
    ├── calendar.csv
    ├──	listings.csv
    └── reviews.csv
```

- airbnb-boston-report.html ==> Generated report from notebook
- airbnb-boston.ipynb ==> Notebook to investigate Airbnb data for year 2016 in Boston.
- calendar.csv         ==> Booking information of houses in Boston.
- listings.csv         ==> Information of properties on offer in Boston.
- reviews.csv          ==> User reviews for listings 

## Results
- There are few neighbourhoods that show higher occupancy compared to others. However, there are no standouts by great margin
- September and October appear to be peak seasons. However, any conclusion on this needs analysis of data over years.
- Poor correlation between number of properties in a neighbourhoood and occupancy rate. No conclusive evidence to suggest over supply of properties in any neighbourhood.
- Prominant features deciding occupancy
  - Property type seems to be most important feature that renters look for with special preference to Villa and appartments
  - This is followed by bed type with high negative weights for air-beds and couches.
- Prominant features deciding review ratings
  - Host Response Time showed up as most important feature deciding the review ratings. Possibly due to the first impression effect.
  - This was followed by property type and cancellation policy.



## References
1. https://www.kaggle.com/airbnb/boston 
1. https://airbnb.com

[1]: https://www.kaggle.com/airbnb/boston "AirBnB Boston data @ Keggle"
[2]: https://airbnb.com "Airbnb"
