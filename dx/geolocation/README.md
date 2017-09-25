# DX Cheatsheet

This is intended to be used as a quick reference of Salesforce DX CI commands.


## Commands

__Create project__

```javascript
sfdx force:project:create -n geolocation
```

###force:org
__Create scratch org__

```javascript
sfdx force:org:create -s -f config/project-scratch-def.json -a GeoAppScratch
```

__Mark a scractch org for deletion__
```javascript
sfdx force:org:delete -u me@my.org
```
__List all active orgs you've created or authenticated to__
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

