## Display Test Results

Displays test results for an enqueued or completed asynchronous Apex test run.



Option | Description
--- | --- 
```-c, --codecoverage``` | retrieve code coverage results
```-d, --outputdir OUTPUTDIR``` | directory to store test run files
```-r, --resultformat RESULTFORMAT``` | test result format emitted to stdout; --json flag overrides this parameter (human*,tap,junit,json)
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-i, --testrunid TESTRUNID``` | id of test run
```-w, --wait WAIT``` | the streaming client socket timeout (in minutes) (default:6, min:2)
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)
```--verbose``` | display apex test processing details


__Exmples:__ 

```
$ sfdx force:apex:test:report -i <test run id>

$ sfdx force:apex:test:report -i <test run id> -r junit

$ sfdx force:apex:test:report -i <test run id> -c --json

```

