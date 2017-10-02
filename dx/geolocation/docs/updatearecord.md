## Update a Record

The format of a field-value pair is <fieldName>=<value>.

Enclose all field-value pairs in one set of double quotation marks.

Enclose values that contain spaces in single quotes.



Option | Description
--- | --- 
```-i, --sobjectid SOBJECTID``` | the id of the record you’re updating
```-s, --sobjecttype SOBJECTTYPE``` | the type of the record you’re updating
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-v, --values VALUES``` | the <fieldName>=<value> pairs you’re updating
```-w, --where WHERE``` | a list of <fieldName>=<value> pairs to search for
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:data:record:update -s Account -i 001D000000Kv3dl -v "Name=NewAcme"

$ sfdx force:data:record:update -s Account -w "Name='Old Acme'" -v "Name='New Acme'"

$ sfdx force:data:record:update -s Account -i 001D000000Kv3dl -v "Name='Acme III' Website=www.example.com"


