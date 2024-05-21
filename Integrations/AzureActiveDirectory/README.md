
# AzureActiveDirectory

Azure Active Directory (Azure AD) is Microsoft’s cloud-based identity and access management service, which helps your employees sign in and access  both internal and external resources.

Python Version - 2
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Client ID|None|True|String||
|Client Secret|None|True|Password|None|
|Directory ID|None|True|String||
|Verify SSL|None|False|Boolean|True|


#### Dependencies
| |
|-|
|cross/certifi-2021.5.30-py2.py3-none-any.whl|
|cross/urllib3-1.26.6-py2.py3-none-any.whl|
|cross/TIPCommon-1.0.10-py3-none-any.whl|
|cross/requests-2.25.1-py2.py3-none-any.whl|
|cross/chardet-4.0.0-py2.py3-none-any.whl|
|cross/idna-2.8-py2.py3-none-any.whl|


## Actions
#### Is User In a Group
Check if user has membership in a specific Azure AD group. Action expects Siemplify user entity in username@domain format and group id in 00e40000-1971-439d-80fc-d0e000001dbd format.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Group ID|Azure AD group id in 00e40000-1971-439d-80fc-d0e000001dbd format.|True|String||



##### JSON Results
```json
[{"EntityResult": "true","Entity": "user@mail.com"}]
```



#### List Groups
List Azure Active Directory groups based on the specified search criteria. Note that action is not working on Siemplify entities. Additionally, filtering is working on the Name field.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Order By|Specifies the result order. Groups are sorted by their display name.|False|List|ASC|
|Results Limit|Specify max number of groups to return.|False|String||
|Filter Logic|Specify what filter logic should be applied. Filtering is working on the Name field.|False|List|Equal|
|Filter Value|Specify what value should be used in the filter. If “Equal“ is selected, action will try to find the exact match among results and if “Contains“ is selected, action will try to find results that contain that substring. If nothing is provided in this parameter, the filter will not be applied. Filtering is working on the Name field.|False|String||



##### JSON Results
```json
[{"Group_Type": "managed", "Id": "1212-12312-123","Name": "Group Name","Description": "This group is ...", "Created_Time":"2019-10-24T19:10:18Z"}]
```



#### Force Password Update
Force password update for user so the user will have to change their password on next login. Action expects Siemplify user entity in username@domain format.
Timeout - 600 Seconds



#### List Members in the Group
List members in the specified Azure AD group.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Records To Return|Specify how many records to return. If nothing is provided, action will return 50 records.|False|String|50|
|Group Name|Specify group name to return user list for.|False|String||
|Group ID|Specify the ID of the group in which you want to list the members. If both "Group Name" and "Group ID" are provided, then "Group ID" will have priority. Example of the id: 00e40000-1971-439d-80fc-d0e000001dbd.|False|String||
|Filter Key|Specify the key that needs to be used to filter group members.|False|List|Select One|
|Filter Logic|Specify what filter logic should be applied. Filtering logic is working based on the value  provided in the "Filter Key" parameter.|False|List|Not Specified|
|Filter Value|Specify what value should be used in the filter. If “Equal“ is selected, action will try to find the exact match among results and if "Contains" is selected, action will try to find results that contain that substring. If nothing is provided in this parameter, the filter will not be applied. Filtering logic is working based on the value  provided in the "Filter Key" parameter.|False|String||



