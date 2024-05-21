<p align="center"><img src="./Resources/CrowdStrikeFalcon.svg" 
     alt="CrowdStrikeFalcon" width="200"/></p>

# CrowdStrikeFalcon

CrowdStrike Falcon is the leader in next-generation endpoint protection, threat intelligence and incident response through cloud-based endpoint protection.

Python Version - 2
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|None|False|String|https://api.crowdstrike.com|
|Client API ID|None|True|String||
|Client API Secret|None|True|Password|None|
|Verify SSL|None|False|Boolean|False|


#### Dependencies
| |
|-|
|cross/six-1.16.0-py2.py3-none-any.whl|
|cross/TIPCommon-1.1.0.1-py2.py3-none-any.whl|
|cross/charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|cross/EnvironmentCommon-1.0.1-py2.py3-none-any.whl|
|cross/certifi-2020.12.5-py2.py3-none-any.whl|
|cross/rsa-4.8-py3-none-any.whl|
|cross/requests-2.28.2-py3-none-any.whl|
|cross/cachetools-5.0.0-py3-none-any.whl|
|cross/google_auth-2.5.0-py2.py3-none-any.whl|
|cross/filelock-3.0.12-py3-none-any.whl|
|cross/requests_file-1.5.1-py2.py3-none-any.whl|
|cross/pyasn1-0.4.8-py2.py3-none-any.whl|
|cross/pyasn1_modules-0.2.8-py2.py3-none-any.whl|
|cross/TIPCommon-1.0.10-py3-none-any.whl|
|cross/TIPCommon-1.0.11-py2.py3-none-any.whl|
|cross/urllib3-1.26.15-py2.py3-none-any.whl|
|cross/chardet-4.0.0-py2.py3-none-any.whl|
|cross/TIPCommon-1.0.12-py2.py3-none-any.whl|
|cross/requests_toolbelt-0.10.1-py2.py3-none-any.whl|
|cross/idna-2.8-py2.py3-none-any.whl|
|cross/tldextract-3.1.0-py2.py3-none-any.whl|


## Actions
#### List Hosts
List available hosts in Crowdstrike Falcon.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter Logic|Specify what logic should be used, when searching for hosts.|False|List|Equal|
|Filter Value|Specify the value that should be used to filter hosts.|False|String||
|Max Hosts To Return|Specify how many hosts to return. Default: 50. Maximum: 1000.|False|String|50|



##### JSON Results
```json
[{"modified_timestamp":"2019-05-15T15:03:12Z","platform_id":"0","config_id_platform":"3","system_manufacturer":"Microsoft Corporation","meta":{"version":"XXXX"},"first_seen":"2019-04-29T07:39:45Z","service_pack_minor":"0","product_type_desc":"Server","build_number":"XXXX","hostname":"Gnrl-Elis","config_id_build":"XXXX","minor_version":"3","os_version":"Windows Server XXXXX","provision_status":"Provisioned","mac_address":"XXXXXXXXX","bios_version":"XXXXX ","agent_load_flags":"0","status":"normal","bios_manufacturer":"American Megatrends Inc.","device_policies":{"sensor_update":{"applied":true,"applied_date":"2019-05-02T22:05:09.577000651Z","settings_hash":"XXXXXXXXXXXXXXXXXXXXX","policy_type":"sensor-update","assigned_date":"2019-05-02T22:03:36.804382667Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXX"},"remote_response":{"applied":true,"applied_date":"2019-04-29T07:40:04.469808388Z","settings_hash":"XXXXXXXX","policy_type":"remote-response","assigned_date":"2019-04-29T07:39:55.218642441Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXX"},"device_control":{"applied":true,"applied_date":"2019-04-29T07:40:06.834362608Z","assigned_date":"2019-04-29T07:39:55.214337999Z","policy_type":"device-control","policy_id":"XXXXXXXXXXXXXXXXXXXXXX"},"prevention":{"applied":true,"applied_date":"2019-04-29T07:40:06.876850888Z","settings_hash":"XXXXXXXXXXXXXXXXXXXXXX","policy_type":"prevention","assigned_date":"2019-04-29T07:39:55.218651583Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXX"},"global_config":{"applied":true,"applied_date":"2019-04-29T07:45:18.94807838Z","settings_hash":"XXXXXXXXXXXXXXXXXXXXXXXXX","policy_type":"globalconfig","assigned_date":"2019-04-29T07:45:08.165941325Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXX"}},"cid":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXx","agent_local_time":"2019-05-02T22:05:00.015Z","slow_changing_modified_timestamp":"2019-05-02T22:05:09Z","service_pack_major":"0","device_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXX","system_product_name":"Virtual Machine","product_type":"3","local_ip":"1.1.1.1","external_ip":"1.1.1.1","major_version":"6","platform_name":"Windows","config_id_base":"XXXXXXXXXXXXXXXXXXX","policies":[{"applied":true,"applied_date":"2019-04-29T07:40:06.876850888Z","settings_hash":"XXXXXXXXXXXXXXXXXXXXXX","policy_type":"prevention","assigned_date":"2019-04-29T07:39:55.218651583Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXX"}],"agent_version":"4.26.XXXX.0","pointer_size":"8","last_seen":"2019-05-15T15:01:23Z"},{"modified_timestamp":"2019-05-13T07:24:36Z","site_name":"Default-First-Site-Name","config_id_platform":"3","system_manufacturer":"Dell Inc.","meta":{"version":"XXXXXX"},"first_seen":"2018-04-17T11:02:20Z","platform_name":"Windows","service_pack_minor":"0","product_type_desc":"Workstation","build_number":"XXXXXXXXXX","hostname":"XXXXXXXXXXX","config_id_build":"XXXX","minor_version":"0","os_version":"Windows 10","provision_status":"Provisioned","mac_address":"XXXXXXXXXXXXXXXXX","bios_version":"1.6.5","agent_load_flags":"0","status":"normal","bios_manufacturer":"Dell Inc.","machine_domain":"SIEMPLIFY.LOCAL","device_policies":{"sensor_update":{"applied":true,"applied_date":"2019-05-05T12:52:23.121596885Z","settings_hash":"XXXXXXXXXXXXXXXXXXXXX","policy_type":"sensor-update","assigned_date":"2019-05-05T12:51:37.544605747Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXX"},"remote_response":{"applied":true,"applied_date":"2019-02-10T07:57:59.064362539Z","settings_hash":"XXXXXXXX","policy_type":"remote-response","assigned_date":"2019-02-10T07:57:50.610924385Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXX"},"device_control":{"applied":true,"applied_date":"2019-03-25T15:01:28.51681072Z","assigned_date":"2019-03-25T15:00:22.442519168Z","policy_type":"device-control","policy_id":"XXXXXXXXXXXXXXXXXXXXXX"},"prevention":{"applied":true,"applied_date":"2019-04-04T06:54:06.909774295Z","settings_hash":"XXXXXXXXXXXXXXXXXXXXXX","policy_type":"prevention","assigned_date":"2019-04-04T06:53:57.135897343Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXX"},"global_config":{"applied":true,"applied_date":"2019-02-10T07:57:53.70275875Z","settings_hash":"XXXXXXXXXXXXXXXXXXXXXXXXX","policy_type":"globalconfig","assigned_date":"2019-02-10T07:57:50.610917888Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXX"}},"cid":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXx","agent_local_time":"2019-05-05T15:52:08.172Z","slow_changing_modified_timestamp":"2019-05-12T12:37:35Z","service_pack_major":"0","device_id":"XXXXXXXXXXXXXXXXXXXXX","system_product_name":"Latitude XXXX","product_type":"1","local_ip":"1.1.1.1","external_ip":"1.1.1.1","major_version":"10","platform_id":"0","config_id_base":"XXXXXXXXXXXXXXXXXXX","policies":[{"applied":true,"applied_date":"2019-04-04T06:54:06.909774295Z","settings_hash":"XXXXXXXXXXXXXXXXXXXXXX","policy_type":"prevention","assigned_date":"2019-04-04T06:53:57.135897343Z","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXX"}],"agent_version":"4.26.XXXX.0","pointer_size":"8","last_seen":"2019-05-13T07:21:30Z"}]
```



