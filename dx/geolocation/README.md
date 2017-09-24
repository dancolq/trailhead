# DX Cheatsheet

This is intended to be used as a quick reference of Salesforce DX CI commands.


## Commands

__Create project__

```javascript
sfdx force:project:create -n geolocation
```

__Create scratch org__

```javascript
sfdx force:org:create -s -f config/project-scratch-def.json -a GeoAppScratch
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

### Export and Import
__Export Data__

```javascript
sfdx force:data:tree:export -q "SELECT Name, Location__Latitude__s, Location__Longitude__s FROM Account WHERE Location__Latitude__s != NULL AND Location__Longitude__s != NULL" -d ./data
```

__Import Data__

```javascript 
sfdx force:data:tree:import --sobjecttreefiles data/Account.json
```


