## Convert Metadata Api Source Into The Sfdx Source Format

To work with source that you retrieved via Metadata API using the Salesforce DX tools, convert the source to the Salesforce DX format using "sfdx force:mdapi:convert".

To convert the source back to the Metadata API format, so that you can deploy it using "sfdx force:mdapi:deploy", run "sfdx force:source:convert".



Option | Description
--- | --- 
```-r, --rootdir ROOTDIR``` | the root directory containing the metadata api source
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

To work with source that you retrieved via Metadata API using the Salesforce DX tools, convert the source to the Salesforce DX format using "sfdx force:mdapi:convert".

To convert the source back to the Metadata API format, so that you can deploy it using "sfdx force:mdapi:deploy", run "sfdx force:source:convert".

$ sfdx force:mdapi:convert -r <path to source>

$ sfdx force:mdapi:convert -r <path to source> -d <path to outputdir>


