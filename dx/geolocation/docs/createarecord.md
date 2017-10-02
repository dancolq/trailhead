## Create a Record

The format of a field-value pair is <fieldName>=<value>.

Enclose all field-value pairs in one set of double quotation marks.

Enclose values that contain spaces in single quotes.



Option | Description
--- | --- 
```-s, --sobjecttype SOBJECTTYPE``` | the type of the record you’re creating
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-v, --values VALUES``` | the <fieldName>=<value> pairs you’re creating
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:data:record:create -s Account -v "Name=Acme"

$ sfdx force:data:record:create -s Account -v "Name='Universal Containers'"

$ sfdx force:data:record:create -s Account -v "Name='Universal Containers' Website=www.example.com"

```

