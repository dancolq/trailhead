## Assign a Permission Set To The Admin User Of An Org



Option | Description
--- | --- 
```-n, --permsetname PERMSETNAME``` | the name of the permission set to assign
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:user:permset:assign -n DreamHouse

$ sfdx force:user:permset:assign -n DreamHouse -u me@my.org

$ sfdx force:user:permset:assign -n DreamHouse -u TestOrg1


