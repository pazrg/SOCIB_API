# What are SOCIB data-products?

SOCIB Data-products are 'artifacts' created by SOCIB and represents either individual deployments (isolate deployments) or groups of deployments (deployments that share a certain context and therefore, certain features). Examples where deployments can be grouped together in major entities are same transect/point long-term monitoring (fixed-stations, glider missions etc) or multiplatform campaings (involving different platforms: gliders, drifters, turtles, vessels...). In these situations, different deployments (instruments & platforms enssembles) are sequencially performed in order to ensure a continous data-retrieval and referring to them as a whole (overlooking individual deployments) might become handy. 

SOCIB data-product ENPOINT gives users a quick way to go trough all data-products and ask for those whose deployments meet specific values by using the socalled ENDPOINT 'PARAMS':

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

    name
        Filters the products which contains the given text in its name or description (Case insensitive) 

    detail
        "full" or "summary" 


This way, someone can ask for those data-products composed by deployments involving certain platforms or instruments that ocurred in a defined time window (initial_datetime, end_datetime) and area (coverage_bounding_box). 


See:

    - What is a data-product? ([Example 6](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/what_is_a_data_product.ipynb))- UNDERDEVELOPMENT

    - Multiplatfrom campaings ([Example 7](https://github.com/pazrg/SOCIB_API/blob/master/data_products/oceanographic_campaings.ipynb))

    - Glider missions ([example 8](https://github.com/pazrg/SOCIB_API/blob/master/data_sources/glider_missions.ipynb)) - UNDERDEVELOPMENT

    - Fixed-stations ([example 9](https://github.com/pazrg/SOCIB_API/blob/master/data_products/fixed_stations.ipynb))

# Who is addressed to?

Anyone interested in exploring SOCIB data archiving can use the API, that is, researchers for finding the data that better suit their study-cases or developers interested in integrating SOCIB data on its products.  

