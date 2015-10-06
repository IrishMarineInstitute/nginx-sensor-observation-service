#nginx OGC Sensor Observation Service#
This repository provides an example nginx configuration with some additional
scripts and files to allow a basic [Open Geospatial Consortium][1] [Sensor 
Observation Service][2] to be deployed against sensors outputting data to a URL.
##Table Of Contents##
 1. [Requirements](#requirements)
 1. [Installation](#installation)
 1. [Usage](#usage)
 2. [Acknowledgements](#acknowledgements)
 1. [To Do](#to-do)
 
##Requirements##
1. [Lua][4] should be available on the system path to handle firing off requests from nginx to the shell
1. [cUrl][5] is needed for fetching remote JSON files
1. [nginx][3] to act as the web server, with the [ngx_lua][6] package installed

##Installation##
Download the package from GitHub and unzip to /nginx-sensor-observation-service

If a different directory is used, the paths within the nginx configuration file will need to be edited.
##Usage##
Start an nginx instance using the ./conf/sensor-observation-service.conf configuration file

The index.html page contains links to a number of example calls using the Sensor Observation Service.
##Acknowledgements##
The [Lua JSON][7] library by Jeffrey Friedl is used within this configuration.

## To Do##

See open [TODO issues][9].

[1]: http://www.opengeosptial.org
[2]: http://www.opengeospatial.org/standards/sos
[3]: http://nginx.org/en/download.html
[4]: http://www.lua.org/
[5]: http://curl.haxx.se/
[6]: https://www.nginx.com/resources/wiki/modules/lua/
[7]: http://regex.info/blog/lua/json
[8]: https://stedolan.github.io/jq/
[9]: https://github.com/IrishMarineInstitute/nginx-sensor-observation-service/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+TODO
