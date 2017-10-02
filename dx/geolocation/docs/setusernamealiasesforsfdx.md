## Set Username Aliases For Sfdx

You can associate an alias with only one username at a time. If you’ve set an alias multiple times, the alias points to the most recent username.

To delete an alias, run "sfdx force:alias:set" with no username.



Option | Description
--- | --- 
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
To delete an alias, run "sfdx force:alias:set" with no username.

$ sfdx force:alias:set DefaultOrg=me@my.org

$ sfdx force:alias:set DefaultOrg=me@my.org DevHubOrg=me@myhub.org

$ sfdx force:alias:set AliasToDelete=

```

