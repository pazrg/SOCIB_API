
<img src="/images/bg-masthead3.jpg" alt="SOCIB">

# What is SOCIB API?

API stands for Application Programming Interface. An API is basically a programmatic tool that is used to interact with a system. More specifically, the new SOCIB API offers the possibility of discovering our data catalog and retrieving the data it contains. This API is a REST API, which means that the requests are issued with an usual HTTP client (available with any programming language). 

# What's new?

One of the main new features is the possibility of discovering and retrieving data without temporal restrictions, unlike Data Discovery API, that only lets you retrieve the latest 60 days of data, at most. Also important is that the data can be filtered with new sets of criteria and retrieved with several resampling methods. 

Gridded data type is now also supported (currently only for HF Radar data). Another important breakthrough has been achieved introducing the concept of "data products", that let us provide grouped data in almost any way. The API also supports authentication via API keys, so the tracking of users will now be possible (it was not with the old one). 

Finally, in future releases the new API will allow responding with new data types such as operational data models or even media data.

# Who is addressed to?

The new SOCIB API is addressed to two different types of users: the IT (software developer) user and the data scientific user. For the IT expert, the use will be almost trivial. For  scientific data experts, with no experience on this kind of tool, some training will be needed. 

A success story is the development of the SOCIB Data Catalog web that fully relies on the capacity of this API, that will be published on the new SOCIB website.

# API examples (python notebooks)

* [Quick start](https://github.com/pazrg/SOCIB_API/blob/master/tips/quick_start.ipynb) - SOCIB API main concepts

* [SOCIB data-sources](https://github.com/pazrg/SOCIB_API/tree/master/data_sources):

	- What is a data-source? ([Example 1](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/what_is_a_data_source.ipynb))

	- Searching for certain data-sources ([Example 2](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/searching_for_certain_data_sources.ipynb))

	- Requesting a data-source's data ([example 3](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/requesting_a_data_sources_data.ipynb))

	- Subsetting a data-source's data: by time-range, by elevation-range and by bounding-box ([example 4](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/subsetting_a_data_sources_data.ipynb))

	- Resampling a data-source's data: ([example 5](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/resampling_a_data_sources_data.ipynb))
 
* [SOCIB data-platforms](https://github.com/pazrg/SOCIB_API/tree/master/data_platforms):
	- What is a data-platform? ([Example 6](https://github.com/pazrg/SOCIB_API/blob/master/data_platforms/what_is_a_data_platform.ipynb))

	- Searching for certain data-platform ([Example 7](https://github.com/pazrg/SOCIB_API/blob/master/data_platforms/searching_for_certain_data_platforms.ipynb)) by coverage_bounding_box, type, status, instrument, platform, initial_time, end_time, processing levels etc.

	- Requesting a data-plaform's historical files ([example 8](https://github.com/pazrg/SOCIB_API/blob/master/data_platforms/requesting_a_data_platforms_historical_files.ipynb))

	- Requesting a data-plaform's latest files ([example 9](https://github.com/pazrg/SOCIB_API/blob/master/data_platforms/requesting_a_data_platforms_latest_files.ipynb))

* [SOCIB data-products](https://github.com/pazrg/SOCIB_API/tree/master/data_products):
	- What is a data-product? ([Example 9](https://github.com/pazrg/SOCIB_API/blob/master/data_products/what_is_a_data_products.ipynb))

	- Searching for certain data-products ([Example 10](https://github.com/pazrg/SOCIB_API/blob/master/data_products/searching_for_certain_data_products.ipynb))

	- Requesting a data-product's data ([example 11](https://github.com/pazrg/SOCIB_API/blob/master/data_products/requesting_a_data_products_data.ipynb))


# Legacy
This material has been developed by [Paz Rotllan](https://github.com/pazrg). Email: protllan@socib.es

# Copyright
Copyright (c) 2017 ICTS SOCIB - Servei d'observació i predicció costaner de les Illes Balears.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
