# 2019 Bay Area Flight Data Exploration
This visual exploration uses data from the [Bureau of Transportation Statistics](https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp), which tracks the on-time performance of US domestic flights as well as the causes of any delays. For this exploration, I have downloaded CSV files from the [Bureau of Transportation Statistics website](https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236) and narrowed down the dataset to 2019 departures and arrivals at Bay Area airports, which include SFO (San Francisco International Airport), SJC (Norman Y. Mineta San Jose International Airport), and OAK (Oakland International Airport). I then use the data to provide guidance on:

- Which Bay Area airport to choose
- What time to fly
- Which carrier to choose
- Which location outside of the Bay Area to fly to or from

In total, the dataset consists of 286,933 departures from and 286,766 arrivals into Bay Area airports. The main features of interest that are used to provide guidance are arrival delay, cancellations, and diversions.

# Requirements
- Jupyter Notebook
- Numpy
- Pandas
- Matplotlib
- Seaborn
- os
- Datetime

# Installation
To get the Jupyter Notebook running, execute the following in the command line and select `bay_area_flights.ipynb` from the Jupyter Notebook dashboard. The conda environment setup is optional; I have provided the base environment in `base.yaml`.

```
$ git clone https://github.com/evanchen13/bay-area-flights.git
$ cd bay-area-flights
$ conda env create -f base.yaml
$ jupyter notebook
```

Also note that the data CSV files, provided in `data.zip`, will need to be unzipped.

# Slides
Summary slides on the findings from this data exploration can be found at `bay_area_flights_slides.slides.html`. To generate the slides from `bay_area_flights_slides.ipynb`, be sure to also download `output_toggle.tpl` and execute the following in the command line:

```
$ jupyter nbconvert bay_area_flights_slides.ipynb --to slides --post serve --template output_toggle
```

# License
The contents of this repository are covered under the [GNU General Public License v3.0](https://github.com/evanchen13/bay-area-flights/blob/main/LICENSE).
