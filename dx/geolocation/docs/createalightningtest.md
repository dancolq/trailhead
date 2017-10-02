## Create a Lightning Test

The outputdir can be an absolute path or relative to the current working directory.



Option | Description
--- | --- 
```-d, --outputdir OUTPUTDIR``` | folder for saving the created files
```-t, --template TEMPLATE``` | template to use for file creation (DefaultLightningTest*)
```-n, --testname TESTNAME``` | name of the generated lightning test
```--json``` | json output
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:lightning:test:create -n MyLightningTest

$ sfdx force:lightning:test:create -n MyLightningTest -d lightningTests

```

