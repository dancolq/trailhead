## Install a Package In The Target Org

Supply the ID of the package you want to install. Installs to the default username org unless you supply the username for a different target org.



Option | Description
--- | --- 
```-i, --id ID``` | id of the package to install (starts with 04t)
```-k, --installationkey INSTALLATIONKEY``` | installation key for key-protected package (default: null)
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-w, --wait WAIT``` | number of minutes to wait for installation status
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:package:install -i 04t6A0000004eytQAA

$ sfdx force:package:install -i 04t6A0000004eytQAA -u me@my.org

```

