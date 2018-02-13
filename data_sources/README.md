# What are SOCIB data-sources?

SOCIB data-sources corresponds to the so-called 'deployments'. In oceanography, 'deployments' are instrument&platform enssembles deployed (placed or released) to retrieve data from the ocean. During the time period a given deployment (unique instrument&platform enssemble) is active, the data measured by it is said to belong together and it is stored in the same netCDF to be later distributed in THREDDS. SOCIB API data-source endpoint allows a quick access to the data collected by a deployment.


SOCIB data-sources ENPOINT gives users a quick way to go trough all deployments and ask for those only meeting specific values by using the socalled ENDPOINT 'PARAMS':

    initial_datetime
        UTC time as YYY-MM-DDTHH:MM:SS 

    end_datetime
        UTC time as YYY-MM-DDTHH:MM:SS 

    standard_variable
        Any value of those returned by /standard-variables/ ENDPOINT 

    bbox
        Area where a given deployment has been operating since deployed (released or placed). Area should be specify as a 4 comma-separated float numbers following the structure: min. lat., max. lat., min. lon., max. lon 

    platform_type
        Any value of those returned by /platform-types/ ENDPOINT 

    instrument_type
        Any value of those returned by /instrument-types/ ENDPOINT 

    data_type
        Any value of those returned by /data-types/ ENDPOINT 

    status
        Two posibilities: active or completed 

    platform_name
        Any string within a deployment name 

    description
        Any string within a deployment description 


This way, someone can ask for deployments involving certain platforms or instruments that ocurred in a defined time window (initial_datetime, end_datetime) and area (coverage_bounding_box). In addition to the above options, SOCIB data-sources ENPOINT enables also to look for specific standard variables (additional PARAM) by doing on its own a quick check of a given data-source (deployment) 'entries'. Once the deployments are found, users can either rely on THREDDS to view, download or access their associated netCDFS ('entries') or rely on SOCIB API again to directly retrive its data with several resampling methods. 

See:
* Find your deployment. [Example 1: /data-source/ ENPOINT & PARAMS](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/finding_your_data_source.ipynb)
* Explore your deployments's netCDFs (THREDDS services).[Example 2: Exploring deployments's netCDFs and THREDDS services available for those](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/working_with_data_sources_netcdfs.ipynb). 
* Access deployment's data. [Example 3: /data-source/{id}/data ENPOINT & PARAMS](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/straightforward_data_access_for_data_sources.ipyn)

# Who is addressed to?

Anyone interested in exploring SOCIB data archiving can use the API, that is, researchers for finding the data that better suit their study-cases or developers interested in integrating SOCIB data on its products.  