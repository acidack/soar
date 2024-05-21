# Analyst View Hands On




**Enabled:** False

**Version:** 0

**Type:** Playbook

**Priority:** 2

**Playbook Simulator:** True


### Playbook Trigger
**Trigger Type:** Custom Trigger

**Conditions Operator:** And

##### Conditions
|Key|Operator|Value|
|---|--------|-----|
|1|Equals|2|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|1_simple string match|Search for the 'Search For' parameter in the input text or loop through the 'Search For Regex' list and find matches in the input text.  If there is a match, the action will return true.|Tools|Search Text|
|5_NonResolvingPlaceholders|Search for the 'Search For' parameter in the input text or loop through the 'Search For Regex' list and find matches in the input text.  If there is a match, the action will return true.|Tools|Search Text|
|3_json, comma separated and arrays|Search for the 'Search For' parameter in the input text or loop through the 'Search For Regex' list and find matches in the input text.  If there is a match, the action will return true.|Tools|Search Text|
|7_Auto JSON to HTML Table|This Action will render a complete HTML table from the JSON/Array input.Note -The output can be used directly in a HTML <body> however for xtra functionality use the predefined Widget.|TemplateEngine|Render Auto HTML Table|
|8_Native Jinja|This action will render a Jinja2 template using a JSON input.  |TemplateEngine|Render Template|
|Change case name|The action changes the case's name (title)|Tools|Change Case Name|
|11_Jinja with Filters|This action will render a Jinja2 template using a JSON input.  |TemplateEngine|Render Template|
|9 Jinja Auto HTML|This Action will render a complete HTML table from the JSON/Array input.Note -The output can be used directly in a HTML <body> however for xtra functionality use the predefined Widget.|TemplateEngine|Render Auto HTML Table|
|0_Insight|Add a general insight configurable message to the case|Siemplify|Add General Insight|
|GoogleChronicle_Enrich IP_1|Enrich IP entities using information from IOCs in Google Chronicle. Supported entities: IP address.|GoogleChronicle|Enrich IP|
|10_Jinja from Array|This action will render a Jinja2 template using a JSON input.  |TemplateEngine|Render Template from Array|
|2_Simple string match, formatted|Search for the 'Search For' parameter in the input text or loop through the 'Search For Regex' list and find matches in the input text.  If there is a match, the action will return true.|Tools|Search Text|
|4_matches into JS var|Search for the 'Search For' parameter in the input text or loop through the 'Search For Regex' list and find matches in the input text.  If there is a match, the action will return true.|Tools|Search Text|

