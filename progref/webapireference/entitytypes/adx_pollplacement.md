---
title: "Microsoft Dynamics 365 Customer Engagement adx_pollplacement EntityType Reference | MicrosoftDocs"
ms.date: "2017-07-10"
ms.service: "crm-online"
ms.topic: "reference"
applies_to: 
  - "Dynamics 365 (online)"
ms.assetid: 999fa591-66c7-414b-9348-c4dfa29a727a
author: "jimdaly"
ms.author: "jdaly"
manager: "jdaly"
meta-description: "Reference information about the Web API adx_pollplacement entitytype."
---
# adx_pollplacement EntityType
<table>
<tr><td><b>Description:</b></td><td>[!INCLUDE[./descriptions/adx_pollplacement.md](./descriptions/adx_pollplacement.md)]</td></tr>
<tr><td><b>Entity Set path:</b></td><td>[!include[current-web-api-base-uri.md](../includes/current-web-api-base-uri.md)]adx_pollplacements </td></tr>
<tr><td><b>Base Type:</b></td><td>[crmbaseentity EntityType](crmbaseentity.md)</td></tr>
<tr><td><b>Display Name:</b></td><td>Poll Placement</td></tr>
<tr><td><b>Primary Key:</b></td><td>adx_pollplacementid</td></tr>
<tr><td><b>Primary Name Attribute:</b></td><td>adx_name</td></tr>
<tr><td><b>Operations supported:</b></td><td>POST,GET,PATCH,DELETE</td></tr>
</table>
  
The adx_pollplacement entitytype has no functions or actions bound to it.

## Properties
Properties represent fields of data stored in the entity. Some properties are read-only. 


|Name|Type|Details|  
|----|----|-------|  
|adx_name|Edm.String|**Display Name**: Name<br />**Description**: Type the name of the custom entity.<br />|
|adx_pollplacementid|Edm.Guid|**Display Name**: Poll Placement<br />**Description**: Shows the entity instance.<br />|
|createdon|Edm.DateTimeOffset|**Display Name**: Created On<br />**Description**: Shows the date and time when the record was created.<br />Read-only<br />|
|importsequencenumber|Edm.Int32|**Display Name**: Import Sequence Number<br />**Description**: Shows the sequence number of the import that created this record.<br />|
|modifiedon|Edm.DateTimeOffset|**Display Name**: Modified On<br />**Description**: Shows the date and time when the record was modified.<br />Read-only<br />|
|overriddencreatedon|Edm.DateTimeOffset|**Display Name**: Record Created On<br />**Description**: Shows the date and time that the record was migrated.<br />|
|statecode|Edm.Int32|**Display Name**: Status<br />**Description**: Status of the Poll Placement<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>0</td><td>Active</td></tr><tr><td>1</td><td>Inactive</td></tr><tbody></table>|
|statuscode|Edm.Int32|**Display Name**: Status Reason<br />**Description**: Select the poll placement's status.<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>1</td><td>Active</td></tr><tr><td>2</td><td>Inactive</td></tr><tbody></table>|
|timezoneruleversionnumber|Edm.Int32|**Display Name**: Time Zone Rule Version Number<br />**Description**: For internal use only.<br />|
|utcconversiontimezonecode|Edm.Int32|**Display Name**: UTC Conversion Time Zone Code<br />**Description**: Shows the time zone code that was in use when the record was created.<br />|
|versionnumber|Edm.Int64|**Display Name**: Version Number<br />**Description**: Version Number<br />Read-only<br />|

