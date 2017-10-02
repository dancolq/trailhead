## Set Config Vars For Sfdx

Sets the configuration variables that the Salesforce CLI uses for various commands and tasks. Local variables apply only to your current project. Global variables apply in any directory.



Option | Description
--- | --- 
```-g, --global``` | set config var globally (to be used from any directory)
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:config:set defaultusername=me@my.org defaultdevhubusername=me@myhub.org

$ sfdx force:config:set defaultdevhubusername=me@myhub.org -g

```

