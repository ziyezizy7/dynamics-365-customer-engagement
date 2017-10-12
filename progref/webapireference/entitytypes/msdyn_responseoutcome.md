---
title: "Microsoft Dynamics 365 Customer Engagement msdyn_responseoutcome EntityType Reference | MicrosoftDocs"
ms.date: "2017-07-10"
ms.service: "crm-online"
ms.topic: "reference"
applies_to: 
  - "Dynamics 365 (online)"
ms.assetid: 2862d961-2c2c-4472-8971-baf502e248c1
author: "jimdaly"
ms.author: "jdaly"
manager: "jdaly"
meta-description: "Reference information about the Web API msdyn_responseoutcome entitytype."
---
# msdyn_responseoutcome EntityType
<table>
<tr><td><b>Description:</b></td><td>[!INCLUDE[./descriptions/msdyn_responseoutcome.md](./descriptions/msdyn_responseoutcome.md)]</td></tr>
<tr><td><b>Entity Set path:</b></td><td>[!include[current-web-api-base-uri.md](../includes/current-web-api-base-uri.md)]msdyn_responseoutcomes </td></tr>
<tr><td><b>Base Type:</b></td><td>[crmbaseentity EntityType](crmbaseentity.md)</td></tr>
<tr><td><b>Display Name:</b></td><td>Response Outcome</td></tr>
<tr><td><b>Primary Key:</b></td><td>msdyn_responseoutcomeid</td></tr>
<tr><td><b>Primary Name Attribute:</b></td><td>msdyn_name</td></tr>
<tr><td><b>Operations supported:</b></td><td>POST,GET,PATCH,DELETE</td></tr>
</table>
  
The msdyn_responseoutcome entitytype has no functions or actions bound to it.

## Properties
Properties represent fields of data stored in the entity. Some properties are read-only. 


|Name|Type|Details|  
|----|----|-------|  
|createdon|Edm.DateTimeOffset|**Display Name**: Created On<br />**Description**: Shows the date and time when the record was created.<br />Read-only<br />|
|importsequencenumber|Edm.Int32|**Display Name**: Import Sequence Number<br />**Description**: Shows the sequence number of the import that created this record.<br />|
|modifiedon|Edm.DateTimeOffset|**Display Name**: Modified On<br />**Description**: Shows the date and time when the record was modified.<br />Read-only<br />|
|msdyn_name|Edm.String|**Display Name**: Name<br />**Description**: The name of the custom entity.<br />|
|msdyn_responseoutcomeid|Edm.Guid|**Display Name**: Action<br />**Description**: Shows the entity instances.<br />|
|msdyn_responseoutcometype|Edm.Int32|**Display Name**: Response Outcome Type<br />**Description**: Select the response outcome type.<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>986540000</td><td>Complaint</td></tr><tr><td>986540001</td><td>Low score</td></tr><tr><td>986540002</td><td>Distress</td></tr><tr><td>986540003</td><td>Unsubscribe</td></tr><tr><td>986540004</td><td>High Score</td></tr><tr><td>986540005</td><td>Contact request</td></tr><tr><td>986540006</td><td>Follow up</td></tr><tr><td>986540007</td><td>NPS Increase</td></tr><tr><td>986540008</td><td>NPS Decrease</td></tr><tr><td>986540009</td><td>Facial Expression Increase</td></tr><tr><td>986540010</td><td>Facial Expression Decrease</td></tr><tbody></table>|
|msdyn_triggeringresponsetext|Edm.String|**Display Name**: Triggering Response Text<br />**Description**: Select the text that will trigger a response.<br />|
|overriddencreatedon|Edm.DateTimeOffset|**Display Name**: Record Created On<br />**Description**: Shows the date and time that the record was migrated.<br />|
|statecode|Edm.Int32|**Display Name**: Status<br />**Description**: Shows the status of the action.<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>0</td><td>Active</td></tr><tr><td>1</td><td>Inactive</td></tr><tbody></table>|
|statuscode|Edm.Int32|**Display Name**: Status Reason<br />**Description**: Shows the reason for the status of the action.<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>1</td><td>Active</td></tr><tr><td>2</td><td>Inactive</td></tr><tbody></table>|
|timezoneruleversionnumber|Edm.Int32|**Display Name**: Time Zone Rule Version Number<br />**Description**: For internal use only.<br />|
|utcconversiontimezonecode|Edm.Int32|**Display Name**: UTC Conversion Time Zone Code<br />**Description**: Shows the time zone code that was in use when the record was created.<br />|
|versionnumber|Edm.Int64|**Display Name**: Version Number<br />**Description**: Version Number<br />Read-only<br />|

