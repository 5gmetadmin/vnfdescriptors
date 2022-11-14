## Usage

[Open Source MANO](https://osm.etsi.org/docs/user-guide/) must be installed to deploy the descriptors.  Please refer to
OSM's [documentation](https://osm.etsi.org/docs/user-guide/03-installing-osm.html) to get started.

Once OSM has been set up correctly, add the repo as follows:

    osm repo-add --type osm --description "5GMETA OSM KNF and NS repository" 5gmeta-osm https://raw.githubusercontent.com/5gmetadmin/vnfdescriptors/main/descriptors/repository

If you had already added this repo earlier, you can run `osm repo-list` to check the existing repositories.

## Usefull comands:
    
    osm nfpkg-repo-list (list NF packages from OSM repositories)
    osm nfpkg-repo-show --repo 5gmeta-osm cits (shows a specific NF package in a repo)
    osm nfpkg-create --repo 5gmeta-osm cits (onboards a package from a repo into OSM)
    
    osm nspkg-repo-list (list NS packages from OSM repositories)
    osm nspkg-repo-show --repo 5gmeta-osm cits (shows a specific NS package in a repo)
    osm nspkg-create --repo 5gmeta-osm cits (onboards a package from a repo into OSM)

## Adding descriptors to the repository
    
To upload a new descriptor follow the next steps:
- Clone the repository
- Add the source code of the descriptor in [descriptors](https://github.com/5gmetadmin/vnfdescriptors/tree/main/descriptors) folder
- "osm repo-index --origin descriptors/ --destination repository/"
- Push the changes to the repository
