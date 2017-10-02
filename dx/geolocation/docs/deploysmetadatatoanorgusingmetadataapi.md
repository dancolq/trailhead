## Deploys Metadata To An Org Using Metadata Api

Specify the location of the files to deploy as a .zip file or by the root of the directory tree containing the files. To check the status of a deployment, specify its job ID.

The default value of --rollbackonerror is true, but the corresponding parameter in the Metadata API deploy() call defaults to false.



Option | Description
--- | --- 
```-c, --checkonly``` | validate deploy but don’t save to org (default: false)
```-d, --deploydir DEPLOYDIR``` | root of directory tree of files to deploy
```-i, --jobid JOBID``` | job ID of the deployment you want to check
```-e, --rollbackonerror ROLLBACKONERROR``` | roll back deployment on any failure (default: true) (default:true)
```-r, --runtests RUNTESTS``` | tests to run if --testlevel RunSpecifiedTests
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-l, --testlevel TESTLEVEL``` | deployment testing level (NoTestRun,RunSpecifiedTests,RunLocalTests,RunAllTestsInOrg)
```-w, --wait WAIT``` | wait time for command to finish in minutes (default: 0)
```-f, --zipfile ZIPFILE``` | path to .zip file of metadata to deploy
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)
```--verbose``` | verbose output of deploy results
