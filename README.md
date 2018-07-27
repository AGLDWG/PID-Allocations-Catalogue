# PID URI Catalogue
This repository contains configuration information for the Australian Government Linked Data Working Group (AGLDWG)'s PID Allocations Catalogue, online at:

* [catalogue.linked.data.gov.au](http://catalogue.linked.data.gov.au)

The issue tracker for this tool is this repository's GitHub issue tracker: <https://github.com/AGLDWG/PID-Allocations-Catalogue/issues>

## Catalogue configuration
This repository documents the setup of the PID proxy.

### In outline
The catalogue is implemented using a standard setup of the [Drupal content management system, version 8](https://www.drupal.org/8). A custom content type is implemented for "Catalogue Records" items, instances of which then contain the catalogue's main data. User accounts are local only - individual local accounts are needed for everyone needing to use the system.

### In detail
* **server hosting**: Virtual Machine in an [Amazon Web Services](https://aws.amazon.com/) account owned by [CSIRO](https://www.csiro.au/)
  * account details available from the Environmental Informatics group in CSIRO's [Land & Water](https://www.csiro.au/en/Research/LWF) division
* **server operating system**: Ubuntu 18.04
* **web server**: Apache 2.4
* **Content Management System**: Drupal 8
  * database: MySQL
  * scripting: PHP7
* **access control**: for the server, SSH using a key. For the CMS, local Drupal accounts
  * the SSH key and other details are managed by the Technical Contact (see below)

The installation log for the server is contained in this repository in the file [install.sh](install.sh).


## Catalogue content
The catalogue's content is all available via its main page, [catalogue.linked.data.gov.au](http://catalogue.linked.data.gov.au).

Schema for the content in the catalogue, when finalised, will be given in this repository, including mappings to Semantic Web models.


## License
This repository is licensed under Creative Commons 4.0 International. See the [LICENSE deed](LICENSE) in this repository for details.


## Contacts
System Owner:  [Australian Government Linked Data Working Group](http://www.linked.data.gov.au)

System Owner contact:  
**Nicholas Car**  
*Senior Experimental Scientist*  
*Co-chair, AGLDWG*  
CSIRO Land & Water  
<nicholas.car@csiro.au>  

Technical Contact:  
**Edmond Chuc**  
*Research Projects Officer*  
CSIRO Land & Water  
<edmond.chuc@csiro.au>  