#### Download File
Download files from the hosts in Crowdstrike Falcon. Supported entities: File Name, IP Address and Hostname. Note: action requires both File Name and IP Address/Hostname entity to be in the scope of the Siemplify alert. The downloaded file will be in password-protected zip. Password is "infected".
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Download Folder Path|Specify the path to the folder, where you want to store the threat file.|True|String||
|Overwrite|If enabled, action will overwrite the file with the same name.|False|Boolean|false|



##### JSON Results
```json
{"absolute_paths":["/opt/file_1","opt_file_2"]}
```



#### Update Incident
Update incident in Crowdstrike.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Incident ID|Specify the ID of the incident that needs to be updated.|True|String||
|Status|Specify the status for the incident.|False|List||
|Assign to|Specify the name or email of the analyst to whom the incident needs to be assigned. If "Unassign" is provided, action will remove assignment from the incident. Note: for name you need to provide first and last name of the analyst in the following format "{first name} {last name}"|False|String||



##### JSON Results
```json
[{"incident_id": "inc:466a00b13a5e4a9a9x.ac1a5e:x.x.x.", "incident_type": 1, "cid": "27fe4e476ca3490b6b2b6650e5a74", "host_ids": ["466a00b13a5e4a9a93ce2aca5eac1a5e"], "hosts": [{"device_id": "466a00b13a5e4a9a93ce2aca5eac1a5e", "cid": "27fe4e476ca34dd90b8476b2b6650e5a74", "agent_load_flags": "0", "agent_local_time": "2023-09-25T15:41:40.130Z", "agent_version": "7.01.17312.0", "bios_manufacturer": "VMware, Inc.", "bios_version": "VMW71.00V.17369862.B64.2012240522", "config_id_base": "65994753", "config_id_build": "17312", "config_id_platform": "3", "external_ip": "35.246.203.0", "hostname": "EX16-AD01", "first_seen": "2023-01-20T00:40:31Z", "last_seen": "2023-10-06T07:19:50Z", "local_ip": "172.30.3.162", "mac_address": "00-50-56-a2-94-8d", "machine_domain": "exlab.local", "major_version": "10", "minor_version": "0", "os_version": "Windows Server 2016", "ou": ["Domain Controllers"], "platform_id": "0", "platform_name": "Windows", "product_type": "2", "product_type_desc": "Domain Controller", "site_name": "Default-First-Site-Name", "status": "contained", "system_manufacturer": "VMware, Inc.", "system_product_name": "VMware7,1", "groups": ["9489d65c343244169627dcbc"], "modified_timestamp": "2023-10-06T07:19:58Z"}], "created": "2023-10-06T07:20:51Z", "start": "2023-10-06T07:19:21Z", "end": "2023-10-06T07:30:27Z", "state": "closed", "assigned_to": "67494-b86d-4a55-9e52-7492449400a1", "assigned_to_name": "Yuriy Landovskyy", "status": 30, "tactics": ["Persistence", "Defense Evasion", "Command and Control", "Credential Access", "Malware", "Privilege Escalation"], "techniques": ["Create Account", "Masquerading", "Ingress Tool Transfer", "OS Credential Dumping", "Malicious File", "Image File Execution Options Injection", "Bypass User Account Control", "Accessibility Features", "Registry Run Keys / Startup Folder"], "objectives": ["Keep Access", "Contact Controlled Systems", "Gain Access", "Falcon Detection Method"], "modified_timestamp": "2023-10-20T08:34:07.078440797Z", "users": ["EX16-AD01$", "administrator"], "fine_score": 100}]
```



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Get Hosts by IOC
DEPRECATED. List hosts related to the IOCs in Crowdstrike Falcon. Supported entities: Hostname, URL, IP address and Hash. Note: Hostname entities are treated as domain IOCs and action will extract domain part out of URLs. Only MD5 and SHA-256 hashes are supported.
Timeout - 600 Seconds



##### JSON Results
```json
{"hash": [{"modified_timestamp": "2019-01-17T13: 44: 57Z", "major_version": "10", "site_name": "Default-First-Site-Name", "platform_id": "0", "config_id_platform": "3", "system_manufacturer": "DellInc.", "meta": {"version": "49622"}, "first_seen": "2018-04-22T13: 06: 53Z", "service_pack_minor": "0", "product_type_desc": "Workstation", "build_number": "14393", "hostname": "name", "config_id_build": "8104", "minor_version": "0", "os_version": "Windows10", "provision_status": "Provisioned", "mac_address": "64-00-6a-2a-43-3f", "bios_version": "1.2.1", "agent_load_flags": "1", "status": "normal", "bios_manufacturer": "DellInc.", "machine_domain": "domain name", "device_policies": {"sensor_update": {"applied": true, "applied_date": "2018-12-11T23: 09: 18.071417837Z", "settings_hash": "65994753|3|2|automatic", "policy_type": "sensor-update", "assigned_date": "2018-12-11T23: 08: 38.16990705Z", "policy_id": "gdfgdghdhdhf53535"}}, "agent_local_time": "2019-01-14T19: 41: 09.738Z", "slow_changing_modified_timestamp": "2019-01-14T17: 44: 40Z", "service_pack_major": "0", "device_id": "2653595a063e4566519ef4fc813fcc56", "system_product_name": "OptiPlex7040", "product_type": "1", "local_ip": "1.1.1.1", "external_ip": "1.1.1.1", "cid": "27fe4e476ca3490b8476b2b6650e5a74", "platform_name": "Windows", "config_id_base": "65994753", "policies": [{"applied": true, "applied_date": "2019-01-02T22: 45: 21.315392338Z", "settings_hash": "18db1203", "policy_type": "prevention", "assigned_date": "2019-01-02T22: 45: 11.214774996Z", "policy_id": "7efdf97d7805402186b61151e8abd745"}], "last_seen": "2019-01-17T13: 44: 46Z", "pointer_size": "8", "agent_version": "4.18.8104.0"}]}
```



