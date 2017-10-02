## Create a New Package Version In The Release Org

The package version is based on the contents of the specified metadata package. Omit -m if you want to create an unmanaged package version.



Option | Description
--- | --- 
```-d, --description DESCRIPTION``` | package version description
```-k, --installationkey INSTALLATIONKEY``` | installation key for key-protected package (default: null)
```-m, --managedreleased``` | create a managed package version
```-n, --name NAME``` | package version name
```-i, --packageid PACKAGEID``` | id of the metadata package (starts with 033) of which you’re creating a new version
```-p, --postinstallurl POSTINSTALLURL``` | post install url
```-r, --releasenotesurl RELEASENOTESURL``` | release notes url
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-v, --version VERSION``` | package version in major.minor format, for example, 3.2
```-w, --wait WAIT``` | minutes to wait for the package version to be created (default: 2 minutes)
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)