##### JSON Results
```json
[{"@odata.type": "#microsoft.graph.group", "id": "367d61e8-ca2a-4370-9cc9-xxx", "deletedDateTime": null, "classification": null, "createdDateTime": "2020-01-10T11:49:07Z", "creationOptions": [], "description": "This group is used during Exchange setup and is not intended to be used for other purposes.", "displayName": "Exchange Install Domain Servers", "expirationDateTime": null, "groupTypes": [], "isAssignableToRole": null, "mail": null, "mailEnabled": false, "mailNickname": "Exchange_Install_Domain_Servers", "membershipRule": null, "membershipRuleProcessingState": null, "onPremisesDomainName": "xxxxx.local", "onPremisesLastSyncDateTime": "2020-01-10T11:49:07Z", "onPremisesNetBiosName": "xxxx", "onPremisesSamAccountName": "$O31000-5FK60FIR1GGC", "onPremisesSecurityIdentifier": "S-1-5-21-1263192401-1628743863-235899853-1144", "onPremisesSyncEnabled": true, "preferredDataLocation": null, "preferredLanguage": null, "proxyAddresses": [], "renewedDateTime": "2020-01-10T11:49:07Z", "resourceBehaviorOptions": [], "resourceProvisioningOptions": [], "securityEnabled": true, "securityIdentifier": "S-1-12-1-914186728-1131465258-3608725916-xxxx", "theme": null, "visibility": null, "onPremisesProvisioningErrors": []}]
```



#### Add User To a Group
Add user to a specific Azure AD group. Action expects Siemplify user entity in username@domain format and group id in 00e40000-1971-439d-80fc-d0e000001dbd format.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Group ID|Azure AD group id in 00e40000-1971-439d-80fc-d0e000001dbd format.|True|String||



#### Ping
Test connectivity to the Azure Active Directory service with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Enrich User
Enrich Siemplify User entity with information from Azure Active Directory. Action expects Siemplify user entity in username@domain format.
Timeout - 600 Seconds



##### JSON Results
```json
[{"Entity":"user@domain.onmicrosoft.com","EntityResult":{"@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users/$entity","@odata.id":"https://graph.microsoft.com/v2/d48f52ca-5b1a-4708-8ed0-xxxxx/directoryObjects/2d14c76d-49ea-429b-ba91-xxxxx/Microsoft.DirectoryServices.User","businessPhones":[],"displayName":"User Name","givenName":"User","jobTitle":null,"mail":null,"mobilePhone":null,"officeLocation":null,"preferredLanguage":null,"surname":"Aleksanyan","userPrincipalName":"user@domain.onmicrosoft.com","id":"2d14c76d-49ea-429b-ba91-xxxxx"}}]
```



#### List Users
List Azure Active Directory users based on the specified search criteria. Note that action is not working on Siemplify entities. Additionally, advanced filtering is working on the Username (userPrincipalName) field.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter|Specifies which fields will be included in the results. By default, we will return all the fields.|False|List|All Fields|
|Order By Field|Specifies the field based on which the results are ordered.|False|List|displayName|
|Order By|Specifies the result order.|False|List|DESC|
|Results Limit|Specify max number of users to return.|False|String||
|Advanced Filter Logic|Specify what filter logic should be applied. Advanced filtering is working on the Username (userPrincipalName) field.|False|List|Equal|
|Advanced Filter Value|Specify what value should be used in the filter. If “Equal“ is selected, action will try to find the exact match among results and if “Contains“ is selected, action will try to find results that contain that substring. If nothing is provided in this parameter, the filter will not be applied.  Advanced filtering is working on the Username (userPrincipalName) field.|False|String||



##### JSON Results
```json
[{"Username": "someusername@mail.com", "Surname": "TestSurname", "Name": "TestName", "Job_Title": "Engineer", "Mobile_Phone": "123456789", "Preferred_Language": "English", "Mail": "someusername@mail.com", "Givenname": "TestGivenName", "Id": "12345678-1234-1234-1234-1234567890"}]
```



#### Reset User Password
Change user password to the password specified in the action. User will have to change their password on next login. Action expects Siemplify user entity in username@domain format.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Password|User Authentication password.|True|Password||



#### Enrich Host
Enrich Siemplify Host entity with information from Azure Active Directory. Action finds a match for a provided Host entity based on the devices displayName field in Azure AD
Timeout - 600 Seconds



