# Who are the best teams and the best players in Euroleague and NBA since 1958?

The objective of this project is to obtain a dataset for its subsequent enrichment either by using an API or by web scrapping techniques. In this case we have opted for the latter since the objective is none other than to obtain some data on the best players and the best teams in the history of basketball by gathering data from both competitions. In turn, we will use and synthesize the code as much as possible by using separate functions. At a later stage, we will illustrate our 'insides' in a correct way by using libraries like seaborn or matplotlib.


![Image text](https://s03.s3c.es/imag/_v0/770x420/b/1/6/770x420-michael-jordan-air-jordan.jpg)

## Table of Contents
1. [General Info](#general-info)
2. [Data treatment](#Data-treatment)
3. [Libraries](#Libraries)
4. [Technology](#Technology)
5. [Methodology](#Methodology)

## General Info

In this analysis * -


## Data treatment

The realization of the project is divided into up in 3 parts: 
1. Cleaning of a dataset. 
2. Web scrapping to obtain and complete the first dataset. 
3. Visualization of the data obtained in section 1 and 2 by using the seaborn and matplotlib library. 


## Libraries
***
A little intro about libraries. 
```
import beautiful soup
import pandas as pd
import numpy as np
import re
import matplotlib.pyplot as plot
import src.funciones as fun
import seaborn as srs

```

## Technology: 

A list of technologies used within the project:
* [Jupyter Notebook](https://jupyter.org/) : Version 6.1.4
* [Python](https://www.python.org/): Version 3.8
* [Visual Studio Code](https://code.visualstudio.com/)

## Methodology: 

The realization of the project is divided into up to 4 parts: 
1. Preliminary cleaning of the dataset and exploratory analysis of the dataset: 
* use of some functions to detect anomalies in the dataset (.valuecounts, .shape, .isnull.sum).
* use of other functions to remove null values (dropna. (tresh),df.drop....)
* substitution of some values by using the replace function
* reset.index 

2. Cleaning of the dataset according to the hypotheses and extraction of up to 3 new data tables.

        * Cleaning of the Activity column
- use of regex to preserve only the gerunds of the activity
- creation of new column to transfer these gerunds
- assignment of values by creating a dictionary to split the activities according to the movement
- elimination of rows with null values in the column of interest.

        * Cleaning of the Fatal column
- standardization of values in Yes, No, Unknown using the replace function. 
- elimination of lines with no value in this section. 
- parallel cleaning of the Activity column in order to be able to relate both in subsequent graphs.
- renaming of columns for further manipulation
- discarding columns using the drop function

        * Cleanup of the Country column
- use of the above to list the Country column next to the Fatal column. 

3. Visualization of the data obtained in section 2 by using mainly the seaborn library.
- sns.catplot
- sns.kdeplot
- sns.histplot
- sns.stripplot
- use of the where function for some data changes. 

4. Conclusions according to the hypotheses


## Authors

* **Luis Sánchez de León** - *Initial work* - (https://github.com/lsdl3)




