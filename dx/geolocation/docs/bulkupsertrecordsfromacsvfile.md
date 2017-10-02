## Bulk Upsert Records From a Csv File

Inserts or updates records from a CSV file.

One job can contain many batches, depending on the length of the CSV file.

Returns a job ID and a batch ID. Use these IDs to check job status with data:bulk:status.

For information about formatting your CSV file, see "Prepare CSV Files" in the Bulk API Developer Guide.



Option | Description
--- | --- 
```-f, --csvfile CSVFILE``` | the path to the csv file that defines the records to upsert
```-i, --externalid EXTERNALID``` | the column name of the external id; if not provided, an arbitrary id is used
```-s, --sobjecttype SOBJECTTYPE``` | the sobject type of the records you want to upsert
```-u, --targetusername TARGETUSERNAME``` | username for the target org; overrides default target org
```-w, --wait WAIT``` | the number of minutes to wait for the command to complete before displaying the results
```--json``` | format output as json
```--loglevel LOGLEVEL``` | logging level for this command invocation (error*,trace,debug,info,warn,fatal)


__Exmples:__ 

$ sfdx force:data:bulk:upsert -s MyObject__c -f ./path/to/file.csv -i MyField__c

$ sfdx force:data:bulk:upsert -s MyObject__c -f ./path/to/file.csv -i Id -w 2


