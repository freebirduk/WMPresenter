# WeatherManager

>**Nothing to see here yet!**
>
>This project is very early in development. The details below show what is to come.

Weather Manager is a suite of programs to download, store and display Personal Weather Station (PWS) data from the 
Weather Underground (WU) website and, later to analyse that historical data. Why bother? WU after all stores your data and has some really useful tables and charts much of which is free. The reasons are these:

- We don't know what will happen to the data in the future. IBM may dump the WU product. The data may get watered down or always charged for or pricey. We just don't have control.
- The data retention period on WU is short for the free or cheap options. 
- The analytics are good but may not be all you want.

So Weather Manager provides, or will later provide:

- A library to access the WU API and retrieve your PWS data.
- A data repository library that defines and manages access to your own database. Currently, this is coded to access 
  a MariaDB(MySQL) database but could easily be changed to address any other type of store. The data model is 
  very simple at present. A table of observation rows and a general settings table. This will grow to include things 
  like the wettest day, the highest average May temperature etc.
- A console app designed to run periodically that will handle the retrieval and storage of the most recent 
  observations.
- A weather dashboard with tables, graphs and aggregates from the current data. This may be a desktop app, a 
  website or both. 

##WMPresenter

This repository reviews all the data already downloaded from Weather Underground, analyses it and creates a range of displays. These are:
- Current conditions
- Analyis of a particular data type over a time range e.g. air pressure for 2021-2022.
- Records of extremes e.g. higest ever recorded temperature
