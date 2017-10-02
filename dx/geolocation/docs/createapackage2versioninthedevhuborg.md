## Create a Package2 Version In The Dev Hub Org

The package2 version is based on the manifest, descriptor, and package2 contents in the specified directory.

To retrieve details about a package2 version create request, including status and package2 version id (05i), run "sfdx force:package2:version:create:get -i 08c...".

To list package2 version creation requests in the org, run "sfdx force:package2:version:create:list".



Option | Description
--- | --- 
```-b, --branch BRANCH``` | the package2 version's branch
```-d, --directory DIRECTORY``` | directory that contains the manifest, descriptor, and contents of the package2 version
```-i, --package2id PACKAGE2ID``` | id of the parent package2 (starts with 0Ho)
```-t, --tag TAG``` | the package2 version's tag
```-v, --targetdevhubusername TARGETDEVHUBUSERNAME``` | username for the dev hub org; overrides default dev hub org
```-w, --wait WAIT``` | minutes to wait for the package2 version to be created (default:0)
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
To retrieve details about a package2 version create request, including status and package2 version id (05i), run "sfdx force:package2:version:create:get -i 08c...".

To list package2 version creation requests in the org, run "sfdx force:package2:version:create:list".

$ sfdx force:package2:version:create --package2id 0Ho... --directory common --tag 'Release 1.0.0' --branch master

$ sfdx force:package2:version:create -i 0Ho... -d common

```

