# Chronicle Hands On




**Enabled:** False

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
||Equals|cs_edr_repeated_auth_failure|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|GoogleChronicle_Lookup Similar Alerts_1|Lookup similar alerts in Google Chronicle. Supported Chronicle alert types: RULE, EXTERNAL, IOC. Note: this action can only work with alerts that come from the "Chronicle Alerts Connector". Note: action can only fetch 10000 alerts. Make sure to narrow down the timeframe for better results.|GoogleChronicle|Lookup Similar Alerts|
|GoogleChronicle_List Events_1|List events on the particular asset in the specified time frame. Supported entities: IP Address, Mac Address, Hostname. Note: action can only fetch 10000 events. Make sure to narrow down the timeframe for better results.|GoogleChronicle|List Events|
|GoogleChronicle_List Assets_1|List assets in Google Chronicle based on the related entities in the specified time frame. Supported entities: URL, IP Address, File hash. Only MD5, SHA-1 or SHA-256 hashes are supported.|GoogleChronicle|List Assets|

