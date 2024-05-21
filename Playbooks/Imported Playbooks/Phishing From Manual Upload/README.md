# Phishing From Manual Upload
The EML must be uploaded to the Case Wall before this playbook is attached



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
|Siemplify_Close Alert_1|Closes the current alert|Siemplify|Close Alert|
|EmailUtilities_Parse Case Wall Email_1|This action will parse an EML or MSG file that has been attached to the case wall.|EmailUtilities|Parse Case Wall Email|
|Tools_Change Case Name_1|The action changes the case's name (title)|Tools|Change Case Name|

