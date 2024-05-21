# IMPORT 1 - File Sandbox
An embedded workflow that can receive inputs and return an output.



**Enabled:** True

**Version:** 0

**Type:** Block

**Priority:** 2

**Playbook Simulator:** True


##### Input Parameters
|Name|Default Value|
|----|-------------|
|file_path|None|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|CrowdStrikeFalcon_Download File_1|Download files from the hosts in Crowdstrike Falcon. Supported entities: File Name, IP Address and Hostname. Note: action requires both File Name and IP Address/Hostname entity to be in the scope of the Siemplify alert. The downloaded file will be in password-protected zip. Password is "infected".|CrowdStrikeFalcon|Download File|
|FalconSandbox_Analyze File_1|Submit a file for analysis and fetch report|FalconSandbox|Analyze File|
|Create File Name Entity|Creates an entity and adds to requested alert. Note - Please make sure to read our documentation regarding the differences in the delimiter’s behavior, between different Siemplify’s platform versions 5.6.0 inclusive and 5.6.2 exclusive, here: https://cloud.google.com/chronicle/docs/soar/marketplace-integrations/siemplify#create-entity|Siemplify|Create Entity|

