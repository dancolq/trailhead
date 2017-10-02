## View a Record

Specify an sObject type and either an ID or a list of <fieldName>=<value> pairs.

The format of a field-value pair is <fieldName>=<value>.

Enclose all field-value pairs in one set of double quotation marks.

Enclose values that contain spaces in single quotes.



Option | Description
--- | --- 
```-i, --sobjectid SOBJECTID``` | the id of the record you’re retrieving
```-s, --sobjecttype SOBJECTTYPE``` | the type of the record you’re retrieving
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-w, --where WHERE``` | a list of <fieldName>=<value> pairs to search for
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:data:record:get -s Account -i 001D000000Kv3dl

$ sfdx force:data:record:get -s Account -w "Name=Acme"

$ sfdx force:data:record:get -s Account -w "Name='Universal Containers'"

$ sfdx force:data:record:get -s Account -w "Name='Universal Containers' Phone='(123) 456-7890'"

```

