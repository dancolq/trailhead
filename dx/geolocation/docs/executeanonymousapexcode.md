## Execute Anonymous Apex Code

Executes one or more lines of Apex code, or executes the code in a local file.

Before you enter code, run this command with no parameters to get a prompt.

From the prompt, all commands are executed in a single execute anonymous request.

For more information, see "Anonymous Blocks" in the Apex Developer Guide.

>> Start typing Apex code. Press the Enter key after each line,

>> then press CTRL+D when finished.



Option | Description
--- | --- 
```-f, --apexcodefile APEXCODEFILE``` | path to a local file containing apex code
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:apex:execute -f ~/test.apex

$ sfdx force:apex:execute


