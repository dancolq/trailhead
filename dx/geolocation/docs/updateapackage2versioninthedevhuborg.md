## Update a Package2 Version In The Dev Hub Org

Specify a new value for each option you want to update.

To display details about a package2 version, run "sfdx package2:version:get".



Option | Description
--- | --- 
```-b, --branch BRANCH``` | the package2 version branch
```-d, --description DESCRIPTION``` | the package2 version description
```-n, --name NAME``` | the package2 version name
```-i, --package2versionid PACKAGE2VERSIONID``` | the package2 version id (starts wtih 05i)
```-s, --setasreleased``` | set the package2 version as released (can't be undone)
```-t, --tag TAG``` | the package2 version tag
```-v, --targetdevhubusername TARGETDEVHUBUSERNAME``` | username for the dev hub org; overrides default dev hub org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:package2:version:update --package2versionid 05i... --setasreleased

$ sfdx force:package2:version:update --i 05i... -b master -t 'Release 1.0.7'