##### JSON Results
```json
[{"Entity":"SENINELONE-xxxxx","EntityResult":{"@odata.id":"https://graph.microsoft.com/v2/d48f52ca-5b1a-4708-8ed0-xxxxx/directoryObjects/433e2228-0aea-448c-9b78-xxxxx/Microsoft.DirectoryServices.Device","id":"433e2228-0aea-448c-9b78-xxxxxx","if":"433e2228-0aea-448c-9b78-xxxxxx","deletedDateTime":null,"accountEnabled":true,"approximateLastSignInDateTime":"2021-08-05T06:24:30Z","complianceExpirationDateTime":null,"createdDateTime":"2021-02-08T12:14:31Z","deviceCategory":null,"deviceId":"356c1602-7255-4191-8590-xxxxx","deviceMetadata":null,"deviceOwnership":"Personal","deviceVersion":2,"displayName":"SENINELONE-H01","domainName":null,"enrollmentProfileName":null,"enrollmentType":"AutoEnrollment","externalSourceName":null,"isCompliant":true,"isManaged":true,"isRooted":false,"managementType":"MDM","manufacturer":"VMware, Inc.","mdmAppId":"0000000a-0000-0000-xxxx-xxxx","model":"VMware Virtual Platform","onPremisesLastSyncDateTime":null,"onPremisesSyncEnabled":null,"operatingSystem":"Windows","operatingSystemVersion":"10.0.18363.1679","physicalIds":["[USER-GID]:b786d3cf-e97d-4511-b61c-xxxxx:6825788988304991","[GID]:g:6825788988xxxx","[USER-HWID]:b786d3cf-e97d-4511-b61c-xxxxx:6825788988304990","[HWID]:h:6825788988xxxx"],"profileType":"RegisteredDevice","registrationDateTime":"2021-02-08T12:14:31Z","sourceType":null,"systemLabels":[],"trustType":"Workplace","extensionAttributes":{"extensionAttribute1":null,"extensionAttribute2":null},"alternativeSecurityIds":[{"type":2,"identityProvider":null,"key":"WAA1ADAAOQA6ADwAUwBIAEEAMQAtAFQAUAAtAFAAVQBCAEsARQBZAD4AMQA4AEYARAAwADUAMwBDAEUAMgBGADEAOABBAEQARQA2ADQAQgA0AEUAQQA1ADMARgA5ADIARABGADgAOQA1AEIARAA2AEYARAAzADcxxxxxxxx"}]}}]
```



#### Get Manager Contact Details
Get manager contact details for user. Action expects Siemplify user entity in username@domain format.
Timeout - 600 Seconds



##### JSON Results
```json
[{"EntityResult": {"displayName": "manager@mail.com", "mobilePhone": "1212-12312-123","@odata.context": "graph.microsoft.com"}, "Entity": "user@mail.com"}]
```



#### List User's Groups Membership
List Azure AD groups user is a member of. Note: The user name can be provided either as a Siemplify entity or as an action input parameter. If the user name is passed to action both as an entity and input parameter - action will be executed on the input parameter. User name should be specified in username@domain format.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User Name|Specify user name to return groups membership for. User name should be specified in username@domain format. Parameter accepts multiple values as a comma separated string.|False|String||
|Return Only Security Enabled Groups|If enabled, only security groups that the user is a member of will be returned.|False|Boolean|false|
|Return Detailed Groups Information|If enabled, detailed information on the AD groups will be returned.|False|Boolean|false|
|Filter Key|Specify the key that needs to be used to filter groups.|False|List|Select One|
|Filter Logic|Specify what filter logic should be applied. Filtering logic is working based on the value  provided in the "Filter Key" parameter.|False|List|Not Specified|
|Filter Value|Specify what value should be used in the filter. If "Equal" is selected, action will try to find the exact match among results and if "Contains" is selected, action will try to find results that contain that substring. If nothing is provided in this parameter, the filter will not be applied. Filtering logic is working based on the value  provided in the "Filter Key" parameter.|False|String||
|Max Records To Return|Specify how many records to return. If nothing is provided, action will return 50 records.|False|String|50|



