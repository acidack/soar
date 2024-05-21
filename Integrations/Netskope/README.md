<p align="center"><img src="./Resources/Netskope.svg" 
     alt="Netskope" width="200"/></p>

# Netskope

The Netskope Security Cloud helps the world’s largest organizations take full advantage of the cloud and web without sacrificing security.

Python Version - 2
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root|None|True|String|https://{IP}|
|Api Key|None|True|Password|None|
|Verify SSL|None|False|Boolean|False|


#### Dependencies
| |
|-|
|cross/certifi-2019.11.28-py2.py3-none-any.whl|
|cross/chardet-3.0.4-py2.py3-none-any.whl|
|cross/urllib3-1.25.7-py2.py3-none-any.whl|
|cross/TIPCommon-1.0.10-py3-none-any.whl|
|cross/requests-2.22.0-py2.py3-none-any.whl|
|cross/idna-2.8-py2.py3-none-any.whl|


## Actions
#### Download File
Download a quarantined file.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File ID|ID of a file, needed to identify a file.|True|String||
|Quarantine Profile ID|ID of a quarantine profile.|True|String||



#### Ping
Test connectivity to Netskope.
Timeout - 600 Seconds



#### List Events
List events.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|This acts as a filter for all the cloud app events in the events database.|False|String||
|Type|The type of the alert to filter by. Valid values: page | application | audit | infrastructure.|False|String||
|Time Period|Time period to search events at (milliseconds backwards). Valid Values: 3600 | 86400 | 604800 | 2592000.|False|String||
|Start Time|Restrict events to those that have timestamps greater than this (unixtime). Needed only if time period is not passed.|False|String||
|End Time|Restrict events to those that have timestamps less than this (unixtime). Needed only if time period is not passed.|False|String||
|Limit|Number of results to return. Default: 100.|False|String||



##### JSON Results
```json
[{"dstip": "0.0.0.0", "browser_session_id": 1066949788113471080, "srcip": "0.0.0.0", "app_session_id": 4502249472406092569, "os_version": "WindowsServer2016", "dst_region": "Virginia", "numbytes": 37480, "req_cnt": 18, "server_bytes": 8994, "page_id": 0, "page_duration": 867, "page_endtime": 1548577530, "dst_latitude": 39.0481, "timestamp": 1548576663, "src_region": "Oregon", "src_location": "Boardman", "ur_normalized": "person@company.com", "appcategory": "", "src_latitude": 45.8491, "count": 1, "bypass_traffic": "no", "type": "page", "userip": "0.0.0.0", "src_longitude": -119.7143, "page": "WebBackground", "browser": "", "domain": "WebBackground", "dst_location": "Ashburn", "_insertion_epoch_timestamp": 1548577621, "site": "WebBackground", "access_method": "Client", "browser_version": "", "category": "", "client_bytes": 28486, "user_generated": "no", "hostname": "IP-C0A84AC", "dst_country": "US", "resp_cnt": 18, "src_zipcode": "97818", "traffic_type": "Web", "http_transaction_count": 18, "organization_unit": "casb.us/Users", "page_starttime": 1548576663, "dst_longitude": -77.4728, "user": "person@email.com", "userkey": "person@email.com", "device": "WindowsDevice", "src_country": "US", "dst_zipcode": "20149", "url": "WebBackground", "sv": "", "ccl": "unknown", "useragent": "RestSharp/105.2.3.0", "_id": "00000000", "os": "WindowsServer2016"}]
```



#### List Quarantined Files
List quarantined files.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Start Time|Restrict events to those that have timestamps greater than this (unixtime). Needed only if time period is not passed.|False|String||
|End Time|Restrict events to those that have timestamps less than this (unixtime). Needed only if time period is not passed.|False|String||



##### JSON Results
```json
{}
```



#### List Clients
List clients.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|This acts as a filter on all the entries in the database.|False|String||
|Limit|Number of results to return. Default: 25.|False|String||



