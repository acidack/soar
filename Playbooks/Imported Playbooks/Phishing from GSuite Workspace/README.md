# Phishing from GSuite Workspace
Download file from GSuite Workspace, decode and save to case wall



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
|GSuite - Email Enterprise_Get Message By RFC Message ID_1|Get EML from GSuite|GSuite - Email Enterprise|Get Message By RFC Message ID|
|FileUtilities_Add Attachment-Fix_1|Save EML to case wall|FileUtilities|Add Attachment-Fix|

