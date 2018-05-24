# bulk-data

GPO provides the capability to download XML in bulk for select collections from the [FDsys Bulk Data Repository] (http://www.gpo.gov/fdsys/bulkdata/). 

Please see the User Guides within this repository for more information on how to make use of the XML data for the available collections.
 
Examples:
 
Federal Register Issues from September 2012: http://www.gpo.gov/fdsys/bulkdata/FR/2012/09
 
Code of Federal Regulations: http://www.gpo.gov/fdsys/bulkdata/CFR/

Bills back to the 113th Congress: http://www.gpo.gov/fdsys/bulkdata/BILLS

## govinfo bulk data
The **govinfo** team has migrated bulk data functionality to govinfo, and we are pleased to make it available for initial feedback.

https://www.govinfo.gov/bulkdata

This should be functionally equivalent to the FDsys bulkdata feed.

New in govinfo, you can add /xml or /json to any govinfo bulkdata link to receive the listing in that format.

e.g. 

https://www.govinfo.gov/bulkdata/BILLS/115/1/hjres<br/>
XML: https://www.govinfo.gov/bulkdata/xml/BILLS/115/1/hjres<br/>
JSON: https://www.govinfo.gov/bulkdata/json/BILLS/115/1/hjres

**Note that these endpoints should not be used for critical production usage at this time -- please continue using the FDsys bulk data site for those purposes.

