## OpenDatacube implementation

### Utility scripts

* dhusget   : script to download whole datasets from scihub.copernicus.eu.

* s1prepare : script to prepare preproccessed images to be indexable through the datacube api

### Setup - Implementation so far

1. First configure the datacube [Datacube installation](https://github.com/ceos-seo/data_cube_ui/blob/master/docs/open_data_cube_install.md)
2. Define the product and the metadata through the use of the datacube api
3. Test the database with a simple jupyter notebook.

### Activation

* Run the script under /PATH_OF_YOUR_DATACUBE_INSTALLATION/datacube_env/bin/activate to get access to the virtualenv

### Problems - Observations

* The path of the images-bands is incorrectly annotated if the rasters are in a subfolder.

* Final yaml is saved as *agdc-metadata.yaml* on all inputs

* The preparation script requires rasters to be on a folder called *SENTINEL_1A* (configurable through the script).

### TODO

* Implement recursive folder search to correct annotate the rasters' path.
