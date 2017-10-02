## Invoke Lightning Component Tests



Option | Description
--- | --- 
```-a, --appname APPNAME``` | name of your lightning test application
```-f, --configfile CONFIGFILE``` | path to config file for the test
```-o, --leavebrowseropen``` | leave browser open
```-d, --outputdir OUTPUTDIR``` | directory path to store test run artifacts: log files, test results, etc
```-r, --resultformat RESULTFORMAT``` | test result format emitted to stdout; --json flag overrides this parameter (human*,tap,junit,json)
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-t, --timeout TIMEOUT``` | time (ms) to wait for element in dom (default:20000)
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:lightning:test:run

$ sfdx force:lightning:test:run -a tests -r human

$ sfdx force:lightning:test:run -f config/myConfigFile.json -d testResultFolder

```

