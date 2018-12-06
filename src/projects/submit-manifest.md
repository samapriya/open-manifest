# **Submit Manifest**

For now there are two ways of getting a manifest added to the library. For this setup you are submitting a manifest that you created. This can be an empty field manifest or an example manifest that is filled with example values.

For example a PlanetScope 4Band Analytic Manifest looks like this. Here you will notice that I have added band names as simply b1, b2 and so on but you can modify this to be "Red","Green","NIR" and so on as needed. This is an example of an empty manifest though I have filled in the bandnames for ease.You can submit this as a file so we can verify and upload.

``` js
data_ps4b={"id": "","bands": [{"id": "b1"},{"id": "b2"},{"id": "b3"},{"id": "b4"}],"missingData": {"value": "0"},"properties": {"system:time_start":"","product_type":"","orbit":"",
"provider":"","instrument":"","satellite_id":"","number_of_bands":"","epsg_code":"","resampling_kernel":"","number_of_rows":"","number_of_columns":"","gsd":"",
"cloud_cover":"","incidence_angle":"","sun_azimuth":"","sun_elevation":"","azimuth_angle":"","spacecraft_angle":"","radiometric_scale_factor":"","reflectance_coefficient_b1":"",
"reflectance_coefficient_b2":"","reflectance_coefficient_b3":"","reflectance_coefficient_b4":""},"tilesets": [{"sources": [{"primaryPath": ""}]}]}
```

#### Steps Involved

- Get the metadata file that you are using to parse the manifest, and then extract fields to be used for the manifest.
- You can email me to be added as a collaborator or simply email me the manifest file and I will attribute you as contributer of said manifest

*Note*: *All manifest that are submitted are user contributed and are in no way inclusive of all fields in the manifest. The license allows you to modify and extend the manifests as necessary.*
