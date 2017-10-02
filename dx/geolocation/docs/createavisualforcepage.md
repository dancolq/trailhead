## Create a Visualforce Page

If not supplied, the apiversion, template, and outputdir use default values.

The outputdir can be an absolute path or relative to the current working directory.

Name and label are required.



Option | Description
--- | --- 
```-a, --apiversion APIVERSION``` | api version number (40.0*,39.0)
```-l, --label LABEL``` | visualforce page label
```-d, --outputdir OUTPUTDIR``` | folder for saving the created files
```-n, --pagename PAGENAME``` | name of the generated visualforce page
```-t, --template TEMPLATE``` | template to use for file creation (DefaultVFPage*)
```--json``` | json output
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:visualforce:page:create -n mypage -l mylabel

$ sfdx force:visualforce:page:create -n mypage -l mylabel -d pages

```

