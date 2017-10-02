## Retrieve a Package2 Version Creation Request In The Dev Hub Org

Specify the request ID for which you want to view details. If applicable, the command displays errors related to the request.

To show all requests in the org, run "sfdx package2:version:create:list".



Option | Description
--- | --- 
```-i, --package2createrequestid PACKAGE2CREATEREQUESTID``` | package2 version creation request id (starts with 08c)
```-v, --targetdevhubusername TARGETDEVHUBUSERNAME``` | username for the dev hub org; overrides default dev hub org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:package2:version:create:get --package2createrequestid 08c...


