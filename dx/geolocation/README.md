# DX Cheatsheet

This is intended to be used as a quick reference of Salesforce DX CI commands.


## force:project

### force:project:create
Create a new SFDX project

Examples

```javascript
sfdx force:project:create --projectname mywork
sfdx force:project:create --projectname mywork --defaultpackagedir myapp
```
Options

| Option  | Desctiption |
| ----------- | ----------------------- |
| -p, --defaultpackagedir DEFAULTPACKAGEDIR | default package directory name (force-app*)|
| -s, --namespace NAMESPACE                 | project associated namespace
| -d, --outputdir OUTPUTDIR                 | folder for saving the created files
| -n, --projectname PROJECTNAME             | name of the generated project
|  -t, --template TEMPLATE                   | template to use for file creation (Defaultsfdx-project.json*)
| --json                                    | json output
| --loglevel LOGLEVEL                       | logging level for this command invocation (error*,trace,debug,info,warn,fatal)



### force:project:upgrade

Update project config files to the latest format

Examples

 ```Javascript
 sfdx force:project:upgrade
 sfdx force:project:upgrade -f
 ```
 
 Options
 
 |Option|Description|
 | -- | -- |
 | -f, --forceupgrade  | run all upgrades even if project has already been upgraded
 | --json              | format output as json
 | --loglevel LOGLEVEL | logging level for this command invocation (error*,trace,debug,info,warn,fatal)
 


##force:org

 sfdx force:org:create               # create a scratch org
 sfdx force:org:delete               # mark a scratch org for deletion
 sfdx force:org:display              # get org description
 sfdx force:org:list                 # list all active orgs you've created or authenticated to
 sfdx force:org:open                 # open an org in your browser

### force:org:create

Create a scratch org

Examples

To set up a connected app for your new scratch org, specify the value that was returned when you created a connected app
 in your Dev Hub org as --clientid.
 
```Javascript
sfdx force:org:create -f config/enterprise-scratch-def.json -a TestOrg1
sfdx force:org:create -a MyDevOrg -s -v me@myhub.org edition=Developer
sfdx force:org:create -f config/enterprise-scratch-def.json -a OrgWithOverrides username=testuser1@mycompany.org
```

Options

|Option|Description|
|---|---|
| -i, --clientid CLIENTID                         | connected app consumer key
| -f, --definitionfile DEFINITIONFILE             | path to a scratch org definition file
| -n, --nonamespace                               | creates the scratch org with no namespace
| -a, --setalias SETALIAS                         | set an alias for for the created scratch org
| -s, --setdefaultusername                        | set the created org as the default username
| -v, --targetdevhubusername TARGETDEVHUBUSERNAME | username for the dev hub org; overrides default dev hub org
| -w, --wait WAIT                                 | the streaming client socket timeout (in minutes) (default:6, min:2)
| --json                                          | format output as json
| --loglevel LOGLEVEL                             | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


### force:org:delete

Mark a scratch org for deletion

To mark the org for deletion without being prompted to confirm, specify --noprompt.

Examples

```Javascript
sfdx force:org:delete -u me@my.org
sfdx force:org:delete -u MyOrgAlias -p
```

Options

|Option | Description|
|---|---|
 |-p, --noprompt                                  | no prompt to confirm deletion
 |-v, --targetdevhubusername TARGETDEVHUBUSERNAME | username for the dev hub org; overrides default dev hub org
 |-u, --targetusername TARGETUSERNAME             | username for the target org
 |--json                                          | format output as json
 |--loglevel LOGLEVEL                             | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


### force:org:display

Get org description

### force:org:list

List all active orgs you've created or authenticated to

### force:org:open

Open an org in your browser







__Create scratch org__

```javascript
sfdx force:org:create -s -f config/project-scratch-def.json -a GeoAppScratch
```

__Mark a scractch org for deletion__
```javascript
sfdx force:org:delete -u me@my.org
```
### force:org:list
---
List all active orgs you've created or authenticated to

Examples:
```javascript
sfdx force:org:list
sfdx force:org:list --verbose --json
sfdx force:org:list --verbose --json > tmp/MyOrgList.json
```
Options:

| Option            | Description                       |
| ------------------- | ---------------------------------- |
 |-p, --noprompt      | do not prompt for confirmation|
 |--all               | include expired, deleted, and unknown-status scratch orgs|
 |--clean             | remove all local org authorizations for non-active orgs |
 |--json              | format output as json|
 |--loglevel LOGLEVEL | logging level for this command invocation (error*,trace,debug,info,warn,fatal)|


__Get org description__
```javascript
sfdx force:org:delete -u me@my.org
```



_Note : Navigate to project directory first._

__Open scratch org__

```javascript
sfdx force:org:open
```


__Assign permission set__

```javascript
sfdx force:user:permset:assign -n Geolocation
```

_Note : Geolocation = permission set._

__Pull Changes__

```javascript
sfdx force:source:pull
```

__Push Changes__

```
sfdx force:source:push
```

__Export Data__

```javascript
sfdx force:data:tree:export -q "SELECT Name, Location__Latitude__s, Location__Longitude__s FROM Account WHERE Location__Latitude__s != NULL AND Location__Longitude__s != NULL" -d ./data
```

__Import Data__

```javascript 
sfdx force:data:tree:import --sobjecttreefiles data/Account.json
```

__Create Apex Class__

```
sfdx force:apex:class:create -n AccountController -d force-app/main/default/classes
```

__Create Lightning Component__
```
sfdx force:lightning:component:create -n AccountLocator -d force-app/main/default/aura
```

__Create Lightning Event__
```
sfdx force:lightning:event:create -n AccountsLoaded -d force-app/main/default/aura
```

