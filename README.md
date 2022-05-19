# Datasets for SmartSense
These datasets are used in the implementation of SmartSense (submitted to CIKM 2022).

## Datasets
We open-source Samsung Bixby Dataset, the dataset for action recommendation for smart home.
Our dataset is composed of log datasets, routine datasets, and dictionary for each dataset.
Log datasets are collected for a month from 4 different countries: Korea, the USA, France, and Spain, respectively.
Routine datasets are collected from 3 different regions: Asia-Pacific, North America, and Europe, respectively.
Dictionaries provide look-up tables for ids of context and device control information in both kinds of datasets.
### Log Datasets
Each log dataset is a tensor size of ![formula](https://render.githubusercontent.com/render/math?math=\N\times\10\times\4), where ![formula](https://render.githubusercontent.com/render/math?math=\N) is the number of instances.
Each instance of log datasets contains ten consecutive actions performed by a user of Bixby service.
Each action of instances is represented as a vector of length 4.
Elements of a vector represent a weekday, a timerange, a device, and a device control in order.
### Routine Datasets
A routine is a sequence of device controls triggered by a predefined condition or a request from a user.
Routines of our datasets are submitted by users of SmartThings service.
Each line of routine datasets is a sequence of devices in a routine.
There are two versions of routine datasets collected from Europe since the device ids of the France dataset and the Spain dataset are different.
### Dictionaries
Dictionaries define the ids of weekdays, timeranges, devices, and device controls.
