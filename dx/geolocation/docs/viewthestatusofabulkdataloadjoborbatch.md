## View The Status Of a Bulk Data Load Job Or Batch



Option | Description
--- | --- 
```-b, --batchid BATCHID``` | the id of the batch whose status you want to view
```-i, --jobid JOBID``` | the id of the job you want to view or of the job whose batch you want to view
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:data:bulk:status -i 750xx000000005sAAA

$ sfdx force:data:bulk:status -i 750xx000000005sAAA -b 751xx000000005nAAA

```

