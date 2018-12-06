# **Submit Metadata**

The second method will be to create a better submissions mechanism where you would be able to submit a metadata file of type either an **xml** or **json** file and I will work on increasing the format and types of files it can read and parse.

Some images ,may not have metadata files but you may still want some metadata during ingestion to be added to it for example number of bands, rows and columns, minima and maxima for the image and so on. GDAL gives us a simple read that allows us to read these stats and create a manifest file from that, this is also useful if there are additionla information in GeoTIFF headers embedded in the imagery.

*This feature will be made available to you using a tool that you can run at your end and avoid the need to upload large images.*