#### Upload IOCs
Add custom IOCs in Crowdstrike Falcon. Supported entities: Hostname, URL, IP address and Hash. Note: Hostname entities are treated as domain IOCs and action will extract domain part out of URLs. Only MD5 and SHA-256 hashes are supported.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Platform|Specify a comma-separated list of the platforms related to the IOC. Possible values: Windows, Linux, Mac.|True|String|Windows,Linux,Mac|
|Severity|Specify the severity for the IOC.|True|List|Medium|
|Comment|Specify a comment with more context related to IOC.|False|String||
|Host Group Name|Specify the name of the host group.|False|String||
|Action|Specify the action for the uploaded IOCs. Note: "Block" action can only be applied to hashes. Action will always apply "Detect" policy to all other IOC types.|False|List|Detect|



#### List Uploaded IOCs
List available custom IOCs in CrowdStrike Falcon.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|IOC Type Filter|Specify a comma-separated list of IOC types that should be returned. If nothing is provided, action will return IOCs from all types. Possible values: ipv4,ipv6,md5,sha256,domain.|False|String|ipv4,ipv6,md5,sha256,domain|
|Value Filter Logic|Specify the value filter logic. If "Equal" is selected, action will try to find the exact match among IOCs and if "Contains" is selected, action will try to find IOCs that contain that substring.|False|List|Equal|
|Value Filter String|Specify the string that should be searched among IOCs.|False|String||
|Max IOCs To Return|Specify how many IOCs to return. Default: 50. Maximum: 500.|False|String|50|



##### JSON Results
```json
[{"id":"6b2987ace3c0f5dbfa5414fa13e7302bc61cca5a5db6cde8e1d135xxxxxxxxxx","type":"sha256","value":"908b64b1971a979c7e3e8ce4621945cba84854cb98d76367b791a6xxxxxxxxxx","source":"testSource","action":"detect","severity":"medium","description":"test description update","metadata":{"company_name":"Microsoft Corporation","original_filename":"PowerShell.EXE","file_version":"10.0.18362.1 (WinBuild.160101.0800)","file_description":"Windows PowerShell","product_name":"Microsoft® Windows® Operating System","product_version":"10.0.18362.1","signed":false,"av_hits":0},"platforms":["windows","mac","linux"],"tags":["f09f1a25-e6d0-4709-a105-05xxxxxxxxxx"],"expiration":"2022-05-01T12:00:00Z","expired":false,"deleted":false,"applied_globally":true,"from_parent":false,"created_on":"2021-02-15T11:36:58Z","created_by":"","modified_on":"2021-10-13T09:42:13.466234223Z","modified_by":"7fff03c3227242a0bae84bxxxxxxxxxx"},{"id":"fbe8c2739f3c6df95e62e0ae54569974437b2d9306eaf6740134ccxxxxxxxxxx","type":"sha256","value":"8a86c4eecf12446ff273afc03e1b3a09a911d0b7981db1af58cb45xxxxxxxxxx","action":"no_action","severity":"","metadata":{"signed":false,"av_hits":-1},"platforms":["windows"],"tags":["Hashes 22.Nov.20 15:29 (Windows)"],"expired":false,"deleted":false,"applied_globally":true,"from_parent":false,"created_on":"2021-04-22T03:54:09.235120463Z","created_by":"internal@crowdstrike.com","modified_on":"2021-04-22T03:54:09.235120463Z","modified_by":"internal@crowdstrike.com"}]
```



#### List Host Vulnerabilities
List vulnerabilities found on the host in Crowdstrike Falcon. Supported entities: IP Address and Hostname. Note: requires Falcon Spotlight license and permissions. 
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Vulnerabilities To Return|Specify how many vulnerabilities to return per host. If nothing is provided action will process all of the related vulnerabilities.|False|String|100|
|Severity Filter|Specify the comma-separated list of severities for vulnerabilities.If nothing is provided, action will ingest all related vulnerabilities. Possible values: Critical, High, Medium, Low, Unknown.|False|String||
|Create Insight|If enabled, action will create an insight per entity containing statistical information about related vulnerabilities.|False|Boolean|true|



##### JSON Results
```json
{"Entity":"XXX.XXX.XXX","EntityResult": {"statistics":{"total":123,"severity":{"critical":1,"high":1,"medium":1,"low":1,"unknown":1},"status":{"open":1,"reopened":1},"total_available_remediations":1},"details":[{"id":"74089e36ac3XXXXXab14abc076ed18eb_fff6dXXXXXX7352babdf7c7d240749e7","cid":"27fe4e476cXXXXXX8476b2b6650e5a74","aid":"74089e36acXXXXXXab14abc076ed18eb","created_timestamp":"2021-05-12T22:45:47Z","updated_timestamp":"2021-05-12T22:45:47Z","status":"open","cve":{"id":"CVE-2021-28476","base_score":9.9,"severity":"CRITICAL","exploit_status":0},"app":{"product_name_version":"Windows Windows 10"},"apps":[{"product_name_version":"Windows Windows 10","sub_status":"open","remediation":{"ids":["acc34cd461023ffXXXXX420fa8839365"]}}],"host_info":{"hostname":"CROWDSTRIKE-H01","local_ip":"172.30.202.33","machine_domain":"","os_version":"Windows 10","ou":"","site_name":"","system_manufacturer":"VMware, Inc.","groups":[],"tags":[],"platform":"Windows"},"remediation":[{"id":"acc34cd461023ffXXXXX420fa8839365","reference":"KB5003169","title":"Update Microsoft Windows 10 1909","action":"Install patch for Microsoft Windows 10 1909 x64 (Workstation): Security Update KB5003169","link":"https://catalog.update.microsoft.com/v7/site/Search.aspx?q=KB5003169"}]}]}}
```



#### Get Host Information
Retrieve information about the hostname from Crowdstrike Falcon. Supported entities: Hostname, IP Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Create Insight|If enabled, action will create insights containing information regarding entities.|False|Boolean|true|



