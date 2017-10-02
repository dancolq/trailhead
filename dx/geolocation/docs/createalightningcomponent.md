## Create a Lightning Component

If not supplied, the apiversion, template, and outputdir use default values.

The outputdir can be an absolute path or relative to the current working directory.



Option | Description
--- | --- 
```-a, --apiversion APIVERSION``` | api version number (40.0*,39.0)
```-n, --componentname COMPONENTNAME``` | name of the generated lightning component
```-d, --outputdir OUTPUTDIR``` | folder for saving the created files
```-t, --template TEMPLATE``` | template to use for file creation (DefaultLightningCmp*)
```--json``` | json output
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:lightning:component:create -n mycomponent

$ sfdx force:lightning:component:create -n mycomponent -d lightning


