# IOC Investigation
An embedded workflow that can receive inputs and return an output.



**Enabled:** True

**Version:** 0

**Type:** Block

**Priority:** 2

**Playbook Simulator:** True


##### Input Parameters
|Name|Default Value|
|----|-------------|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|VirusTotalV3_Enrich Hash_1|Enrich Hash using information from VirusTotal. Supported entities: Filehash. Note: only MD5, SHA-1 and SHA-256 are supported.|VirusTotalV3|Enrich Hash|
|False Positive|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Malicious File Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|

