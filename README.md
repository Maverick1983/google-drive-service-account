# MyBag - 45TB on Google Drive for free
Use Google cloud Free Tier 1 to have 45 TB of cloud storage for free (https://cloud.google.com/free).

It is possible to use Google Cloud, for free, and use Google Drive up to 45 TB, through the Google IAM Service Accounts (https://cloud.google.com/iam/docs/service-accounts)

# Documentation
https://docs.google.com/document/d/1PEBrzBDQJRsKWTYnjzrp8eL1H7TzVQdIqrhLprTyrqs/edit?usp=sharing


Note
The owner account appears to be the one who uploaded the file. In other words, if a folder is shared by someone else, giving you read/write access to the folder, but you upload a 2GB file to it, then the 2GB file is owned by you and goes against your storage limit; not the storage limit of the folder owner.


# Project Creation
https://cloud.google.com/resource-manager/docs/creating-managing-projects
- It’s possible create 30 project
- Every project can have 100 Service Account
- Every Service Account can have 15 GB in Drive

# Total space on Drive with one Google Cloud account: (100 x 15) x 30 = 45 TB


# Creation Project’s Service Account
https://cloud.google.com/iam/docs/creating-managing-service-accounts#iam-service-accounts-create-rest

# Max 100 Service Account per Project
https://cloud.google.com/iam/docs/service-accounts 

# Creation Keys for Service Account
https://cloud.google.com/iam/docs/creating-managing-service-account-keys#iam-service-account-keys-create-rest 

# Adding role to the Project on Service Account
https://cloud.google.com/iam/reference/rest/v1/projects.serviceAccounts/setIamPolicy 
roles/owner

# Add rule to Resource Service Account
https://cloud.google.com/iam/docs/granting-roles-to-service-accounts#granting_access_to_a_service_account_for_a_resource
- roles/owner
- roles/servicemanagement.admin

# Enable Google Drive API
https://cloud.google.com/service-infrastructure/docs/service-management/reference/rest/v1/services/enable
- ServiceName: drive.googleapis.com


I will add a Windows Form project C#