##### JSON Results
```json
[{"EntityResult":[{"modified_timestamp":"2019-01-17T13: 44: 57Z","major_version":"10","site_name":"Default-First-Site-Name","platform_id":"0","config_id_platform":"3","system_manufacturer":"DellInc.","meta":{"version":"1111"},"first_seen":"2018-04-22T13: 06: 53Z","service_pack_minor":"0","product_type_desc":"Workstation","build_number":"111","hostname":"name","config_id_build":"8104","minor_version":"0","os_version":"Windows10","provision_status":"Provisioned","mac_address":"64-00-6a-2a-43-3f","bios_version":"1.2.1","agent_load_flags":"1","status":"normal","bios_manufacturer":"DellInc.","machine_domain":"Domain name","agent_local_time":"2019-01-14T19: 41: 09.738Z","slow_changing_modified_timestamp":"2019-01-14T17: 44: 40Z","service_pack_major":"0","device_id":"2653595a063e4566519ef4fc813xxxx","system_product_name":"OptiPlex7040","product_type":"1","local_ip":"1.1.x.x","external_ip":"1.1.x.x","cid":"27fe4e476ca3490b8476b2b66xxxx","platform_name":"Windows","config_id_base":"65994753","last_seen":"2019-01-17T13: 44: 46Z","pointer_size":"8","agent_version":"4.18.8104.0","recent_logins":[{"user_name":"test","login_time":"2022-08-10T07:36:38Z"},{"user_name":"test","login_time":"2022-08-10T07:36:35Z"}],"online_status":"offline"}],"Entity":"1.1.x.x"}]
```



#### Execute Command
Execute commands on the hosts in Crowdstrike Falcon. Supported entities: IP Address and Hostname.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Command|Specify what command to execute on the hosts.|True|String||
|Admin Command|If enabled, action will execute commands with the admin level permissions. This is necessary for certain commands like "put".|False|Boolean|false|



##### JSON Results
```json
{"Entity":"XXX.XXX.XXX","EntityResult":{"session_id":"2a066818-XXXX-XXXX-XXXX-c295ed7295b3","task_id":"84846f59-XXXX-XXXX-XXXX-12af4af88a8b","complete":true,"stdout":"","stderr":"","base_command":"get"}}
```



#### Lift Contained Endpoint
Lift endpoint containment in Crowdstrike Falcon. Supported entities: Hostname and IP address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Fail If Timeout|If enabled, action will be failed, if containment was not lifted on all endpoints.|False|Boolean|true|



##### JSON Results
```json
{"Entity":"XXX.XXX.XXX","EntityResult":{"device_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","cid":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","agent_load_flags":"1","agent_local_time":"2021-05-26T11:54:38.105Z","agent_version":"X.XXX.XXX.0","bios_manufacturer":"Phoenix Technologies LTD","bios_version":"6.00","build_number":"XXXX","config_id_base":"XXXX","config_id_build":"XXXX","config_id_platform":"3","cpu_signature":"XXXXX","external_ip":"XXX.XXX.XXX.XXX","mac_address":"XX-XX-XX-XX-XX-XX","hostname":"XXXXXXXXXXXX","first_seen":"2021-01-12T16:01:43Z","last_seen":"2021-05-26T12:46:53Z","local_ip":"XXX.XXX.X.XX","major_version":"10","minor_version":"0","os_version":"Windows 10","platform_id":"0","platform_name":"Windows","policies":[{"policy_type":"prevention","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"71932dc2","assigned_date":"2021-02-05T10:17:18.181166503Z","applied_date":"2021-02-05T10:17:29.147610493Z","rule_groups":[]}],"reduced_functionality_mode":"no","device_policies":{"prevention":{"policy_type":"prevention","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"71932dc2","assigned_date":"2021-02-05T10:17:18.181166503Z","applied_date":"2021-02-05T10:17:29.147610493Z","rule_groups":[]},"sensor_update":{"policy_type":"sensor-update","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"tagged|1;101","assigned_date":"2021-05-20T13:21:15.793890625Z","applied_date":"2021-05-20T13:23:10.339303233Z","uninstall_protection":"ENABLED"},"device_control":{"policy_type":"device-control","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"assigned_date":"2021-01-12T16:05:30.418267934Z","applied_date":"2021-01-12T16:07:29.124988572Z"},"global_config":{"policy_type":"globalconfig","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"f61a5761","assigned_date":"2021-05-26T08:56:57.749380428Z","applied_date":"2021-05-26T08:57:09.08333925Z"},"remote_response":{"policy_type":"remote-response","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"XXXXXXX","assigned_date":"2021-01-12T16:05:30.418259588Z","applied_date":"2021-01-12T16:05:41.768614744Z"},"firewall":{"policy_type":"firewall","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"assigned_date":"2021-01-12T16:05:30.41820681Z","applied_date":"2021-01-12T16:07:35.656641903Z","rule_set_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"}},"groups":[],"group_hash":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","product_type":"1","product_type_desc":"Workstation","provision_status":"Provisioned","serial_number":"VMware-XX XX XX XX XX XX XX XX-XX XX XX XX XX XX XX XX","service_pack_major":"0","service_pack_minor":"0","pointer_size":"8","status":"normal","system_manufacturer":"VMware, Inc.","system_product_name":"VMware Virtual Platform","tags":[],"modified_timestamp":"2021-05-26T12:46:59Z","slow_changing_modified_timestamp":"2021-05-26T08:54:51Z","meta":{"version":"XXXXX"}}}
```



#### Update IOC Information
Update information about custom IOCs in Crowdstrike Falcon. Supported entities: Hostname, URL, IP address and Hash. Note: Hostname entities are treated as domain IOCs and action will extract domain part out of URLs. Only MD5 and SHA-256 hashes are supported.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Description|Specify a new description for custom IOCs.|False|Content||
|Source|Specify the source for custom IOCs.|False|Content||
|Expiration days|Specify the amount of days till expiration.|False|String||
|Detect policy|If enabled, IOCs that have been identifed, will send a notification. In other case, no action will be taken|False|Boolean||