## Lookup Properties
Lookup properties are read-only, computed properties which contain entity primary key Edm.Guid data for one or more corresponding single-valued navigation properties. More information: [Lookup properties](https://msdn.microsoft.com/library/mt607990.aspx#bkmk_lookupProperties) and [Retrieve data about lookup properties](https://msdn.microsoft.com/library/gg334767.aspx#bkmk_lookupProperty).


|Name|Single-valued navigation property|Description|  
|----|---------------------------------|-----------|  
|_createdby_value|createdby<br />|Shows the user who created the record.|
|_createdonbehalfby_value|createdonbehalfby<br />|Shows the delegate user who created the record.|
|_modifiedby_value|modifiedby<br />|Shows the user who modified the record.|
|_modifiedonbehalfby_value|modifiedonbehalfby<br />|Shows the delegate user who modified the record.|
|_msdyn_account_value|msdyn_Account<br />|Shows the account associated with the action.|
|_msdyn_contact_value|msdyn_Contact<br />|Shows Contact associated with Action.|
|_msdyn_invitation_value||Shows Survey Activity associated with Action.|
|_msdyn_lead_value|msdyn_Lead<br />|Shows Lead associated with Action.|
|_msdyn_surveyid_value|msdyn_SurveyId<br />|Shows Survey associated with Action.|
|_msdyn_surveyresponse_value|msdyn_SurveyResponse<br />|Shows Survey Response associated with Action.|
|_msdyn_triggeringresponseactionrule_value|msdyn_TriggeringResponseActionRule<br />|Shows Response Outcome Rule associated with Response Outcome.|
|_ownerid_value|ownerid<br />|Owner Id|
|_owningbusinessunit_value|owningbusinessunit<br />|Shows the business unit that owns the record|
|_owningteam_value|owningteam<br />|Unique identifier for the team that owns the record.|
|_owninguser_value|owninguser<br />|Unique identifier for the user that owns the record.|


## Single-valued navigation properties
Single-valued navigation properties represent lookup fields where a single entity can be referenced. Each single-valued navigation property has a corresponding partner collection-valued navigation property on the related entity.


|Name|Type|Partner|  
|----|----|-------|  
|createdby|[systemuser EntityType](systemuser.md)|lk_msdyn_responseoutcome_createdby|
|createdonbehalfby|[systemuser EntityType](systemuser.md)|lk_msdyn_responseoutcome_createdonbehalfby|
|modifiedby|[systemuser EntityType](systemuser.md)|lk_msdyn_responseoutcome_modifiedby|
|modifiedonbehalfby|[systemuser EntityType](systemuser.md)|lk_msdyn_responseoutcome_modifiedonbehalfby|
|msdyn_Account|[account EntityType](account.md)|msdyn_account_msdyn_responseoutcome_Account|
|msdyn_Contact|[contact EntityType](contact.md)|msdyn_contact_msdyn_responseoutcome_Contact|
|msdyn_Invitation|[msdyn_surveyinvite EntityType](msdyn_surveyinvite.md)|msdyn_msdyn_surveyinvite_msdyn_responseoutcome_Invitation|
|msdyn_Lead|[lead EntityType](lead.md)|msdyn_lead_msdyn_responseoutcome_Lead|
|msdyn_SurveyId|[msdyn_survey EntityType](msdyn_survey.md)|msdyn_msdyn_survey_msdyn_responseoutcome_SurveyId|
|msdyn_SurveyResponse|[msdyn_surveyresponse EntityType](msdyn_surveyresponse.md)|msdyn_surveyresponse_SurveyResponse|
|msdyn_TriggeringResponseActionRule|[msdyn_responseaction EntityType](msdyn_responseaction.md)|msdyn_msdyn_responseaction_msdyn_responseoutcome_TriggeringResponseActionRule|
|ownerid|[principal EntityType](principal.md)|owner_msdyn_responseoutcome|
|owningbusinessunit|[businessunit EntityType](businessunit.md)|business_unit_msdyn_responseoutcome|
|owningteam|[team EntityType](team.md)|team_msdyn_responseoutcome|
|owninguser|[systemuser EntityType](systemuser.md)|user_msdyn_responseoutcome|

## Collection-valued navigation properties
Collection-valued navigation properties represent collections of entities which may represent either a one-to-many (1:N) or many-to-many (N:N) relationship between the entities.


|Name|Type|Partner|  
|----|----|-------|  
|msdyn_responseoutcome_AsyncOperations|[asyncoperation EntityType](asyncoperation.md)|regardingobjectid_msdyn_responseoutcome|  
|msdyn_responseoutcome_BulkDeleteFailures|[bulkdeletefailure EntityType](bulkdeletefailure.md)|regardingobjectid_msdyn_responseoutcome|  
|msdyn_responseoutcome_SyncErrors|[syncerror EntityType](syncerror.md)|regardingobjectid_msdyn_responseoutcome|  

## Operations
The following operations can be used with the msdyn_responseoutcome entity type.


|Name|Binding|Description|  
|----|-------|-----------|  
|[GrantAccess Action](../actions/grantaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/grantaccess.md](../actions/descriptions/grantaccess.md)]|  
|[IsValidStateTransition Function](../functions/isvalidstatetransition.md)|Not Bound|[!INCLUDE[../functions/descriptions/isvalidstatetransition.md](../functions/descriptions/isvalidstatetransition.md)]|  
|[ModifyAccess Action](../actions/modifyaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/modifyaccess.md](../actions/descriptions/modifyaccess.md)]|  
|[RetrievePrincipalAccess Function](../functions/retrieveprincipalaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrieveprincipalaccess.md](../functions/descriptions/retrieveprincipalaccess.md)]|  
|[RetrieveSharedPrincipalsAndAccess Function](../functions/retrievesharedprincipalsandaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrievesharedprincipalsandaccess.md](../functions/descriptions/retrievesharedprincipalsandaccess.md)]|  
|[RevokeAccess Action](../actions/revokeaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/revokeaccess.md](../actions/descriptions/revokeaccess.md)]|  

## Solutions
The following solutions include the msdyn_responseoutcome entity type.


|Name|Description |  
|----|------------|  
|[Voice of the Customer for Microsoft Dynamics 365 Solution](../solutions/voiceofthecustomer.md)|[!INCLUDE[../solutions/descriptions/voiceofthecustomer.md](../solutions/descriptions/voiceofthecustomer.md)]|    

[!INCLUDE[./remarks/msdyn_responseoutcome.md](./remarks/msdyn_responseoutcome.md)]

### See also  
 [Use the Microsoft Dynamics CRM Web API](https://msdn.microsoft.com/library/mt593051.aspx)<br />
 [Web API EntityType Reference](../entitytypereference.md)<br />
 [Web API Action Reference](../actionreference.md)<br />
 [Web API Function Reference](../functionreference.md)<br />
 [Web API Query Function Reference](../queryfunctionreference.md)<br />
 [Web API EnumType Reference](../enumtypereference.md)<br />
 [Web API ComplexType Reference](../complextypereference.md)<br />
 [Web API Metadata EntityType Reference](../entitytypereference.md)<br />
 [Web API Solutions Reference](../solutionreference.md)<br />