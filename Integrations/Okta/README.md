
# Okta

The Okta Identity Cloud provides secure identity management with Single Sign-On, Multi-factor Authentication, Lifecycle Management (Provisioning), and more.

Python Version - 1
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root|None|True|String|https://{okta_domain}.com/|
|Api Token|None|True|Password|None|
|Verify SSL|None|False|Boolean|False|


#### Dependencies
| |
|-|
|cross/python2_secrets-1.0.5-py2.py3-none-any.whl|


## Actions
#### Ping
Test Connection With Okta
Timeout - 600 Seconds



#### List User Groups
Get the groups that the user is a member of
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User IDs Or Logins|Ids or logins of users in Okta|False|String||
|Also Run On Scope|Whether to run on entities as well as the input|False|Boolean|false|



#### Get Group
Get information about a group
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Group Ids Or Names|Ids or names of groups in Okta|True|String||
|Is Id|Whether the value is an id or a name|False|Boolean|false|



#### Add Group
Add a group
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Group Name|The name of the group in Okta|True|String||
|Group Description|The description for the group|False|String||



#### Unassign Role
Unassign a role from a user
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User IDs|Ids of users in Okta|False|String||
|Role IDs Or Names|Ids or names of roles in Okta|True|String||
|Is Id|Whether the values are ids or names|False|Boolean|false|
|Also Run On Scope|Whether to run on entities as well as the input|False|Boolean|false|



#### List Providers
List identity providers (IdPs) in your organization
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|Search the name property for a match|False|String||
|Type|Filter by type|False|String||
|Limit|Max amount of results to return|False|String|20|



#### Set Password
Set the password of a user without validating existing credentials
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User IDs Or Logins|Ids or logins of users in Okta|False|String||
|New Password|The new password|True|String||
|Add 10 Random Chars|Whether to add extra characters to every user password or not|False|Boolean|false|
|Also Run On Scope|Whether to run on entities as well as the input|False|Boolean|false|



#### Enable User
Enables the specified user
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User IDs Or Logins|Ids or logins of users in Okta|False|String||
|Is Activate|Whether to activate the user or just unsuspend|False|Boolean|false|
|Send Email If Activate|Whether to send an email after activating or not|False|Boolean|false|
|Also Run On Scope|Whether to run on entities as well as the input|False|Boolean|false|



#### List Roles
Lists all roles assigned to a user
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User IDs|Ids of users in Okta|False|String||
|Also Run On Scope|Whether to run on entities as well as the input|False|Boolean|false|



#### List Users
Get the list of users
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|Search for a match in the firstname, lastname or in the email|False|String||
|Filter|Custom search query for a subset of properties|False|String||
|Search|Custom search query for most properties|False|String||
|Limit|Max amount of results to return|False|String|200|



#### Disable User
Disables the specified user
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User IDs Or Logins|Ids of users in Okta|False|String||
|Is Deactivate|Whether to dactivate or only suspend the user|False|Boolean|false|
|Send Email If Deactivate|Whether to send an email after deactivating or not|False|Boolean|false|
|Also Run On Scope|Whether to run on entities as well as the input|False|Boolean|false|



#### Assign Role
Assign a role to a user
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User IDs|Ids of users in Okta|False|String||
|Role Types|The type of role to assign to the users|True|String||
|Also Run On Scope|Whether to run on entities as well as the input|False|Boolean|false|



#### Get User
Get information about a user
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User Ids Or Logins|Ids or logins (email or short email name) of a user in Okta, e.g. test@gmail.com or simply 'test'|False|String||
|Also Run On Scope|Whether to run on entities as well as the input|False|Boolean|false|



##### JSON Results
```json
[{"status":"ACTIVE","profile":{"mobilePhone":null,"firstName":"Test","lastName":"User","secondEmail":null,"login":"test.user@asd.com","email":"test.user@asd.com"},"passwordChanged":"2022-07-11T06:11:25.000Z","created":"2022-07-11T06:07:55.000Z","activated":null,"lastUpdated":"2022-07-11T06:11:25.000Z","_links":{"schema":{"href":"https://trial-0000.okta.com/api/v1/meta/schemas/user/osc1xxxxxxxx"},"suspend":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx/lifecycle/suspend","method":"POST"},"forgotPassword":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx/credentials/forgot_password","method":"POST"},"self":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx"},"expirePassword":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx/lifecycle/expire_password","method":"POST"},"resetFactors":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx/lifecycle/reset_factors","method":"POST"},"deactivate":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx/lifecycle/deactivate","method":"POST"},"changePassword":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx/credentials/change_password","method":"POST"},"changeRecoveryQuestion":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx/credentials/change_recovery_question","method":"POST"},"type":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx"},"resetPassword":{"href":"https://trial-0000.okta.com/api/v1/users/00u1xxxxxxxx/lifecycle/reset_password","method":"POST"}},"lastLogin":"2022-07-11T06:15:14.000Z","credentials":{"password":{},"provider":{"type":"OKTA","name":"OKTA"}},"type":{"id":"oty1xxxxxxxxxxxxx"},"id":"oty1xxxxxxxxxxxxx","statusChanged":"2022-07-11T06:11:25.000Z"}]
```



#### Reset Password
Generate a one-time token that can be used to reset a user's password
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User IDs Or Logins|Ids or logins of users in Okta|False|String||
|Send Email|Whether to send an email for the password reset or return the token for every user|False|Boolean|false|
|Also Run On Scope|Whether to run on entities as well as the input|False|Boolean|false|






## Jobs



## Connectors