##### JSON Results
```json
[{"Entity":"69630e4574ec6798239b09xxxxxxxxxx","EntityResult":{"id":"1cbca683ca9575609567419287aa92fba40f3ffee8badf6738f2c1xxxxxxxxxx","type":"md5","value":"69630e4574ec6798239b09xxxxxxxxxx","source":"test","action":"no_action","severity":"","description":"test","platforms":["windows","mac","linux"],"tags":["a7829d13-1d10-4126-9970-60xxxxxxxxxx"],"expiration":"2021-10-19T13:04:22Z","expired":false,"deleted":false,"applied_globally":true,"from_parent":false,"created_on":"2019-04-29T07:15:48Z","created_by":"","modified_on":"2021-10-14T13:04:23.666091115Z","modified_by":"7fff03c3227242a0bae84bxxxxxxxxxx"}},{"Entity":"908b64b1971a979c7e3e8ce4621945cba84854cb98d76367b791a6xxxxxxxxxx","EntityResult":{"id":"6b2987ace3c0f5dbfa5414fa13e7302bc61cca5a5db6cde8e1d135xxxxxxxxxx","type":"sha256","value":"908b64b1971a979c7e3e8ce4621945cba84854cb98d76367b791a6xxxxxxxxxx","source":"test","action":"detect","severity":"medium","description":"test","metadata":{"company_name":"Microsoft Corporation","original_filename":"PowerShell.EXE","file_version":"10.0.18362.1 (WinBuild.160101.0800)","file_description":"Windows PowerShell","product_name":"Microsoft® Windows® Operating System","product_version":"10.0.18362.1","signed":false,"av_hits":0},"platforms":["windows","mac","linux"],"tags":["f09f1a25-e6d0-4709-a105-05xxxxxxxxxx"],"expiration":"2021-10-19T13:04:26Z","expired":false,"deleted":false,"applied_globally":true,"from_parent":false,"created_on":"2021-02-15T11:36:58Z","created_by":"","modified_on":"2021-10-14T13:04:28.074605009Z","modified_by":"7fff03c3227242a0bae84bxxxxxxxxxx"}}]
```



#### Get Process Name By IOC
DEPRECATED. Retrieve processes related to the IOCs and provided devices in Crowdstrike Falcon. Supported entities: Hostname, URL, IP address and Hash. Note: Hostname entities are treated as domain IOCs and action will extract domain part out of URLs. Only MD5 and SHA-256 hashes are supported. IP address entities are treated as IOCs.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Devices Names|Specify a comma-separated list of devices for which you want to retrieve processes related to entities.|True|String||



##### JSON Results
```json
{"EntityResult": [{"device_id":"74089e3XXXXa4271ab14abXXXXXd18eb","command_line":"\\C:\\\\TMP\\\\mim.exe\\","process_id":"74089e3XXXXa4271ab14abXXXXXd18eb:400084000045","process_id_local":"400084000045","file_name":"\\\\Device\\\\HarddiskVolume2\\\\TMP\\\\mim.exe","start_timestamp":"2021-05-21T06:05:10Z","start_timestamp_raw":"132660507103371800","stop_timestamp":"2021-05-21T06:05:26Z","stop_timestamp_raw":"132660507260335807"},{"device_id":"74089e3XXXXa4271ab14abXXXXXd18eb","command_line":"C:\\\\TMP\\\\mim.exe\\","process_id":"74089e3XXXXa4271ab14abXXXXXd18eb:000029753080","process_id_local":"000029753080","file_name":"\\\\Device\\\\HarddiskVolume2\\\\TMP\\\\mim.exe","start_timestamp":"2021-05-21T06:07:15Z","start_timestamp_raw":"132660508352040249","stop_timestamp":"2021-05-21T06:07:21Z","stop_timestamp_raw":"132660508418773254"},{"device_id":"74089e3XXXXa4271ab14abXXXXXd18eb","command_line":"\\C:\\\\TMP\\\\mim.exe\\","process_id":"74089e3XXXXa4271ab14abXXXXXd18eb:000021388856","process_id_local":"000021388856","file_name":"\\\\Device\\\\HarddiskVolume2\\\\TMP\\\\mim.exe","start_timestamp":"2021-05-21T05:53:03Z","start_timestamp_raw":"132660499835265266","stop_timestamp":"2021-05-21T05:53:25Z","stop_timestamp_raw":"132660500056273239"},{"device_id":"74089e3XXXXa4271ab14abXXXXXd18eb","command_line":"\\C:\\\\TMP\\\\mim.exe\\","process_id":"74089e3XXXXa4271ab14abXXXXXd18eb:0000310768731","process_id_local":"000010768731","file_name":"\\\\Device\\\\HarddiskVolume2\\\\TMP\\\\mim.exe","start_timestamp":"2021-05-21T05:47:59Z","start_timestamp_raw":"132660496793281001","stop_timestamp":"2021-05-21T05:48:00Z","stop_timestamp_raw":"132660496807679553"}], "Entity": "f8f1c210a8c863efc0f6b8ac3553030a14a702ce8cf573cb5e9cd58f70c7c622"}
```



#### Get Event Offset
Action will retrieve the event offset that is used by the Event Streaming Connector. Note: action starts processing events from 30 days ago.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Events To Process|Specify how many events the action needs to process starting from the offset from 30 days ago.|True|String|10000|



##### JSON Results
```json
{"offset":100000,"timestamp":1627634506826}
```



#### Add Identity Protection Detection Comment
Add a comment to identity protection detection in Crowdstrike.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Detection ID|Specify the ID of the detection that needs to be updated.|True|String||
|Comment|Specify the comment for the detection.|True|String||



#### Close Detection
Close a Crowdstrike Falcon detection. Note: Action "Update Detection" is the best practice for this use case.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Detection ID|Specify the id of the detection that needs to be closed.|True|String||
|Hide Detection|If enabled, action will hide the detection in the UI.|False|Boolean|true|



#### Add Comment to Detection
Add a comment to the detection in Crowdstrike Falcon.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Detection ID|Specify the id of the detection to which you want to add a comment.|True|String||
|Comment|Specify the comment that needs to be added to the detection.|True|String||



#### Delete IOC
Delete custom IOCs in Crowdstrike Falcon. Supported entities: Hostname, URL, IP address and Hash. Note: Hostname entities are treated as domain IOCs and action will extract domain part out of URLs. Only MD5 and SHA-256 hashes are supported.
Timeout - 600 Seconds



#### Update Detection
Update detection in Crowdstrike Falcon.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Detection ID|Specify the ID of the detection that needs to be updated.|True|String||
|Status|Specify the new status for the detection.|True|List||
|Assign Detection to|Specify the email address of the Crowdstrike Falcon user, who needs to be assigned to this detection|False|String||



#### Submit File
Submit files to a sandbox in Crowdstrike. Note: This action requires a Falcon Sandbox license. For the list of supported file formats, refer to the documentation portal.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Paths|Specify the file paths to the files that need to be submitted. Refer to the documentation portal for a list of the supported file formats.|True|String||
|Sandbox Environment|Specify the sandbox environment for the analysis.|False|List|Windows 10, 64-bit|
|Network Environment|Specify the network environment for the analysis.|False|List|Default|
|Archive Password|Specify the password that would need to be used, when working with archive files.|False|Password||
|Document Password|Specify the password that would need to be used, when working with Adobe or Office files. Maximum: 32 characters.|False|Password||
|Check Duplicate|If enabled, the action checks if the file was already submitted previously and returns the available report. Note: during the validation “Network Environment” and “Sandbox Environment” are not taken into consideration.|False|Boolean|true|
|Comment|Specify the comment for the submission.|False|String||
|Confidential Submission|If enabled, the file is only shown to users within your customer account.|False|Boolean|false|



