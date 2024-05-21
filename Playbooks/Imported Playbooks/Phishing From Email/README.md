# Phishing From Email
Download the EML files from the Email received by the Connector to a mailbox



**Enabled:** True

**Version:** 0

**Type:** Block

**Priority:** 2

**Playbook Simulator:** False


##### Input Parameters
|Name|Default Value|
|----|-------------|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Exchange_Download Attachments_1|Download email attachments from email to specific file path on Siemplify server. NOTICE - to search for an email in all mailboxes, please configure impersonation permissions. https://docs.microsoft.com/en-us/exchange/client-developer/exchange-web-services/impersonation-and-ews-in-exchange. Note: Action is running as async, please adjust script timeout value in Siemplify IDE for action as needed. Additionally, please note that if the downloaded attachments have "/" or "\" characters in the names, those will be replaced with the '_' character.|Exchange|Download Attachments|
|Exchange_Send Mail_1||Exchange|Send Mail|
|EmailV2_Send Email_1|Send email message. Requires: SMTP configuration|EmailV2|Send Email|
|Siemplify_Close Alert_2|Closes the current alert|Siemplify|Close Alert|
|EmailV2_DownloadEmailAttachments_1|Download email attachments from email to specific file path on Siemplify server. Requires: IMAP configuration|EmailV2|DownloadEmailAttachments|
|EmailUtilities_Parse Case Wall Email_1|This action will parse an EML or MSG file that has been attached to the case wall.|EmailUtilities|Parse Case Wall Email|
|Siemplify_Close Alert_1|Closes the current alert|Siemplify|Close Alert|
|Tools_Change Case Name_1|The action changes the case's name (title)|Tools|Change Case Name|

