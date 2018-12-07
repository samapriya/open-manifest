# **Manifests in Earth Engine**

Once you have a manifest, you can now build a custom ingestor that will allow you push datasets based assets and your metadata. This can be achieved by changing the primary Path and point it to the gs:// image and add the metadata values.

``` js hl_lines="5"
data_ps4b={"id": "","bands": [{"id": "b1"},{"id": "b2"},{"id": "b3"},{"id": "b4"}],"missingData": {"value": "0"},"properties": {"system:time_start":"","product_type":"","orbit":"",
"provider":"","instrument":"","satellite_id":"","number_of_bands":"","epsg_code":"","resampling_kernel":"","number_of_rows":"","number_of_columns":"","gsd":"",
"cloud_cover":"","incidence_angle":"","sun_azimuth":"","sun_elevation":"","azimuth_angle":"","spacecraft_angle":"","radiometric_scale_factor":"","reflectance_coefficient_b1":"",
"reflectance_coefficient_b2":"","reflectance_coefficient_b3":"","reflectance_coefficient_b4":""},
"tilesets": [{"sources": [{"primaryPath": ""}]}]}
```

Once you modify this to include the metadata and image path, and write this to a JSON file you can simply use the **```earthengine upload_manifest```** tool to upload the image.

**```
earthengine upload_manifest "full path to your manifest json file"
```**

A universal ingestor would allow us to
- use these manifests as plug and play to ingest imagery along with metadata.
- This will also allow users to modify manifests to create metadata for images that have already been ingested.