##### JSON Results
```json
[{"Entity": "/test1.pdf", "EntityResult": [{"id": "27fe4e476ca3490b8476b2b6650e5a74_8b43a4c9d5ea4306af4e827b6901cd60", "cid": "27fe4e476ca3490b8476b2b6650e5a74", "created_timestamp": "2023-04-28T14:00:00Z", "origin": "apigateway", "sandbox": [{"sha256": "8decc8571946d4cd70a024949e033a2a2a54377fe9f1c1b944c20f9ee11a9e51", "environment_id": 160, "environment_description": "Windows 10 64 bit", "submit_name": "test1.pdf", "submission_type": "file", "verdict": "no specific threat", "file_type": "PDF document, version 1.3", "sample_flags": ["Extracted Files"], "network_settings": "default"}], "verdict": "whitelisted", "ioc_report_strict_csv_artifact_id": "ded2c6801f51b43ba4b6de371188960239e84d227a16f065b6b96404854f27d4", "ioc_report_broad_csv_artifact_id": "ded2c6801f51b43ba4b6de371188960239e84d227a16f065b6b96404854f27d4", "ioc_report_strict_json_artifact_id": "9a659092e0dc2ea6b57254eed04af5012267fb2c8990b277492fe172dfa86bf2", "ioc_report_broad_json_artifact_id": "9a659092e0dc2ea6b57254eed04af5012267fb2c8990b277492fe172dfa86bf2", "ioc_report_strict_stix_artifact_id": "fa98bc61b6e62837dbff2a7c34e0e3cee3e90ff277bed059b634d806bcdad726", "ioc_report_broad_stix_artifact_id": "fa98bc61b6e62837dbff2a7c34e0e3cee3e90ff277bed059b634d806bcdad726", "ioc_report_strict_maec_artifact_id": "cf12de7c8249dd80dc9e9591d964b13aa18b9b4a292a4ec3c9f58e7b1ff1d50d", "ioc_report_broad_maec_artifact_id": "cf12de7c8249dd80dc9e9591d964b13aa18b9b4a292a4ec3c9f58e7b1ff1d50d"}]}]
```



#### Contain Endpoint
Contain endpoint in Crowdstrike Falcon. Supported entities: Hostname and IP address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Fail If Timeout|If enabled, action will be failed, if not all of the endpoints were contained.|False|Boolean|true|



##### JSON Results
```json
{"Entity":"XXX.XXX.XXX","EntityResult":{"device_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","cid":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","agent_load_flags":"1","agent_local_time":"2021-05-26T11:54:38.105Z","agent_version":"X.XXX.XXX.0","bios_manufacturer":"Phoenix Technologies LTD","bios_version":"6.00","build_number":"XXXX","config_id_base":"XXXX","config_id_build":"XXXX","config_id_platform":"3","cpu_signature":"XXXXX","external_ip":"XXX.XXX.XXX.XXX","mac_address":"XX-XX-XX-XX-XX-XX","hostname":"XXXXXXXXXXXX","first_seen":"2021-01-12T16:01:43Z","last_seen":"2021-05-26T12:46:53Z","local_ip":"XXX.XXX.X.XX","major_version":"10","minor_version":"0","os_version":"Windows 10","platform_id":"0","platform_name":"Windows","policies":[{"policy_type":"prevention","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"71932dc2","assigned_date":"2021-02-05T10:17:18.181166503Z","applied_date":"2021-02-05T10:17:29.147610493Z","rule_groups":[]}],"reduced_functionality_mode":"no","device_policies":{"prevention":{"policy_type":"prevention","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"71932dc2","assigned_date":"2021-02-05T10:17:18.181166503Z","applied_date":"2021-02-05T10:17:29.147610493Z","rule_groups":[]},"sensor_update":{"policy_type":"sensor-update","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"tagged|1;101","assigned_date":"2021-05-20T13:21:15.793890625Z","applied_date":"2021-05-20T13:23:10.339303233Z","uninstall_protection":"ENABLED"},"device_control":{"policy_type":"device-control","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"assigned_date":"2021-01-12T16:05:30.418267934Z","applied_date":"2021-01-12T16:07:29.124988572Z"},"global_config":{"policy_type":"globalconfig","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"f61a5761","assigned_date":"2021-05-26T08:56:57.749380428Z","applied_date":"2021-05-26T08:57:09.08333925Z"},"remote_response":{"policy_type":"remote-response","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"settings_hash":"XXXXXXX","assigned_date":"2021-01-12T16:05:30.418259588Z","applied_date":"2021-01-12T16:05:41.768614744Z"},"firewall":{"policy_type":"firewall","policy_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","applied":true,"assigned_date":"2021-01-12T16:05:30.41820681Z","applied_date":"2021-01-12T16:07:35.656641903Z","rule_set_id":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"}},"groups":[],"group_hash":"XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX","product_type":"1","product_type_desc":"Workstation","provision_status":"Provisioned","serial_number":"VMware-XX XX XX XX XX XX XX XX-XX XX XX XX XX XX XX XX","service_pack_major":"0","service_pack_minor":"0","pointer_size":"8","status":"contained","system_manufacturer":"VMware, Inc.","system_product_name":"VMware Virtual Platform","tags":[],"modified_timestamp":"2021-05-26T12:46:59Z","slow_changing_modified_timestamp":"2021-05-26T08:54:51Z","meta":{"version":"XXXXX"}}}
```



#### Update Identity Protection Detection
Update an identity protection detection in Crowdstrike. Note: this action requires an Identity Protection license.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Detection ID|Specify the ID of the detection that needs to be updated.|True|String||
|Status|Specify the status for the detection.|False|List|Select One|
|Assign To|Specify the name of the analyst to whom the detection needs to be assigned. If "Unassign" is provided, action will remove assignment from the detection. Note: API will accept any value that is provided, even if the underlying user doesn't exist.|False|String||



