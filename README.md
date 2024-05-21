# GitSync

## Integrations
|Name|Description|
|----|-----------|
|Active Directory|Microsoft Active Directory integration facilitates the centralized management and synchronization of Windows user accounts with Security Center's administrator and cardholder accounts.|
|Azure Active Directory|Azure Active Directory (Azure AD) is Microsoft’s cloud-based identity and access management service, which helps your employees sign in and access  both internal and external resources.|
|CrowdStrike Falcon|CrowdStrike Falcon is the leader in next-generation endpoint protection, threat intelligence and incident response through cloud-based endpoint protection.|
|EmailUtilities|A set of utility actions to assist with working with emails.  Includes actions to parse EMLs and analyze email headers.|
|EmailV2|Email integration over smtp and imap protocols|
|Enrichment|A set of entity enrichment actions to assist in the managing of entity attributes.|
|FileUtilities|A set of file utility actions created for Siemplify Community to power up playbook capabilities.|
|Functions|A set of math and data manipulation actions created for Siemplify Community to power up playbook capabilities.|
|Google Chronicle|Chronicle enables you to examine the aggregated security information for your enterprise going back for months or longer. Use Chronicle to search across all of the domains accessed from within your enterprise. To enable the Google API client to communicate with the Backstory API you will need Google Developer Service Account Credential, https://developers.google.com/identity/protocols/OAuth2#serviceaccount.|
|Lists|A set of tools to facilitate managing custom lists within Siemplify|
|MITRE ATT&CK™|MITRE ATT&CK™ is a globally-accessible knowledge base of adversary tactics and techniques based on real-world observations. The ATT&CK knowledge base is used as a foundation for the development of specific threat models and methodologies in the private sector, in government, and in the cybersecurity product and service community.|
|Netskope|The Netskope Security Cloud helps the world’s largest organizations take full advantage of the cloud and web without sacrificing security.|
|Okta|The Okta Identity Cloud provides secure identity management with Single Sign-On, Multi-factor Authentication, Lifecycle Management (Provisioning), and more.|
|Siemplify ThreatFuse|ThreatFuse combines best-in-class security orchestration, automation and response (SOAR) with a market-leading Threat Intelligence Platform (TIP) powered by Anomali, to make intelligence-driven security operations simple and accessible for organizations of all sizes.With robust integration out of the box, ThreatFuse ingrains threat-intelligence across the entire detection and response lifecycle. From enrichment with real-time threat indicators, through threat-hunting and intelligence sharing, security analysts can validate, investigate and respond to threats with unprecedented speed and precision.|
|Tools|A set of utility actions for data manipulation and common platform tasks to power up playbook capabilities.|
|VirusTotalV3|VirusTotal was founded in 2004 as a free service that analyzes files and URLs for viruses, worms, trojans and other kinds of malicious content. Our goal is to make the internet a safer place through collaboration between members of the antivirus industry, researchers and end users of all kinds. Fortune 500 companies, governments and leading security companies are all part of the VirusTotal community, which has grown to over 500,000 registered users.This integration was created using the 3rd iteration of VT API.|


## Connectors
|Name|Description|Has Mappings|
|----|-----------|------------|
|Google Chronicle - Chronicle Alerts Connector|Pull information about Rule based alerts from Google Chronicle. Note: dynamic list is used for filtering purposes. For all of the details please visit the documentation portal.|True|


## Playbooks
|Name|Description|
|----|-----------|
|Asset Enrichment|An embedded workflow that can receive inputs and return an output.|
|Enrich Hash|An embedded workflow that can receive inputs and return an output.|
|File Sandbox|An embedded workflow that can receive inputs and return an output.|
|Hash Enrichment VT|An embedded workflow that can receive inputs and return an output.|
|IOC Investigation|An embedded workflow that can receive inputs and return an output.|
|IOC_Investigation_Playbook||
|SIEM Investigation|An embedded workflow that can receive inputs and return an output.|
|Analyst View Hands On||
|Chronicle Hands On||
|IMPORT 1 - Analyst View Hands On||
|IMPORT 1 - Chronicle Hands On||
|IMPORT 1 - File Sandbox|An embedded workflow that can receive inputs and return an output.|
|Mitre|An embedded workflow that can receive inputs and return an output.|
|Phishing From Email|Download the EML files from the Email received by the Connector to a mailbox|
|Phishing From Manual Upload|The EML must be uploaded to the Case Wall before this playbook is attached|
|Phishing from GSuite Workspace|Download file from GSuite Workspace, decode and save to case wall|
|Phishing from SNOW Secops|Download file from SNOW SecOps(Download Attachment Action needs Validating for table records)|
|User Enrichment|Enrich Internal users for case context|


## Jobs
|Name|Description|
|----|-----------|
|Google Chronicle Sync Job|This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM. Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.|

