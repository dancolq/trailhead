## Bulk Delete Records From a Csv File

The file must be a CSV file with only one column: "Id".

One job can contain many batches, depending on the length of the CSV file.

Returns a job ID and a batch ID. Use these IDs to check job status with data:bulk:status.



Option | Description
--- | --- 
```-f, --csvfile CSVFILE``` | the path to the csv file containing the ids of the records to delete
```-s, --sobjecttype SOBJECTTYPE``` | the sobject type of the records you’re deleting
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-w, --wait WAIT``` | the number of minutes to wait for the command to complete before displaying the results
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:data:bulk:delete -s Account -f ./path/to/file.csv

$ sfdx force:data:bulk:delete -s MyObject__c -f ./path/to/file.csv


