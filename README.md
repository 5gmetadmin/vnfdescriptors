# repo-template
template to be used as common for all the new repositories

This document tries to provide the guidelines to properly upload code, technical documentation or binary files to the WP3 repository.

The document covers:
 - namespace or naming convention of the repository
 - structure of the files and folders in the repository
 - readme file structure and contents at the repository root

## Naming

The name of the repository is according to the architecture Building Block defined in WP3 Tasks at TEAMS then suffix "cloud", "edge" or "sensor"

For example:
> discovery_edge

### Not recognised

Avoid to:
 - use unofficial system name
 - include the project title
 - include the WP number
 - include the affiliation / partner name

For example:
> ~~discover_edge~~
> ~~5GMETAdiscovery_edge~~
> ~~WP3discovery_edge~~
> ~~vicom_discovery_edge~~


## Files and folders structure

The structure of the repository should include:
|File |Folder |Contains |
|---|---|---|
|README| |All the contents described in the next section |
|LICENSE | |Applicable license terms and conditions |
| |utils |all the dependencies not core of the system|
| |tests |all the unit tests to be done |
| |deploy |all the auxiliar files for deployment, including GITHUB actions if applicable, ansible playbook, ... |
| |miscelania |all the images, videos, ... |
| |examples |to guide integration purposes include a readme with scenario and pre-conditions, and scripts/Dockers |
| |api | YAML file for the API definition |
| |thirdparties | YAML file for the API definition for third parties and documentation for them |
| |src |the code |
| |system|the scripts/Dockers or binaries |

## README contents

The README file should include:

 1. Overview: including a summary of the intended functions and scope
 2. Prerequisites: including:
 	 -  infrastructure: assets/systems required and their features
 	 - device: model of the sensor
 	 - dependencies: list of [packages](http://example.org/) and their versions
 3. Features: including a list of implememented functions
 4. Deployment: including all the steps to deploy the system of the repository and the links to the deploy folder
 5. API: including:
 	 -  some guidelines or tips to integrate and links to examples and API folders
 	 - a sequence diagram to better understand the prerequisites, features and deployment
 6. Authors: list of authors of the code/implementation
 7. License: applicable license


