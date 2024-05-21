# User Enrichment
Enrich Internal users for case context



**Enabled:** True

**Version:** 0

**Type:** Block

**Priority:** 2

**Playbook Simulator:** True


##### Input Parameters
|Name|Default Value|
|----|-------------|
|simulate|true|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|ActiveDirectory_Enrich entities_1|Enrich Hostname or Username entities with Active Directory properties|ActiveDirectory|Enrich entities|
|get full user JSON|The action gets a key and value in a specific context (alert or case)|Tools|Get Context Value|
|AppendAD to user|The action gets a key and value in a specific context (alert or case)|Tools|Append to Context Value|
|GetInstances|Returns all the integration instances for an environment.|Tools|Get Integration Instances|
|Tools_Append to Context Value_3|The action gets a key and value in a specific context (alert or case)|Tools|Append to Context Value|
|Append Azure AD|The action gets a key and value in a specific context (alert or case)|Tools|Append to Context Value|
|AzureActiveDirectory_Enrich User_1|Enrich Siemplify User entity with information from Azure Active Directory. Action expects Siemplify user entity in username@domain format.|AzureActiveDirectory|Enrich User|
|Append GSuite|The action gets a key and value in a specific context (alert or case)|Tools|Append to Context Value|
|GSuite_Enrich Entities_1|Enrich Siemplify User entities with information from Google GSuite.|GSuite|Enrich Entities|
|Tools_Set Context Value_1|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|get simulated user|The action gets a key and value in a specific context (alert or case)|Tools|Get Context Value|