## Lookup Properties
Lookup properties are read-only, computed properties which contain entity primary key Edm.Guid data for one or more corresponding single-valued navigation properties. More information: [Lookup properties](https://msdn.microsoft.com/library/mt607990.aspx#bkmk_lookupProperties) and [Retrieve data about lookup properties](https://msdn.microsoft.com/library/gg334767.aspx#bkmk_lookupProperty).


|Name|Single-valued navigation property|Description|  
|----|---------------------------------|-----------|  
|_adx_websiteid_value|adx_websiteid<br />|Unique identifier for Website associated with Poll Placement.|
|_adx_webtemplateid_value|adx_webtemplateid<br />|Unique identifier for Web Template associated with Poll Placement.|
|_createdby_value|createdby<br />|Shows who created the record.|
|_createdonbehalfby_value|createdonbehalfby<br />|Shows who created the record on behalf of another user.|
|_modifiedby_value|modifiedby<br />|Shows who last updated the record.|
|_modifiedonbehalfby_value|modifiedonbehalfby<br />|Shows who last updated the record on behalf of another user.|
|_ownerid_value|ownerid<br />|Enter the user who is assigned to manage the record. This field is updated every time the record is assigned to a different user.|
|_owningbusinessunit_value|owningbusinessunit<br />|Shows the business unit that owns the record.|
|_owningteam_value|owningteam<br />|Unique identifier for the team that owns the record.|
|_owninguser_value|owninguser<br />|Unique identifier for the user that owns the record.|


## Single-valued navigation properties
Single-valued navigation properties represent lookup fields where a single entity can be referenced. Each single-valued navigation property has a corresponding partner collection-valued navigation property on the related entity.


|Name|Type|Partner|  
|----|----|-------|  
|adx_websiteid|[adx_website EntityType](adx_website.md)|adx_website_pollplacement|
|adx_webtemplateid|[adx_webtemplate EntityType](adx_webtemplate.md)|adx_webtemplate_pollplacement|
|createdby|[systemuser EntityType](systemuser.md)|lk_adx_pollplacement_createdby|
|createdonbehalfby|[systemuser EntityType](systemuser.md)|lk_adx_pollplacement_createdonbehalfby|
|modifiedby|[systemuser EntityType](systemuser.md)|lk_adx_pollplacement_modifiedby|
|modifiedonbehalfby|[systemuser EntityType](systemuser.md)|lk_adx_pollplacement_modifiedonbehalfby|
|ownerid|[principal EntityType](principal.md)|owner_adx_pollplacement|
|owningbusinessunit|[businessunit EntityType](businessunit.md)|business_unit_adx_pollplacement|
|owningteam|[team EntityType](team.md)|team_adx_pollplacement|
|owninguser|[systemuser EntityType](systemuser.md)|user_adx_pollplacement|

## Collection-valued navigation properties
Collection-valued navigation properties represent collections of entities which may represent either a one-to-many (1:N) or many-to-many (N:N) relationship between the entities.


|Name|Type|Partner|  
|----|----|-------|  
|adx_pollplacement_ActivityPointers|[activitypointer EntityType](activitypointer.md)|regardingobjectid_adx_pollplacement|  
|adx_pollplacement_adx_alertsubscriptions|[adx_alertsubscription EntityType](adx_alertsubscription.md)|regardingobjectid_adx_pollplacement_adx_alertsubscription|  
|adx_pollplacement_adx_inviteredemptions|[adx_inviteredemption EntityType](adx_inviteredemption.md)|regardingobjectid_adx_pollplacement_adx_inviteredemption|  
|adx_pollplacement_adx_portalcomments|[adx_portalcomment EntityType](adx_portalcomment.md)|regardingobjectid_adx_pollplacement_adx_portalcomment|  
|adx_pollplacement_Annotations|[annotation EntityType](annotation.md)|objectid_adx_pollplacement|  
|adx_pollplacement_Appointments|[appointment EntityType](appointment.md)|regardingobjectid_adx_pollplacement_appointment|  
|adx_pollplacement_AsyncOperations|[asyncoperation EntityType](asyncoperation.md)|regardingobjectid_adx_pollplacement|  
|adx_pollplacement_BulkDeleteFailures|[bulkdeletefailure EntityType](bulkdeletefailure.md)|regardingobjectid_adx_pollplacement|  
|adx_pollplacement_DuplicateBaseRecord|[duplicaterecord EntityType](duplicaterecord.md)|baserecordid_adx_pollplacement|  
|adx_pollplacement_DuplicateMatchingRecord|[duplicaterecord EntityType](duplicaterecord.md)|duplicaterecordid_adx_pollplacement|  
|adx_pollplacement_Emails|[email EntityType](email.md)|regardingobjectid_adx_pollplacement_email|  
|adx_pollplacement_Faxes|[fax EntityType](fax.md)|regardingobjectid_adx_pollplacement_fax|  
|adx_pollplacement_Letters|[letter EntityType](letter.md)|regardingobjectid_adx_pollplacement_letter|  
|adx_pollplacement_msdyn_approvals|[msdyn_approval EntityType](msdyn_approval.md)|regardingobjectid_adx_pollplacement_msdyn_approval|  
|adx_pollplacement_msdyn_bookingalerts|[msdyn_bookingalert EntityType](msdyn_bookingalert.md)|regardingobjectid_adx_pollplacement_msdyn_bookingalert|  
|adx_pollplacement_msdyn_surveyinvites|[msdyn_surveyinvite EntityType](msdyn_surveyinvite.md)|regardingobjectid_adx_pollplacement_msdyn_surveyinvite|  
|adx_pollplacement_PhoneCalls|[phonecall EntityType](phonecall.md)|regardingobjectid_adx_pollplacement_phonecall|  
|adx_pollplacement_poll|[adx_poll EntityType](adx_poll.md)|adx_pollplacement_poll|  
|adx_pollplacement_RecurringAppointmentMasters|[recurringappointmentmaster EntityType](recurringappointmentmaster.md)|regardingobjectid_adx_pollplacement_recurringappointmentmaster|  
|adx_pollplacement_ServiceAppointments|[serviceappointment EntityType](serviceappointment.md)|regardingobjectid_adx_pollplacement_serviceappointment|  
|adx_pollplacement_SocialActivities|[socialactivity EntityType](socialactivity.md)|regardingobjectid_adx_pollplacement_socialactivity|  
|adx_pollplacement_SyncErrors|[syncerror EntityType](syncerror.md)|regardingobjectid_adx_pollplacement|  
|adx_pollplacement_Tasks|[task EntityType](task.md)|regardingobjectid_adx_pollplacement_task|  

## Operations
The following operations can be used with the adx_pollplacement entity type.


|Name|Binding|Description|  
|----|-------|-----------|  
|[GrantAccess Action](../actions/grantaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/grantaccess.md](../actions/descriptions/grantaccess.md)]|  
|[IsValidStateTransition Function](../functions/isvalidstatetransition.md)|Not Bound|[!INCLUDE[../functions/descriptions/isvalidstatetransition.md](../functions/descriptions/isvalidstatetransition.md)]|  
|[ModifyAccess Action](../actions/modifyaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/modifyaccess.md](../actions/descriptions/modifyaccess.md)]|  
|[RetrievePrincipalAccess Function](../functions/retrieveprincipalaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrieveprincipalaccess.md](../functions/descriptions/retrieveprincipalaccess.md)]|  
|[RetrieveSharedPrincipalsAndAccess Function](../functions/retrievesharedprincipalsandaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrievesharedprincipalsandaccess.md](../functions/descriptions/retrievesharedprincipalsandaccess.md)]|  
|[RevokeAccess Action](../actions/revokeaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/revokeaccess.md](../actions/descriptions/revokeaccess.md)]|  

## Solutions
The following solutions include the adx_pollplacement entity type.


|Name|Description |  
|----|------------|  
|[Dynamics 365 Portals - Portal Base Solution](../solutions/microsoftcrmportalbase.md)|[!INCLUDE[../solutions/descriptions/microsoftcrmportalbase.md](../solutions/descriptions/microsoftcrmportalbase.md)]|    

[!INCLUDE[./remarks/adx_pollplacement.md](./remarks/adx_pollplacement.md)]

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