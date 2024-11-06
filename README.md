# cloudsocapi

## Postman Collection for DLP Cloud
PROVIDED AS-IS

Version CloudSOC CASB 3.174 

### Set the Variables
- Open Postman and import the DLP Cloud collection (**_DLPCloud.postman.json_**).
- In the DLP Cloud collection (top level), click on **Variables**. You will find the following items:
```
cloudsoc_tenant_name
clouddlp_tenant_name
clouddlp_token
```
- Fill in the values for the first two variables (_cloudsoc_tenant_name_ and _clouddlp_tenant_name_) with the corresponding CloudSOC and/or Cloud DLP tenant identifiers, available in CloudSOC under **Settings > General**.  

### CloudSOC Folder
- The CloudSOC API supports **Basic Access Authentication**. Obtain the corresponding Username and Password values by following the process available here: https://techdocs.broadcom.com/us/en/symantec-security-software/information-security/symantec-cloudsoc/cloud/api-home/create-api-key.html.
- In Postman, go to the **CloudSOC** folder.
- Click on the **Authorization** Tab, and select **Basic Auth** as the **Type**.
- Use the key_id as the username and the key_secret as the password. The API keys are allocated on a per-user basis and inherit the permissions granted to that user.

### Cloud DLP Folder
- The Cloud DLP APIs require an ephemeral token. In this collection, the variable **_clouddlp_token_** can help you store the token for most API calls under this folder.
- You can also navigate to **DLP Cloud > Cloud DLP > API: Get Token** request and use CloudSOC's key_id and key_secret as explained here: https://techdocs.broadcom.com/us/en/symantec-security-software/information-security/symantec-cloudsoc/cloud/api-home/protect-api/api-encoded-key.html
Assign the value of the clouddlp_token variable accordingly.
