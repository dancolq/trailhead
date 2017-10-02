## Convert Sfdx Source Into The Metadata Api Source Format

To convert Salesforce DX–formatted source into a format that you can deploy using Metadata API, run "sfdx force:source:convert". Then deploy the source using "sfdx force:mdapi:deploy".

To convert Metadata API–formatted source into the Salesforce DX format, run "sfdx force:mdapi:convert".



Option | Description
--- | --- 
```-d, --outputdir OUTPUTDIR``` | the output directory to export the metadata api source to
```-n, --packagename PACKAGENAME``` | the name of the package to associate with the metadata api source
```-r, --rootdir ROOTDIR``` | the source directory for the source to be converted
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

To convert Salesforce DX–formatted source into a format that you can deploy using Metadata API, run "sfdx force:source:convert". Then deploy the source using "sfdx force:mdapi:deploy".

To convert Metadata API–formatted source into the Salesforce DX format, run "sfdx force:mdapi:convert".

$ sfdx force:source:convert -r <path to source>

$ sfdx force:source:convert -r <path to source> -d <path to output dir>


