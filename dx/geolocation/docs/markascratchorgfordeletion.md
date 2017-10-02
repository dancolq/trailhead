## Mark a Scratch Org For Deletion

To mark the org for deletion without being prompted to confirm, specify --noprompt.



Option | Description
--- | --- 
```-p, --noprompt``` | no prompt to confirm deletion
```-v, --targetdevhubusername TARGETDEVHUBUSERNAME``` | username for the dev hub org; overrides default dev hub org
```-u, --targetusername TARGETUSERNAME``` | username for the target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:org:delete -u me@my.org

$ sfdx force:org:delete -u MyOrgAlias -p

```

