## Create a Package2

First, use this command to create a package2. Then create a package2 version.

Run 'sfdx force:package2:list' to list all package2 packages in the dev hub org.



Option | Description
--- | --- 
```-d, --description DESCRIPTION``` | package2 description
```-n, --name NAME``` | package2 name
```-s, --namespace NAMESPACE``` | the package2 global namespace
```-v, --targetdevhubusername TARGETDEVHUBUSERNAME``` | username for the dev hub org; overrides default dev hub org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:package2:create --name PackageName --namespace MyNamespace --description 'My New Package'

Run 'sfdx force:package2:list' to list all package2 packages in the dev hub org.

```