##### JSON Results
```json
[{"client_install_time": 1532040251, "users": [{"heartbeat_status_since": 1532040385, "user_added_time": 1532040167, "last_event": {"status": "Enabled", "timestamp": 1548578307, "event": "Tunnel Up", "actor": "System"}, "device_classification_status": "Not Configured", "username": "john_doe@example.com", "user_source": "Manual", "userkey": "00000", "_id": "00000", "heartbeat_status": "Active"}], "last_event": {"status": "Enabled", "timestamp": 1548578307, "event": "Tunnel Up", "actor": "System"}, "host_info": {"device_model": "VMware Virtual Platform", "os": "Windows", "hostname": "host000", "device_make": "VMware, Inc.", "os_version": "10.0"}, "client_version": "1.1.1.1", "_id": "device000", "device_id": "device000"}]
```



#### Block File
Block a quarantined file.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File ID|ID of a file, needed to identify a file.|True|String||
|Quarantine Profile ID|ID of a quarantine profile.|True|String||



#### Allow File
Allow a quarantined file.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File ID|ID of a file, needed to identify a file.|True|String||
|Quarantine Profile ID|ID of a quarantine profile.|True|String||



#### List Alerts
List alerts.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|This acts as a filter for all the cloud app events in the alerts database.|False|String||
|Type|The type of the alert to filter by. Valid values: anomaly | 'Compromised Credential' | policy | 'Legal Hold' | malsite | Malware | DLP | watchlist | quarantine | Remediation.|False|String||
|Time Period|Time period to search alerts at (milliseconds backwards). Valid Values: 3600 | 86400 | 604800 | 2592000.|False|String||
|Start Time|Restrict alerts to those that have timestamps greater than this (unixtime). Needed only if time period is not passed.|False|String||
|End Time|Restrict alerts to those that have timestamps less than this (unixtime). Needed only if time period is not passed.|False|String||
|Is Acknowledged|Whether to get only acknowledged alerts.|False|Boolean||
|Limit|Number of results to return. Default: 100.|False|String||



##### JSON Results
```json
[[{"src_region": "Quebec", "dstip": "13.107.6.000", "dst_location": "Des Moines", "app": "LastPass", "_insertion_epoch_timestamp": 1595484010, "site": "LastPass", "device": "Win Device", "browser_version": "54.0.2840.90", "file_size": 10174706, "object_type": "File", "app_session_id": 7870854727506923561, "browser_session_id": 5221268058711925774, "page_site": "lastpass.com", "dst_country": "US", "category": "Identity and Access Management", "dst_region": "Iowa", "hostname": "EC2AMAZ-1OAJxxx", "severity": "unknown", "object_id": "1996cb6d-4436-4153-9202-a6b7ddfacxxx", "managed_app": "yes", "os_version": "Win", "parent_id": "/personal/perftester2_perfskope_com/Documents", "src_zipcode": "H3G", "src_timezone": "America/Toronto", "src_location": "Montreal", "traffic_type": "CloudApp", "slc_longitude": -73.5792999268, "type": "anomaly", "transaction_id": 1131115872485042512, "slc_latitude": 45.4986991882, "object": "10MB.jpg_20170904-000456_demo.jpg", "timestamp": 1595484010, "organization_unit": "", "telemetry_app": "", "alert": "yes", "referer": "https:// ", "user": "Abe@mail.com", "userkey": "v@test.com", "srcip": "35.182.91.154", "dst_timezone": "America/Los_Angeles", "src_country": "CA", "md5": "60d2e411eb2f43968bd63f3ea0949xxx", "count": 1, "access_method": "Client", "dst_zipcode": "9000", "url": " GetFolderByServerRelativeUrl(@a1)/Files/Add(url=@a2,overwrite=@a3)", "instance_id": "perfskope", "ccl": "excellent", "activity": "Upload", "userip": "172.31.11.000", "os": "Win", "page": " ", "browser": "Chrome", "nsdeviceuid": "", "managementID": "", "src_geoip_src": 2, "dst_geoip_src": 1, "ur_normalized": "abe@mail.com", "profile_id": "NS_306", "download_app": "Cisco WebEx", "bin_timestamp": 1595491200, "threshold_time": 7200, "event_type": "data_exfiltration", "alert_name": "data_exfiltration", "risk_level": "high", "risk_level_id": 2, "alert_type": "anomaly", "acked": "false", "orig_ty": "nspolicy", "_id": "d14ab47c90b2a257b6ab2322", "other_categories": ["Cloud Storage"], "cci": 81, "page_id": 7638768646583785531, "appcategory": "Identity and Access Management"}]]
```






## Jobs



## Connectors


