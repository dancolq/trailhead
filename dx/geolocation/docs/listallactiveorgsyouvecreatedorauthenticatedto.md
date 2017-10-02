## List All Active Orgs You’Ve Created Or Authenticated To



Option | Description
--- | --- 
```-p, --noprompt``` | do not prompt for confirmation
```--all``` | include expired, deleted, and unknown-status scratch orgs
```--clean``` | remove all local org authorizations for non-active orgs
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:org:list

$ sfdx force:org:list --verbose --json

$ sfdx force:org:list --verbose --json > tmp/MyOrgList.json

```

