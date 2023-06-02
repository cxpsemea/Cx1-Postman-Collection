This collection covers various parts of the Cx1 API:

- Basic user and group management
- Getting some data on applications, projects, scans, queries, presets
- Running scans, generating reports
- Creating and modifying queries
- Data import (including the new Project-to-Application mapping)

Instructions:

Import the collection (Cx1.postman_collection.json)
Import the environment (Cx1 EU Blank.postman_environment.json)

In Postman, in the Environments tab, either edit the imported Cx1 EU Blank or duplicate it and edit the copy

- set the correct IAM and Cx1 URLs for your region
- set the correct tenant and API Key 
- update other fields if desired but it should be good to go

Scripts are set up in each of the sections to pick up and persist variables as needed. For example, if you use the "Get Projects" request, the Project ID from the first project returned in the API response will be stored in a variable "Cx1_ProjectID". If you then use "Get Scans" it will default to retrieving the scans for the same Cx1_ProjectID. 