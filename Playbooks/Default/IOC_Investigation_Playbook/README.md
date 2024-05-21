# IOC_Investigation_Playbook




**Enabled:** True

**Version:** 0

**Type:** Playbook

**Priority:** 2

**Playbook Simulator:** False


### Playbook Trigger
**Trigger Type:** Alert Type

**Conditions Operator:** And

##### Conditions
|Key|Operator|Value|
|---|--------|-----|
||Equals|ExecutableDetected|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|CrowdStrikeFalcon_Contain Endpoint_1|Contain endpoint in Crowdstrike Falcon. Supported entities: Hostname and IP address.|CrowdStrikeFalcon|Contain Endpoint|
|Siemplify_Close Alert_1|Closes the current alert|Siemplify|Close Alert|
|Siemplify_Add General Insight_1|Add a general insight configurable message to the case|Siemplify|Add General Insight|
|Siemplify_Close Alert_2|Closes the current alert|Siemplify|Close Alert|

### Involved Blocks
|Name|Description|
|----|-----------|
|IOC Investigation|An embedded workflow that can receive inputs and return an output.|
|Asset Enrichment|An embedded workflow that can receive inputs and return an output.|
|IMPORT 1 - File Sandbox|An embedded workflow that can receive inputs and return an output.|
