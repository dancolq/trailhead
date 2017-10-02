## Get Config Var Value(S) For Given Name(S)

To see your default scratch org username, include "defaultusername".

To see your default Dev Hub, include "defaultdevhubusername".

To see your default instance URL, include "instanceUrl".

To see the locations where your values are set, include the --verbose flag.



Option | Description
--- | --- 
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)
```--verbose``` | emit additional command output to stdout


__Exmples:__ 

```
$ sfdx force:config:get defaultusername

$ sfdx force:config:get defaultusername defaultdevhubusername instanceUrl

$ sfdx force:config:get defaultusername defaultdevhubusername --verbose

```