##### JSON Results
```json
[{"Entity": "test@example.com", "EntityResult": [{"id": "00b135d0-603d-4b1e-93e4-24xxxxxxxxxx", "deletedDateTime": null, "classification": null, "createdDateTime": "2021-11-28T20:28:56Z", "creationOptions": ["ProvisionGroupHomepage", "HubSiteId:00000000-0000-0000-0000-000000000000", "SPSiteLanguage:1033"], "description": "SiemplifyIntegration2", "displayName": "SiemplifyIntegration2", "expirationDateTime": null, "groupTypes": ["Unified"], "isAssignableToRole": null, "mail": "test@example.com", "mailEnabled": true, "mailNickname": "SiemplifyIntegration2", "membershipRule": null, "membershipRuleProcessingState": null, "onPremisesDomainName": null, "onPremisesLastSyncDateTime": null, "onPremisesNetBiosName": null, "onPremisesSamAccountName": null, "onPremisesSecurityIdentifier": null, "onPremisesSyncEnabled": null, "preferredDataLocation": null, "preferredLanguage": null, "proxyAddresses": ["SPO:SPO_80b058c6-6886-47d4-adcc-8cffa88aca4c@SPO_d48f52ca-5b1a-4708-8ed0-ebxxxxxxxxxx", "SMTP:test@example.com"], "renewedDateTime": "2021-11-28T20:28:56Z", "resourceBehaviorOptions": [], "resourceProvisioningOptions": [], "securityEnabled": false, "securityIdentifier": "S-1-12-1-11613648-1260281917-3844400275-xxxxxxxxxx", "theme": null, "visibility": "Private", "onPremisesProvisioningErrors": []}, {"id": "59a278af-e84f-48ed-acab-84xxxxxxxxxx", "deletedDateTime": null, "classification": null, "createdDateTime": "2021-11-10T13:36:47Z", "creationOptions": [], "description": "k8s", "displayName": "k8s", "expirationDateTime": null, "groupTypes": [], "isAssignableToRole": true, "mail": null, "mailEnabled": false, "mailNickname": "4eccf442-d", "membershipRule": null, "membershipRuleProcessingState": null, "onPremisesDomainName": null, "onPremisesLastSyncDateTime": null, "onPremisesNetBiosName": null, "onPremisesSamAccountName": null, "onPremisesSecurityIdentifier": null, "onPremisesSyncEnabled": null, "preferredDataLocation": null, "preferredLanguage": null, "proxyAddresses": [], "renewedDateTime": "2021-11-10T13:36:47Z", "resourceBehaviorOptions": [], "resourceProvisioningOptions": [], "securityEnabled": true, "securityIdentifier": "S-1-12-1-1503819951-1223551055-3062148012-xxxxxxxxx", "theme": null, "visibility": "Private", "onPremisesProvisioningErrors": []}]}]
```



#### Remove User from a Group
Remove User from the specified group. Note: The user name can be provided either as a Siemplify entity or as an action input parameter. If the user name is passed to action both as an entity and input parameter - action will be executed on the input parameter. User name should be specified in username@domain format.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User Name|Specify user name to remove from the target group. User name should be specified in username@domain format. Parameter accepts multiple values as a comma separated string.|False|String||
|Group Name|Specify group name to remove user from.|False|String||
|Group ID|Specify the ID of the group from which you want to remove the user. If both "Group Name" and "Group ID" are provided, then "Group ID" will have priority. Example of the id: 00e40000-1971-439d-80fc-d0e000001dbd.|False|String||



#### Disable Account
Disable account in Azure Active Directory. Action expects Siemplify user entity in username@domain format.
Timeout - 600 Seconds



#### Revoke User Session
Revoke user session. Supported entities: Username, Email Address (username that matches email regex).
Timeout - 600 Seconds



##### JSON Results
```json
[{"Entity":"user@domain.onmicrosoft.com","EntityResult":{"@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Edm.Boolean","value":true}},{"Entity":"username","EntityResult":{"error":"User not found."}}]
```



#### Enable Account
Enable account in Azure Active Directory. Action expects Siemplify user entity in username@domain format.
Timeout - 600 Seconds






## Jobs



## Connectors


