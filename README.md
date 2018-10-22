>In the coming weeks, GPO is planning to release Beta USLM XML in the draft 2.0 schema on the govinfo Bulk Data Repository for enrolled bills from the 113th Congress forward, public laws from the 113th Congress forward, and the Statutes at Large from the 108th Congress forward. For enrolled bills, the Beta USLM XML will be made available in addition to the existing Bill DTD XML. The Beta USLM XML will use the same file naming convention as the Bill DTD XML but the Beta USLM XML will be in a /bulkdata/BILLS/uslm/ folder. We are also planning to make the Beta USLM XML available on the govinfo website through "USLM" buttons and in the ZIP files. Beta USLM XML will be added to the govinfo API and Link Service in an upcoming release. See [GPO's USLM GitHub repository](https://github.com/usgpo/uslm/tree/proposed) for more information. 

>In December 2018, the FDsys website including the FDsys Bulk Data Repository, FDsys Sitemaps, and the FDsys Link Service will be retired. Please migrate tools and processes to [govinfo](https://www.govinfo.gov/developers).

# bulk-data

GPO provides the capability to download XML in bulk for select collections from the [FDsys Bulk Data Repository] (http://www.gpo.gov/fdsys/bulkdata/). 

Please see the User Guides within this repository for more information on how to make use of the XML data for the available collections.
 
### Examples:
 
Federal Register Issues from September 2012: http://www.gpo.gov/fdsys/bulkdata/FR/2012/09
 
Code of Federal Regulations: http://www.gpo.gov/fdsys/bulkdata/CFR/

Bills back to the 113th Congress: http://www.gpo.gov/fdsys/bulkdata/BILLS

FDsys will be retired in December 2018. Please begin adapting your processes to use the govinfo bulk data repository instead -- this contains the same data, but with additional features. Read more about the [transition to **govinfo**](https://www.govinfo.gov/about#fdsys-transition)

## govinfo bulk data
The **govinfo** team has migrated bulk data functionality to govinfo. 

https://www.govinfo.gov/bulkdata

### XML and JSON endpoints
New in govinfo, you can add /xml or /json to any govinfo bulkdata link to receive the listing in that format.

https://www.govinfo.gov/bulkdata/BILLS/115/1/hjres<br/>
XML: https://www.govinfo.gov/bulkdata/xml/BILLS/115/1/hjres<br/>
JSON: https://www.govinfo.gov/bulkdata/json/BILLS/115/1/hjres

### Examples 

Federal Register Issues from September 2012: http://www.govinfo.gov/bulkdata/FR/2012/09

Code of Federal Regulations: http://www.govinfo.gov/bulkdata/CFR/

Bills back to the 113th Congress: http://www.govinfo.gov/bulkdata/BILLS