##### JSON Results
```json
{"added_privileges":["DomainAdminsRole"],"aggregate_id":"aggind:27fe4e476ca3490b8476b2xxxxx:xxxxxxxx-xxxx-xxxx-xxxx-4ED8DB047549","cid":"27fxxxxxxxxxxxxxxxxxxxxxa74","composite_id":"27fe4e4xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx-4ED8DB047549","confidence":20,"context_timestamp":"2022-11-15T12:58:15.629Z","crawl_edge_ids":{"Sensor":["N6KIxxxxxxxxxCA4lr/"]},"crawl_vertex_ids":{"Sensor":["ind:27fe4e47xxxxxxxxxxxxxxxxxxxxxxxxxxxx4ED8DB047549"]},"crawled_timestamp":"2022-11-15T13:58:17.251061883Z","created_timestamp":"2022-11-15T12:59:17.239585706Z","description":"A user received new privileges","display_name":"Privilege escalation (user)","end_time":"2022-11-15T12:58:15.629Z","falcon_host_link":"https://falcon.crowdstrike.com/identity-protection/detections/nd:27fe4e476caxxxxxxxxxxxxxxxxxxxxxxxxxxxxED8DB047549","id":"ind:27fe4e476caxxxxxxxxxxxxxxxxxxxxxxxxxxxxED8DB047549","name":"IdpEntityPrivilegeEscalationUser","objective":"Gain Access","pattern_id":51113,"previous_privileges":"0","privileges":"8321","product":"idp","scenario":"privilege_escalation","severity":2,"show_in_ui":true,"source_account_domain":"test","source_account_name":"Mailbox438","source_account_object_sid":"S-1-5-21-3479765008-4256118348-3151044947-3595","start_time":"2022-11-15T12:58:15.629Z","status":"new","tactic":"Privilege Escalation","tactic_id":"TA0xxx","tags":["red_team"],"technique":"Valid Accounts","technique_id":"Txxx8","timestamp":"2022-11-15T12:58:17.239Z","type":"idp-user-endpoint-app-info","updated_timestamp":"2023-03-03T10:24:48.744735285Z"}
```



#### Submit URL
Submit urls to a sandbox in Crowdstrike. Note: This action requires a Falcon Sandbox license.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|URLs|Specify the URLs that need to be submitted.|True|String||
|Sandbox Environment|Specify the sandbox environment for the analysis.|False|List|Windows 10, 64-bit|
|Network Environment|Specify the network environment for the analysis.|False|List|Default|
|Check Duplicate|If enabled, the action checks if the file was already submitted previously and returns an available report. Note: during the validation “Network Environment” and “Sandbox Environment” are not taken into consideration.|False|Boolean|true|



##### JSON Results
```json
[{"Entity": "https://www.google.com", "EntityResult": [{"id": "27fe4e476ca3490b8476b2b6650e5a74_aa14936582d941fda1441fcc47a65d86", "cid": "27fe4e476ca3490b8476b2b6650e5a74", "created_timestamp": "2023-04-28T12:01:51Z", "origin": "apigateway", "sandbox": [{"sha256": "15fea7cc23194aea10dce58cff8fff050c81e1be0d16e4da542f4fedd5a421c3", "environment_id": 160, "environment_description": "Windows 10 64 bit", "submit_url": "hxxps://www.google.com", "submission_type": "page_url", "verdict": "no specific threat", "incidents": [{"name": "Network Behavior", "details": ["Contacts 3 domains and 3 hosts"]}], "sample_flags": ["Network Traffic", "Extracted Files"], "network_settings": "default"}], "verdict": "no specific threat", "ioc_report_strict_csv_artifact_id": "6fb809c85f671f754f9af8ef345e1db2c432ed8a4638197a187f5b23c6c0388e", "ioc_report_broad_csv_artifact_id": "4149f8276272bc8f0cbf485aff5969d24dcdca62b28bf90432186e2db7e82e24", "ioc_report_strict_json_artifact_id": "d3b00b1fb18996afe15960c30ce226052f7d6901bd43a180764bfd020ca119da", "ioc_report_broad_json_artifact_id": "6d3bef8ddf0513bf009ffa36d0fb169627c73eddca9404dbe9ea75fb6ad454e5", "ioc_report_strict_stix_artifact_id": "5b05d9fe2b7d0baa7cc005fca234c8eebd3b8ae899776ec7be882cedfcbbb0b3", "ioc_report_broad_stix_artifact_id": "45b4cdd9a4316a91f764c09b14f9cbde04ffc87e0730e2df86c8d4c57a0a77ec", "ioc_report_strict_maec_artifact_id": "3f5a7636feaf55492ae2cb8315d821fc1a89a5ebc108056a1905fb66019f35a2", "ioc_report_broad_maec_artifact_id": "7e8db3819b3a4a0bbb62b545cf14b18d090934eeed160d04007bbcb00f3290cc"}]}]
```



#### Add Incident Comment
Add comment to incident in Crowdstrike.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Incident ID|Specify the ID of the incident that needs to be updated.|True|String||
|Comment|Specify the comment for the incident.|True|String||



##### JSON Results
```json
[{"incident_id": "inc:466a00b13a5e4a9a9x.ac1a5e:x.x.x.", "incident_type": 1, "cid": "27fe4e476ca3490b6b2b6650e5a74", "host_ids": ["466a00b13a5e4a9a93ce2aca5eac1a5e"], "hosts": [{"device_id": "466a00b13a5e4a9a93ce2aca5eac1a5e", "cid": "27fe4e476ca34dd90b8476b2b6650e5a74", "agent_load_flags": "0", "agent_local_time": "2023-09-25T15:41:40.130Z", "agent_version": "7.01.17312.0", "bios_manufacturer": "VMware, Inc.", "bios_version": "VMW71.00V.17369862.B64.2012240522", "config_id_base": "65994753", "config_id_build": "17312", "config_id_platform": "3", "external_ip": "35.246.203.0", "hostname": "EX16-AD01", "first_seen": "2023-01-20T00:40:31Z", "last_seen": "2023-10-06T07:19:50Z", "local_ip": "172.30.3.162", "mac_address": "00-50-56-a2-94-8d", "machine_domain": "exlab.local", "major_version": "10", "minor_version": "0", "os_version": "Windows Server 2016", "ou": ["Domain Controllers"], "platform_id": "0", "platform_name": "Windows", "product_type": "2", "product_type_desc": "Domain Controller", "site_name": "Default-First-Site-Name", "status": "contained", "system_manufacturer": "VMware, Inc.", "system_product_name": "VMware7,1", "groups": ["9489d65c343244169627dcbc"], "modified_timestamp": "2023-10-06T07:19:58Z"}], "created": "2023-10-06T07:20:51Z", "start": "2023-10-06T07:19:21Z", "end": "2023-10-06T07:30:27Z", "state": "closed", "assigned_to": "67494-b86d-4a55-9e52-7492449400a1", "assigned_to_name": "Yuriy Landovskyy", "status": 30, "tactics": ["Persistence", "Defense Evasion", "Command and Control", "Credential Access", "Malware", "Privilege Escalation"], "techniques": ["Create Account", "Masquerading", "Ingress Tool Transfer", "OS Credential Dumping", "Malicious File", "Image File Execution Options Injection", "Bypass User Account Control", "Accessibility Features", "Registry Run Keys / Startup Folder"], "objectives": ["Keep Access", "Contact Controlled Systems", "Gain Access", "Falcon Detection Method"], "modified_timestamp": "2023-10-20T08:34:07.078440797Z", "users": ["EX16-AD01$", "administrator"], "fine_score": 100}]
```






## Jobs



