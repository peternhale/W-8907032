# W-8907032
Artifacts needed to reproduce W-8907032

- Clone repo
- Create a new org (Enterprise Edition)
- Auth to new org using sfdx
- run `sfdx force:source:deploy -p ./force-app -u <org username>`
- run `sfdx force:source:retrieve -p ./force-app -u <org username>`

Inspect the [businessProcesses folder](force-app/main/default/objects/Opportunity/businessProcesses) and one will find file `Test.recordType-meta.xml`. 
This file should be in [recordTypes](force-app/main/default/objects/Opportunity/recordTypes) folder.