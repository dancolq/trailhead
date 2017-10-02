## Fetch a Debug Log

When you execute this command in a project, it fetches the specified log from your default scratch org.To get the IDs for your debug logs, run "sfdx force:apex:log:list".



Option | Description
--- | --- 
```-i, --logid LOGID``` | id of the log to display
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

When you execute this command in a project, it fetches the specified log from your default scratch org.To get the IDs for your debug logs, run "sfdx force:apex:log:list".

$ sfdx force:apex:log:get -i <log id>

$ sfdx force:apex:log:get -i <log id> -u me@my.org


