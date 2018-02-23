```
Title: Business & Environment Lecture
Author: John Fay
Date: Spring 2018
```

# Business &amp; Environment Demo

## CDP Demo

* Main site: https://data.cdp.net/

* Global 500 Emissions Data (2011):

  https://data.cdp.net/Companies/2011-Global-500-Emissions-and-Response-Status/cxp6-pzzb



### I. Online Visualization: *2011-Global-500-Emissions-and-Response-Status*

* Navigate to database: [Link](https://data.cdp.net/Companies/2011-Global-500-Emissions-and-Response-Status/cxp6-pzzb)

* **View** data: https://data.cdp.net/Companies/2011-Global-500-Emissions-and-Response-Status/cxp6-pzzb/data

* **Sort** data: on `Performance Band`

* **Filter** data: `Country is USA`

* **Visualize** data:

  * Column plot of `Mean` `Disclosure Score` by `country`
  * Histogram of `Disclosure score` 
  * Histogram of `Disclosure score` , filtered for `Counttry is USA`
  * Point Map of `Count of rows`

  ​


##### Review: 

* No need for additional software; all in browser (+)

* Low learning curve (+)

* Restricted to pre-packaged tools (-)

* Can't combine datasets (what about 2012, 2013?) (-)

  ---


### II. Download data; use Excel

* Export as CSV ([link](https://data.cdp.net/api/views/cxp6-pzzb/rows.csv?accessType=DOWNLOAD))

* Open in Excel...
  * **Sort** data: on `Performance Band`
  * **Filter** data: `Country is USA`
  * **Aggregate** data (Pivot Tables)
    * Mean `Disclosure Score` by `Country`
      * Add `Permission` as sub column
    * Set `Permissions` as row
  * **Visualize** data:
    - Column plot of `Mean` `Disclosure Score` by `country`
    - Histogram of `Disclosure score` 
      - Set bins to "5"
    - Histogram of `Disclosure score` , filtered for `Counttry is USA`

  ---

### III. Download data: use Python & Pandas

[Link to notebooks](http://nbviewer.jupyter.org/github/DataDevils/Feb23/tree/master/)

* Fire up Jupyter notebooks

* Navigate to `CDPDemos` folder

* **01-ExploreData**

  * Read in CSV file as a dataframe
  * Sort
  * Filter
  * Aggregate
  * Plot
    * Bar plot of mean `Disclosure score` by `country`
    * Box plot of `Disclosure score` by `country`
    * Histograms of `Disclosure score`: All and USA only

* **02-FetchData**

  * Bypass the step of downloading the data

* **03-FetchData-API**

  * Better control of how and what data are fetched

* **04-Merging-Data**

  * Combine multiple years of data

  ---

### IV. Other examples

* **GettingData**
  * 04-Grabbing HTML tables
* **UsingAPIs**
  * 2-Exploring the BISON API
  * 4-Geocoding with OSM
  * 4a-Geocoding with OSM in bulk
* **WaterDemos**
  * 01-WaterFlow Terse
  * 05-Flood Frequency Analysis
  * 08-Show All Sites

