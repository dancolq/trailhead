## List Local Changes And/Or Changes In a Scratch Org



Option | Description
--- | --- 
```-a, --all``` | list all the changes that have been made
```-l, --local``` | list the changes that have been made locally
```-r, --remote``` | list the changes that have been made in the scratch org
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:source:status -l

$ sfdx force:source:status -r

$ sfdx force:source:status -a

$ sfdx force:source:status -a -u me@my.org --json


