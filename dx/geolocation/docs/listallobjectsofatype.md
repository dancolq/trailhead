## List All Objects Of a Type



Option | Description
--- | --- 
```-c, --sobjecttypecategory SOBJECTTYPECATEGORY``` | the type of objects to list (all|custom|standard)
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:schema:sobject:list -c all

$ sfdx force:schema:sobject:list -c custom

$ sfdx force:schema:sobject:list -c standard


