# Maybms

Maybms was an interesting research outcome to build a probebalistic db system on top of postgres. 

Unfortunatelly there are no docker images available of the original system build. The original Dockerfile pulled from Ubuntu 12.04 and the repos no longer resolve. 

In this repo I updated the Dockerfile to pull from 16.04, the system compiled but the conf() function in the HelloWorld example throws an error. Uncommenting the error condition reveals that postgres cannot perform a proper aggregation with this function, but this is as far as I went with troubleshooting this issue.
