# Mitre
An embedded workflow that can receive inputs and return an output.



**Enabled:** True

**Version:** 0

**Type:** Block

**Priority:** 2

**Playbook Simulator:** False


##### Input Parameters
|Name|Default Value|
|----|-------------|
|additionalID|na|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Siemplify_Create Or Update Entity Properties_4|Create\Change properties for entities in an entity scope.|Siemplify|Create Or Update Entity Properties|
|Siemplify_Create Or Update Entity Properties_1|Create\Change properties for entities in an entity scope.|Siemplify|Create Or Update Entity Properties|
|Create ATT&CK ID|Creates an entity and adds to requested alert. Note - Please make sure to read our documentation regarding the differences in the delimiter’s behavior, between different Siemplify’s platform versions 5.6.0 inclusive and 5.6.2 exclusive, here: https://integrations.siemplify.co/doc/siemplify#create-entity|Siemplify|Create Entity|
|Siemplify_Create Or Update Entity Properties_3|Create\Change properties for entities in an entity scope.|Siemplify|Create Or Update Entity Properties|
|MitreAttck_Get Mitigations_1|Retrieve information about mitigations that are associated with MITRE attack technique|MitreAttck|Get Mitigations|
|Siemplify_Create Entity_1|Creates an entity and adds to requested alert|Siemplify|Create Entity|
|Siemplify_Create Or Update Entity Properties_2|Create\Change properties for entities in an entity scope.|Siemplify|Create Or Update Entity Properties|
|Tag MITRE ATT&CK|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|MitreAttck_Get Technique Details_1|Retrieve detailed information about MITRE attack technique|MitreAttck|Get Technique Details|
|MitreAttck_Get Techniques Mitigations_1|Retrieve information about mitigations that are associated with MITRE attack techniques.|MitreAttck|Get Techniques Mitigations|

