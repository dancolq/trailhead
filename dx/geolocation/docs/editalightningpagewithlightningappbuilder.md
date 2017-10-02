## Edit a Lightning Page With Lightning App Builder

If Force.com IDE 2 is installed, the file opens in an embedded browser within the IDE. If Force.com IDE 2 isn’t installed, the file opens in your default browser.

If no browser-based editor is available for the selected file, this command opens your org’s home page.

To generate a URL for the browser-based editor but not open the editor, use --urlonly.



Option | Description
--- | --- 
```-f, --sourcefile SOURCEFILE``` | file to edit
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-r, --urlonly``` | generate a navigation url; don’t launch the editor
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

```
$ sfdx force:source:open -f Property_Record_Page.flexipage-meta.xml

$ sfdx force:source:open -f Property_Record_Page.flexipage-meta.xml -r

```

