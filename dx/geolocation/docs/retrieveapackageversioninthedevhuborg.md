## Retrieve a Package Version In The Dev Hub Org

To update package version values, run "sfdx force:package2:version:update".



Option | Description
--- | --- 
```-i, --package2versionid PACKAGE2VERSIONID``` | the package2 version id (starts wtih 05i)
```-v, --targetdevhubusername TARGETDEVHUBUSERNAME``` | username for the dev hub org; overrides default dev hub org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:package2:version:get --package2versionid 05i...

To update package version values, run "sfdx force:package2:version:update".

```

