# Reducing-Traffic-Mortality-in-the-USA

<img src="images/../Data/images/car-accident.jpg" >

We analyze data collected by the National Highway Traffic Safety Administration and the National Association of Insurance Commissioners to wrangle, plot, dimensionally reduce and cluster data to make an attempt to find patterns and help reduce Traffic Mortality in USA.

### Datasets

there are two datasets : **miles-driven.csv** , **road-accidents.csv**

#### Install the requirements

> - Install the pandas library using command pip install pandas.
> - Install the numpy library using command pip install numpy.

```import pandas as pd```

```import numpy as np```

```import matplotlib.pyplot as plt```

Our dataset **road-accidents.csv** show this :




|    | state      |   drvr_fatl_col_bmiles |   perc_fatl_speed |   perc_fatl_alcohol |   perc_fatl_1st_time |
|---:|:-----------|-----------------------:|------------------:|--------------------:|---------------------:|
|  0 | Alabama    |                   18.8 |                39 |                  30 |                   80 |
|  1 | Alaska     |                   18.1 |                41 |                  25 |                   94 |
|  2 | Arizona    |                   18.6 |                35 |                  28 |                   96 |
|  3 | Arkansas   |                   22.4 |                18 |                  26 |                   95 |
|  4 | California |                   12   |                35 |                  28 |                   89 |

The columns are:

* drvr_fatl_col_bmiles = Number of drivers involved in fatal collisions per billion miles (2011).

* perc_fatl_speed = Percentage Of Drivers Involved In Fatal Collisions Who Were Speeding (2009).

* perc_fatl_alcohol = Percentage Of Drivers Involved In Fatal Collisions Who Were Alcohol-Impaired (2011).

* perc_fatl_1st_time = Percentage Of Drivers Involved In Fatal Collisions Who Had Not Been Involved In Any Previous Accidents (2011).
  

Ensuite, on utilise ````.describe``` to return the description of the data and to view some basic statistical details like percentile, mean, std etc. we observe this:

|       |   drvr_fatl_col_bmiles |   perc_fatl_speed |   perc_fatl_alcohol |   perc_fatl_1st_time |
|:------|-----------------------:|------------------:|--------------------:|---------------------:|
| count |                51      |          51       |            51       |             51       |
| mean  |                15.7902 |          31.7255  |            30.6863  |             88.7255  |
| std   |                 4.122  |           9.63344 |             5.13221 |              6.96011 |
| min   |                 5.9    |          13       |            16       |             76       |
| 25%   |                12.75   |          23       |            28       |             83.5     |

## Graphical summary of the data

The graphical overview is good to get a sense for the distribution of variables within the data and could consist of one histogram per column. It is often a good idea to also explore the pairwise relationship between all columns in the data set by using a pairwise **scatter plots**

The result is like this :

<img src="images/../Data/images/téléchargement.png" >

