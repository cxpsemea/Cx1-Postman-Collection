This collection covers the following basic interactions with the Cx1 REST API:
- Get & create projects
- Get a list of applications, scans, queries, presets
- Start a scan using the zip-upload method
- Get a list of users & groups, add a user to a group, create a group (requires using the API Key authentication approach)
- Generate and retrieve a PDF report

GET  {{Cx1_URL}}/api/projects
POST {{{Cx1_URL}}/api/projects
GET {{Cx1_URL}}/api/applications
GET {{Cx1_URL}}/api/scans
GET {{Cx1_URL}}/api/sast-rm/scans
GET {{Cx1_URL}}/api/scans/:scanid
GET {{Cx1_URL}}/api/sast-metadata/:scanid
GET {{Cx1_URL}}/api/results/
GET {{Cx1_URL}}/api/sast-results/
GET {{Cx1_URL}}/api/queries
GET {{Cx1_URL}}/api/queries/presets
GET {{Cx1_URL}}/api/presets
GET {{Cx1_URL}}/api/presets/queries
GET {{Cx1_IAM}}/auth/realms/{{Cx1_Tenant}}/users
GET {{Cx1_IAM}}/auth/admin/realms/{{Cx1_Tenant}}/users/:userid/groups
PUT {{Cx1_IAM}}/auth/admin/realms/{{Cx1_Tenant}}/users/:userid/groups/:groupId
GET {{Cx1_IAM}}/auth/admin/realms/{{Cx1_Tenant}}/groups
GET {{Cx1_IAM}}/auth/admin/realms/{{Cx1_Tenant}}/groups/:groupId/members
POST {{{Cx1_IAM}}/auth/admin/realms/{{Cx1_Tenant}}/groups
GET {{Cx1_URL}}/api/queries/descriptions?ids=1
GET {{Cx1_URL}}/api/webhooks/projects/:projectid
POST {{Cx1_URL}}/api/uploads
PUT {{Cx1_UploadURI}}
POST {{{Cx1_URL}}/api/scans/
POST {{{Cx1_URL}}/api/reports
GET {{Cx1_URL}}/api/reports/:reportId
GET {{Cx1_ReportURL}}
POST {{Cx1_IAM}}/auth/realms/{{Cx1_Tenant}}/protocol/openid-connect/token
POST {{Cx1_IAM}}/auth/realms/{{Cx1_Tenant}}/protocol/openid-connect/token
