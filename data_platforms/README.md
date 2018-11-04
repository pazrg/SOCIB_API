# What are SOCIB data-platforms?

SOCIB data-platforms wrapp data-sources sharing the same platform which enables then a quick recovery of the latest or historical data comming from a specific platform (particularly useful in case of long-term platform-based monitoring). 

A certain SOCIB data-platform can be composed then by a single data-source (i.e only one deployment has been performed with it) or serveral (i.e more than one deloyment has been perfomed with it). 

Examples of long-term platform-based monitoring are the contonous monitoring performed SOCIB fixed-stations (HFRadar, Ocenographic buoys, Sea Level stations, Weather Stations etc) or other platforms recurringly deployed (ie SOCIB gliders involved in 'CANALES' missions). 

<br><br>
<img src="https://github.com/socib/API_examples/raw/master/images/SOCIBfixed_station.jpg">


SOCIB data-platforms constitute the first level of abstraction build over the data-sources, being the second one the so-called SOCIB data-products.


See here how to use it:

- What is a data-platform? ([Example 6](https://github.com/socib/API_examples/blob/master/data_platforms/what_is_a_data_platform.ipynb))

- Searching for certain data-platform ([Example 7](https://github.com/socib/API_examples/blob/master/data_platforms/searching_for_certain_data_platform.ipynb)) by coverage_bounding_box, type, status, instrument, platform, initial_time, end_time, processing levels etc.

- Requesting a data-plaform's historical files ([example 8](https://github.com/socib/API_examples/blob/master/data_platforms/requesting_a_data_platforms_historical_files.ipynb))

- Requesting a data-plaform's latest files ([example 9](https://github.com/socib/API_examples/blob/master/data_platforms/requesting_a_data_platforms_latest_files.ipynb))


# Who is addressed to?

Anyone interested in exploring SOCIB data archiving can use the API, that is, researchers for finding the data that better suit their study-cases or developers interested in integrating SOCIB data on its products.  