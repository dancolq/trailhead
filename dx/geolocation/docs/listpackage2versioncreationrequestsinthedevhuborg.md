## List Package2 Version Creation Requests In The Dev Hub Org

Shows the details of each request to create a package2 version that's run in the Dev Hub org.

All filter parameters are applied using the AND logical operator (not OR).

To get information about a specific request, run "sfdx force:package2:version:create:get" and supply the request ID.



Option | Description
--- | --- 
```-c, --createdlastdays CREATEDLASTDAYS``` | created in the last specified number of days (starting at 00:00:00 of first day to now; 0 for today)
```-s, --status STATUS``` | filter the list by version creation request status (Queued,InProgress,Success,Error)
```-v, --targetdevhubusername TARGETDEVHUBUSERNAME``` | username for the dev hub org; overrides default dev hub org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
To get information about a specific request, run "sfdx force:package2:version:create:get" and supply the request ID.

$ sfdx force:package2:version:create:list

$ sfdx force:package2:version:create:list --createdlastdays 3

$ sfdx force:package2:version:create:list --status Error

$ sfdx force:package2:version:create:list -s InProgress

$ sfdx force:package2:version:create:list -c 3 -s Success

```

