## Usage

[Open Source MANO](https://osm.etsi.org/docs/user-guide/) must be installed to deploy the descriptors.  Please refer to
OSM's [documentation](https://osm.etsi.org/docs/user-guide/03-installing-osm.html) to get started.

Once OSM has been set up correctly, add the repo as follows:

    osm repo-add --type osm 5gmeta-osm https://raw.githubusercontent.com/5gmetadmin/vnfdescriptors/main/descriptors/repository

If you had already added this repo earlier, you can run `osm repo-list` to check the existing repositories.
