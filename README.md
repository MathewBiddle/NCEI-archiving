# NCEI-archiving
Code, documentation and issue tracking for NANOOS NCEI archiving

- Refer to the excellent NCEI IOOS archiving cookbook documentation: [Archiving your data at NCEI - A Guide for IOOS Regional Association Data Managers](https://sites.google.com/a/noaa.gov/ncei-ioos-archive/cookbook/data-integrity)
- [NCEI NetCDF Templates v2.0](https://www.nodc.noaa.gov/data/formats/netcdf/v2.0/)
- [Attribute Conventions Dataset Discovery (ACDD)](http://wiki.esipfed.org/index.php/Attribute_Convention_for_Data_Discovery). This ESIP-hosted site is now the official ACDD documentation. The [ERDDAP documentation](http://coastwatch.pfeg.noaa.gov/erddap/download/setupDatasetsXml.html#globalAttributes) also has useful information in a useful format.

## NCEI Disclaimer

*The recommendations provided by NCEI staff on the issues and documents in this repository are primarily for the NANOOS archival process at NCEI. While some of the information might be useful and applicable to other data sets, these are not blanket statements for all of NCEI's archival procedures.*

## NANOOS OHSU CMOP NCEI Archiving

- Monthly netcdf files for archiving (pulled by NCEI): http://data.nanoos.org/ncei/ohsucmop/
- [NCEI Submission Agreement (SA).](http://www.nanoos.org/documents/certification/DMP/NANOOS-NCEI-Submission_Agreement_2017-03-13T19-51-12.pdf) The SA has extensive technical details about the archiving procedures. Some relevant fragments from the SA, with small additions: *"Submission Information Packages (SIP) will be organized into 'bags'. Each 'bag' will contain data, metadata, and manifest files which fully document the files intended to be submitted. The 'bags' will be folders on http://data.nanoos.org/ncei/ohsucmop/ which correspond to the name of the platform. E.g. abpoa/, riverrad/, saturn01/, etc. Within the station folder (or 'bag') there will be four standard files with the following names: bag-into.txt, bagit.txt, manifest-sha256.txt, and tagmanifest-sha256.txt as well as a data/ directory which will contain folders for all of the netCDF files to be submitted. Each of the folders within the data/ directory represent an instrument/instrument deployment.... NCEI will organize the Archival Information Packages (AIP) by station. Each time a new station arrives, a new AIP will be generated."*


## Other NANOOS or NANOOS-related data archived on NCEI

In addition to the formal data archiving process we are setting up, which will follow the IOOS-NCEI "gold standard" and will be done in coordination with NANOOS DMAC, other data packages may have been archived already at NCEI with a keyword linkage or acknowledgment to NANOOS. [This "NANOOS" search](http://data.nodc.noaa.gov/geoportal/rest/find/document?searchText=%22NANOOS%22&start=1&max=250&contentOption=intersecting&f=searchPage) to the [NCEI Geoportal](http://data.nodc.noaa.gov/geoportal/) returns all current NCEI records matching a NANOOS string.
- Currently (2016-12-7), there is one record there: [Dissolved inorganic carbon, total alkalinity, phosphate, silicate, and other variables collected from profile and discrete sample observations using CTD, Niskin bottle and other instruments in the northwest coast of the United States near the Cha Ba mooring off La Push, Washington from 2011-05-22 to 2014-10-24 (NCEI Accession 0145160)](http://data.nodc.noaa.gov/cgi-bin/iso?id=gov.noaa.nodc:0145160). It looks like it was [submitted March 2016](ftp://ftp.nodc.noaa.gov/nodc/archive/arc0099/0145160/1.1/about/0-email.txt), but may have been updated in early Nov 2016. Data files are in Excel and csv formats (*"Distribution Formats: Originator data format"*).
- Note that **Glider DAC data** are not returned! Neither CMOP gliders, nor the CeNCOOS-NANOOS glider, both of which have been submitted to the Glider DAC. *(Emilio has discussed this issue with IOOS, NCEI and Glider DAC teams since June 2016; Glider DAC technical options/solutions were discussed at https://github.com/ioos/ioosngdac/issues/105, but it's not clear a solution has been implemented as of 12/9/2016).*
  - However, I did find the CMOP Glider DAC records by searching for "CMOP": [the search returned 16 records](http://data.nodc.noaa.gov/geoportal/rest/find/document?searchText=%22CMOP%22&start=1&max=250&contentOption=intersecting&f=searchPage); here's [one of the records](http://data.nodc.noaa.gov/cgi-bin/iso?id=gov.noaa.nodc:0145907). But none of the records have any description words or keywords listing NANOOS. I'm sure we had such affiliation somewhere in the ACDD or other information we provided to the Glider DAC (hence the ability to find NANOOS-affiliated gliders in the [Glider DAC ERDDAP](https://data.ioos.us/gliders/erddap/search/index.html?searchFor=NANOOS)), so I assume the affiliation was lost in the transfer from the DAC to NCEI. 
  - I also found one of the **Trinidad Head glider** records, which appears to have been submitted by OSU directly (not the Glider DAC); [here's the record](http://data.nodc.noaa.gov/cgi-bin/iso?id=gov.noaa.nodc:0125046) obtained by searching on `"trinidad" AND "glider"`; a "glider" and geographical search didn't return any other records. This Trinidad record (Accession# 0125046) is the same one Anatoli told me about in May 2015.
  - The **complete list of NANOOS-affiliated glider datasets (deployments) submitted to the Glider DAC** are [listed on the DAC ERDDAP using "NANOOS" as a search string](https://data.ioos.us/gliders/erddap/search/index.html?searchFor=NANOOS). Currently there are 16 CMOP ("corie") and 5 OSU / Trinidad ("mbari") deployments. At the Glider DAC v2 site (not ERDDAP), we can get at these listings by "provider" for [corie](https://data.ioos.us/gliders/providers/users/corie/deployments) and [mbari](https://data.ioos.us/gliders/providers/users/mbari/deployments)
