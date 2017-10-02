## Authorize An Org Using An Sfdx Auth Url

Authorize a Salesforce org using an SFDX auth URL stored within a file.

The file must have the format "force://<refreshToken>@<instanceUrl>" or "force://<clientId>:<clientSecret>:<refreshToken>@<instanceUrl>".

The file must contain only the URL or be a JSON file that has a top-level property named sfdxAuthUrl.



Option | Description
--- | --- 
```-a, --setalias SETALIAS``` | set an alias for for the authenticated org
```-d, --setdefaultdevhubusername``` | set the authenticated org as the default dev hub org for scratch org creation
```-s, --setdefaultusername``` | set the authenticated org as the default username that all commands run against
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:auth:sfdxurl:store -f <path to sfdxAuthUrl file>

$ sfdx force:auth:sfdxurl:store -f <path to sfdxAuthUrl file> -s -a MyDefaultOrg

```

