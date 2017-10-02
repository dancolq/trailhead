## List Debug Logs

When you execute this command in a project, it lists the log IDs for your default scratch org.



Option | Description
--- | --- 
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:apex:log:list

$ sfdx force:apex:log:list -u me@my.org


