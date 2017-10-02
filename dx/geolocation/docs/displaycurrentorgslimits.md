## Display Current Org’S Limits

When you execute this command in a project, it provides limit information for your default scratch org.



Option | Description
--- | --- 
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:limits:api:display

$ sfdx force:limits:api:display -u me@my.org

```

