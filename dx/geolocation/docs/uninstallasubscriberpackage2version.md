## Uninstall a Subscriber Package2 Version

Specify the subscriber package2 version ID.

To list the org’s installed subscriber package2 versions, run "package2:installed:list".



Option | Description
--- | --- 
```-i, --subscriberpackage2versionid SUBSCRIBERPACKAGE2VERSIONID``` | the id of the subscriber package2 version to uninstall (starts with 04t)
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:package2:version:uninstall --subscriberpackage2versionid 04t...

$ sfdx force:package2:version:uninstall -i 04t... -u <username of target org>


