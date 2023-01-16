EPrints / Azure Project
=======================

WHAT WE NEED
------------

CI/CD pipeline

Container registry

MariaDB (Azure SAAS)
* **NOT** containerised database as part of Pod
* **Requires** Access tables -> flat file

AZ Storage
* EPrints Storage Plugin to use blobs (like [amazon_s3](http://bazaar.eprints.org/115/) plugin)
* [BagIt](https://en.wikipedia.org/wiki/BagIt)
* [OCFL](https://ocfl.io/)
* volatile data
* usage metrics
* access tables

AZ Functions

AZ Firewalls

AZ ScaleSets (for containers)

AZ networking

WHAT WE'RE CREATING
-------------------

Containers to run:
* RDL
* RADAR
* Timescapes
* Digital Library
* DUAL
* RADIAL
* WRRO
* WREO

+ DEV instances of above
+ QA instances of above (where needed)
+ Digital preservation strategy - Wellcome [Storage Service](https://github.com/wellcomecollection/storage-service)?

Web front-ends

Processing back-ends

Ingest back-ends

Management dashoard

Workflows

Ingest sources (e.g. from Globus / Z:\ drive / ??? )

Research compute resource adjacent to content
* [LASER](https://lida.leeds.ac.uk/laser/)
* [SafePod](https://safepodnetwork.ac.uk/)

IIIF

ElasticSearch (container)

Volatile / Derivative versions (thumbnails / coversheets / indexes)

Connector with explore.library.leeds.ac.uk + DLIB API layer

Usage metrics (volatile data within storage format).

TOOLCHAIN
---------

* Terraform / Ansible
* S21 [Soure-To-Image](https://github.com/openshift/source-to-image)
* EPrints (versioned)
  * Flavours (versioned)
  * Ingredients (versioned)

 