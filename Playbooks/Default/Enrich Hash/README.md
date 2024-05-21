# Enrich Hash
An embedded workflow that can receive inputs and return an output.



**Enabled:** True

**Version:** 1

**Type:** Block

**Priority:** 2

**Playbook Simulator:** False


##### Input Parameters
|Name|Default Value|
|----|-------------|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|CrowdStrikeFalcon_Get Host Information_1|Retrieve information about the hostname from Crowdstrike Falcon. Supported entities: Hostname, IP Address.|CrowdStrikeFalcon|Get Host Information|
|AzureActiveDirectory_Enrich Host_1|Enrich Siemplify Host entity with information from Azure Active Directory. Action finds a match for a provided Host entity based on the devices displayName field in Azure AD|AzureActiveDirectory|Enrich Host|
|AzureActiveDirectory_Enrich User_1|Enrich Siemplify User entity with information from Azure Active Directory. Action expects Siemplify user entity in username@domain format.|AzureActiveDirectory|Enrich User|
|CrowdStrikeFalcon_List Host Vulnerabilities_1|List vulnerabilities found on the host in Crowdstrike Falcon. Supported entities: IP Address and Hostname. Note: requires Falcon Spotlight license and permissions. |CrowdStrikeFalcon|List Host Vulnerabilities|

