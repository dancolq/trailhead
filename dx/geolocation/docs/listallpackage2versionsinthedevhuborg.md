## List All Package2 Versions In The Dev Hub Org

Displays details of each package2 version in the org.

Use --concise or --verbose to display limited or additional details, respectively.

All filter parameters are applied using the AND logical operator (not OR).



Option | Description
--- | --- 
```-c, --createdlastdays CREATEDLASTDAYS``` | created in the last specified number of days (starting at 00:00:00 of first day to now; 0 for today)
```-m, --modifiedlastdays MODIFIEDLASTDAYS``` | list items modified in the last given number of days (starting at 00:00:00 of first day to now; 0 for today)
```-o, --orderby ORDERBY``` | order by the specified package2 version fields
```-i, --package2ids PACKAGE2IDS``` | filter results on specified comma-delimited package2 ids (start with 0Ho)
```-r, --released``` | display released versions only
```-v, --targetdevhubusername TARGETDEVHUBUSERNAME``` | username for the dev hub org; overrides default dev hub org
```--concise``` | display limited package2 version details
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)
```--verbose``` | display extended package2 versions detail


__Exmples:__ 

```
$ sfdx force:package2:version:list --verbose --createdlastdays 3 --released --orderby PatchVersion

$ sfdx force:package2:version:list --package2ids 0Ho000000000000,0Ho000000000001 --released --modifiedlastdays 0

$ sfdx force:package2:version:list --released

$ sfdx force:package2:version:list --concise --modifiedlastdays 0

$ sfdx force:package2:version:list --concise -c 3 -r

```

