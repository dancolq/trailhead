## Install a Subscriber Package2 Version

Installs a second-generation subscriber package version in the target org. To view the error messages, open the Dev Hub org, select the Setup menu, enter Deployment in the Quick Find box, and select Deployment Status.

To find the ID for the subscriber package2 version, run "sfdx package2:version:list".

To list the org’s installed subscriber package2 versions, run "package2:installed:list".



Option | Description
--- | --- 
```-i, --subscriberpackage2versionid SUBSCRIBERPACKAGE2VERSIONID``` | the id of the subscriber package2 version to install (starts with 04t)
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:package2:version:install --subscriberpackage2versionid 04t...

$ sfdx force:package2:version:install -i 04t... -u <username of target org>