## Connectors
#### Crowdstrike - Identity Protection Detections Connector
Pull Identity Protection detections from Crowdstrike. Note: this connector requires an Identity Protection license. Dynamic List works with the “display_name” parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|DeviceProductField|Enter the source field name in order to retrieve the Product Field name.|True|String|Product Name|
|EventClassId|Enter the source field name in order to retrieve the Event Field name.|True|String|type|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field through regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|PythonProcessTimeout|Timeout limit for the python process running the current script.|True|Integer|180|
|API Root|API root of the Crowdstrike instance.|True|String|https://api.crowdstrike.com|
|Client ID|Client ID  of the Crowdstrike account.|True|String||
|Client Secret|Client Secret of the Crowdstrike account.|True|Password||
|Lowest Severity Score To Fetch|Lowest severity score of the identity protection detections to fetch. If nothing is provided, the connector will ingest detections with all severities. Maximum is 100. Note: action also supports the following values: Informational, Low, Medium, High, Critical.|False|String||
|Max Hours Backwards|Amount of hours from where to fetch identity protection detections.|False|Integer|1|
|Max Detections To Fetch|How many identity protection detections to process per one connector iteration. Default: 10.|False|Integer|10|
|Use dynamic list as a blocklist|If enabled, the dynamic list will be used as a blocklist.|False|Boolean|true|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Crowdstrike server is valid.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password||


#### Crowdstrike - Incidents Connector
Pull incident and related behaviors from Crowdstrike. Dynamic List works with the “incident_type” parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|DeviceProductField|Enter the source field name in order to retrieve the Product Field name.|True|String|Product Name|
|EventClassId|Enter the source field name in order to retrieve the Event Field name.|True|String|data_type|
|API Root|API root of the Crowdstrike instance.|True|String|https://api.crowdstrike.com|
|Client ID|Client ID  of the Crowdstrike account.|True|String||
|Client Secret|Client Secret of the Crowdstrike account.|True|Password||
|Max Hours Backwards|Amount of hours from where to fetch incidents. Default: 1|False|String|1|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|PythonProcessTimeout|Timeout limit for the python process running the current script. Default: 180|True|Integer|180|
|Lowest Severity Score To Fetch|Lowest severity score of the incidents to fetch. If nothing is provided, the connector will ingest incidents with all severities. Maximum is 100. Note: action also supports the following values: Low, Medium, High, Critical. In the Crowdstrike UI the same value is presented as divided by 10.|False|String||
|Max Incidents To Fetch|How many incidents to process per one connector iteration. Default: 10. Max: 100.|False|String|10|
|Use dynamic list as a blocklist|If enabled, the dynamic list will be used as a blocklist.|False|Boolean|false|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Crowdstrike server is valid.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password||


#### Crowdstrike - Detections Connector
Pull detections from Crowdstrike. Whitelist works with filters that are supported by the API of Crowdstrike. For the details, please refer to the documentation portal.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|DeviceProductField|Enter the source field name in order to retrieve the Product Field name.|True|String|Product Name|
|EventClassId|Enter the source field name in order to retrieve the Event Field name.|True|String|behaviors_technique|
|PythonProcessTimeout|Timeout limit for the python process running the current script.|True|Integer|180|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API root of the Crowdstrike instance.|True|String|https://api.crowdstrike.com|
|Client ID|Client ID  of the Crowdstrike account.|True|String||
|Client Secret|Client Secret of the Crowdstrike account.|True|Password||
|Lowest Severity Score To Fetch|Lowest severity score of the detections to fetch. If nothing is provided, the connector won't apply this filter. Maximum is 100. Note: action also supports the following values: Low, Medium, High, Critical.|False|String|50|
|Lowest Confidence Score To Fetch|Lowest confidence score of the detections to fetch. If nothing is provided, the connector won't apply this filter. Maximum is 100.|False|Integer|0|
|Max Hours Backwards|Amount of hours from where to fetch detections.|False|Integer|1|
|Max Detections To Fetch|How many detections to process per one connector iteration. Default: 10.|False|Integer|10|
|Padding Period|The number of hours that connector will use for padding. Maximum: 6.|False|Integer|1|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Crowdstrike server is valid.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password||


#### Crowdstrike Falcon Streaming Events Connector
Crowdstrike Falcon Streaming Events Connector

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|DeviceProductField|Describes the name of the field where the product name is stored.|True|String|device_product|
|EventClassId|Describes the name of the field where the event name is stored.|True|String|Name|
|PythonProcessTimeout|The timeout limit (in seconds) for the python process running current script|True|Integer|60|
|Environment Field Name|Describes the name of the field where the environment name is stored. If environment field isn't found, environment is ""|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field.|False|String||
|API Root|API root of the Crowdstrike instance|False|String|https://api.crowdstrike.com|
|Client ID|Client ID for Crowdstrike API|True|String||
|Client Secret|Client Secret for Crowdstrike API|True|Password||
|Event types|Specify a comma-separated list of event types. Examples of the event types: DetectionSummaryEvent, IncidentSummaryEvent, AuthActivityAuditEvent, UserActivityAuditEvent, RemoteResponseSessionStartEvent, RemoteResponseSessionEndEvent. For more information visit documentation portal.|False|String|DetectionSummaryEvent, IncidentSummaryEvent, AuthActivityAuditEvent, UserActivityAuditEvent, RemoteResponseSessionStartEvent, RemoteResponseSessionEndEvent|
|Max Events per Cycle|Max events to process per connector run.|True|Integer|100|
|Max Day Backwards|Max amount of days to fetch events data backwards|False|Integer|3|
|Min Severity|Specify the events that should be ingested based on the events severity (detections events). The value ranges from 0-5. If other event types besides detections are ingested by the connector, connector sets a severity for them as -1 and this filter is not applied to those types of events|False|Integer|0|
|Alert Name Template|If provided, connector will use this value for Siemplify Alert Name. Please refer to the documentation portal for more details. You can provide placeholders in the following format: [name of the field]. Example: Phishing - [event_mailbox]. Note: connector will use first Siemplify Event for placeholders. Only keys that have string value will be handled. If nothing is provided or user provides an invalid template, connector will use the default alert name.|False|String||
|Rule Generator Template|	If provided, the connector will use this value for Siemplify Rule Generator. Please refer to the documentation portal for more details. You can provide placeholders in the following format: [name of the field]. Example: Phishing - [event_mailbox]. Note: connector will use the first Siemplify event for placeholders. Only keys that have string value will be handled. If nothing is provided or the user provides an invalid template, the connector will use the default rule generator.|False|String||
|Proxy Server Address|Proxy server address.|False|String||
|Proxy Username|Proxy username.|False|String||
|Proxy Password|Proxy password.|False|Password||
|Verify SSL|Indicate whether to use SSL in the session or not|False|Boolean|false|




