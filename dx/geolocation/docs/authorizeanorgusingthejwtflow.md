## Authorize An Org Using The Jwt Flow

Authorizes a Salesforce org using a private key file that has been uploaded to a personal connected app.



Option | Description
--- | --- 
```-i, --clientid CLIENTID``` | oauth client id (sometimes called the consumer key)
```-r, --instanceurl INSTANCEURL``` | the login url of the instance the org lives on
```-f, --jwtkeyfile JWTKEYFILE``` | path to a file containing the private key
```-a, --setalias SETALIAS``` | set an alias for for the authenticated org
```-d, --setdefaultdevhubusername``` | set the authenticated org as the default dev hub org for scratch org creation
```-s, --setdefaultusername``` | set the authenticated org as the default username that all commands run against
```-u, --username USERNAME``` | authentication username
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:auth:jwt:grant -u me@my.org -f <path to jwt key file> -i <oauth client id>

$ sfdx force:auth:jwt:grant -u me@my.org -f <path to jwt key file> -i <oauth client id> -s -a MyDefaultOrg

```

