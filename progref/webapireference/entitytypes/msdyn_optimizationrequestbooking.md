---
title: "Microsoft Dynamics 365 Customer Engagement msdyn_optimizationrequestbooking EntityType Reference | MicrosoftDocs"
ms.date: "2017-07-10"
ms.service: "crm-online"
ms.topic: "reference"
applies_to: 
  - "Dynamics 365 (online)"
ms.assetid: bb694fc4-f29e-4eeb-833b-b6f751b6de31
author: "jimdaly"
ms.author: "jdaly"
manager: "jdaly"
meta-description: "Reference information about the Web API msdyn_optimizationrequestbooking entitytype."
---
# msdyn_optimizationrequestbooking EntityType
<table>
<tr><td><b>Description:</b></td><td>[!INCLUDE[./descriptions/msdyn_optimizationrequestbooking.md](./descriptions/msdyn_optimizationrequestbooking.md)]</td></tr>
<tr><td><b>Entity Set path:</b></td><td>[!include[current-web-api-base-uri.md](../includes/current-web-api-base-uri.md)]msdyn_optimizationrequestbookings </td></tr>
<tr><td><b>Base Type:</b></td><td>[crmbaseentity EntityType](crmbaseentity.md)</td></tr>
<tr><td><b>Display Name:</b></td><td>Optimization Request Booking</td></tr>
<tr><td><b>Primary Key:</b></td><td>msdyn_optimizationrequestbookingid</td></tr>
<tr><td><b>Primary Name Attribute:</b></td><td>msdyn_name</td></tr>
<tr><td><b>Operations supported:</b></td><td>POST,GET,PATCH,DELETE</td></tr>
</table>
  
The msdyn_optimizationrequestbooking entitytype has no functions or actions bound to it.

## Properties
Properties represent fields of data stored in the entity. Some properties are read-only. 


|Name|Type|Details|  
|----|----|-------|  
|createdon|Edm.DateTimeOffset|**Display Name**: Created On<br />**Description**: Date and time when the record was created.<br />Read-only<br />|
|importsequencenumber|Edm.Int32|**Display Name**: Import Sequence Number<br />**Description**: Sequence number of the import that created this record.<br />|
|modifiedon|Edm.DateTimeOffset|**Display Name**: Modified On<br />**Description**: Date and time when the record was last modified.<br />Read-only<br />|
|msdyn_name|Edm.String|**Display Name**: Name<br />**Description**: Name of the custom entity.<br />|
|msdyn_operation|Edm.Int32|**Display Name**: Operation<br />**Description**: The operation, which RSO performed on the booking.<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>192350003</td><td>Unchanged</td></tr><tr><td>192350000</td><td>Create</td></tr><tr><td>192350001</td><td>Update</td></tr><tr><td>192350002</td><td>Delete</td></tr><tbody></table>|
|msdyn_operationdetails|Edm.String|**Display Name**: Operation Details<br />**Description**: The details of the operation, which RSO performed on the booking.<br />|
|msdyn_optimizationrequestbookingid|Edm.Guid|**Display Name**: Optimization Request Booking<br />**Description**: Unique identifier for entity instances.<br />|
|overriddencreatedon|Edm.DateTimeOffset|**Display Name**: Record Created On<br />**Description**: Date and time when the record was migrated.<br />|
|statecode|Edm.Int32|**Display Name**: Status<br />**Description**: Status of the optimization request booking.<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>0</td><td>Active</td></tr><tr><td>1</td><td>Inactive</td></tr><tbody></table>|
|statuscode|Edm.Int32|**Display Name**: Status Reason<br />**Description**: Reason for the status of the optimization request booking.<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>1</td><td>Active</td></tr><tr><td>2</td><td>Inactive</td></tr><tbody></table>|
|timezoneruleversionnumber|Edm.Int32|**Display Name**: Time Zone Rule Version Number<br />**Description**: Internal use only.<br />|
|utcconversiontimezonecode|Edm.Int32|**Display Name**: UTC Conversion Time Zone Code<br />**Description**: Time zone code that was in use when the record was created.<br />|
|versionnumber|Edm.Int64|**Display Name**: Version Number<br />**Description**: Version Number<br />Read-only<br />|

## Lookup Properties
Lookup properties are read-only, computed properties which contain entity primary key Edm.Guid data for one or more corresponding single-valued navigation properties. More information: [Lookup properties](https://msdn.microsoft.com/library/mt607990.aspx#bkmk_lookupProperties) and [Retrieve data about lookup properties](https://msdn.microsoft.com/library/gg334767.aspx#bkmk_lookupProperty).


|Name|Single-valued navigation property|Description|  
|----|---------------------------------|-----------|  
|_createdby_value|createdby<br />|User who created the record.|
|_createdonbehalfby_value|createdonbehalfby<br />|Delegate user who created the record.|
|_modifiedby_value|modifiedby<br />|User who last modified the record.|
|_modifiedonbehalfby_value|modifiedonbehalfby<br />|Delegate user who modified the record.|
|_msdyn_bookableresourcebooking_value|msdyn_BookableResourceBooking<br />|Bookable resource booking that corresponds to the record.|
|_msdyn_routingoptimization_value|msdyn_RoutingOptimization<br />|Scheduling optimization request ID that corresponds to the bookable resource booking.|
|_ownerid_value|ownerid<br />|Owner ID.|
|_owningbusinessunit_value|owningbusinessunit<br />|Business unit that owns the record.|
|_owningteam_value|owningteam<br />|Team that owns the record.|
|_owninguser_value|owninguser<br />|User that owns the record.|


## Single-valued navigation properties
Single-valued navigation properties represent lookup fields where a single entity can be referenced. Each single-valued navigation property has a corresponding partner collection-valued navigation property on the related entity.


|Name|Type|Partner|  
|----|----|-------|  
|createdby|[systemuser EntityType](systemuser.md)|lk_msdyn_optimizationrequestbooking_createdby|
|createdonbehalfby|[systemuser EntityType](systemuser.md)|lk_msdyn_optimizationrequestbooking_createdonbehalfby|
|modifiedby|[systemuser EntityType](systemuser.md)|lk_msdyn_optimizationrequestbooking_modifiedby|
|modifiedonbehalfby|[systemuser EntityType](systemuser.md)|lk_msdyn_optimizationrequestbooking_modifiedonbehalfby|
|msdyn_BookableResourceBooking|[bookableresourcebooking EntityType](bookableresourcebooking.md)|msdyn_bookableresourcebooking_msdyn_optimizationrequestbooking_BookableResourceBooking|
|msdyn_RoutingOptimization|[msdyn_routingoptimizationrequest EntityType](msdyn_routingoptimizationrequest.md)|msdyn_msdyn_routingoptimizationrequest_msdyn_optimizationrequestbooking_RoutingOptimization|
|ownerid|[principal EntityType](principal.md)|owner_msdyn_optimizationrequestbooking|
|owningbusinessunit|[businessunit EntityType](businessunit.md)|business_unit_msdyn_optimizationrequestbooking|
|owningteam|[team EntityType](team.md)|team_msdyn_optimizationrequestbooking|
|owninguser|[systemuser EntityType](systemuser.md)|user_msdyn_optimizationrequestbooking|

## Collection-valued navigation properties
Collection-valued navigation properties represent collections of entities which may represent either a one-to-many (1:N) or many-to-many (N:N) relationship between the entities.


|Name|Type|Partner|  
|----|----|-------|  
|msdyn_optimizationrequestbooking_AsyncOperations|[asyncoperation EntityType](asyncoperation.md)|regardingobjectid_msdyn_optimizationrequestbooking|  
|msdyn_optimizationrequestbooking_BulkDeleteFailures|[bulkdeletefailure EntityType](bulkdeletefailure.md)|regardingobjectid_msdyn_optimizationrequestbooking|  
|msdyn_optimizationrequestbooking_DuplicateBaseRecord|[duplicaterecord EntityType](duplicaterecord.md)|baserecordid_msdyn_optimizationrequestbooking|  
|msdyn_optimizationrequestbooking_DuplicateMatchingRecord|[duplicaterecord EntityType](duplicaterecord.md)|duplicaterecordid_msdyn_optimizationrequestbooking|  
|msdyn_optimizationrequestbooking_SyncErrors|[syncerror EntityType](syncerror.md)|regardingobjectid_msdyn_optimizationrequestbooking|  

## Operations
The following operations can be used with the msdyn_optimizationrequestbooking entity type.


|Name|Binding|Description|  
|----|-------|-----------|  
|[GrantAccess Action](../actions/grantaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/grantaccess.md](../actions/descriptions/grantaccess.md)]|  
|[IsValidStateTransition Function](../functions/isvalidstatetransition.md)|Not Bound|[!INCLUDE[../functions/descriptions/isvalidstatetransition.md](../functions/descriptions/isvalidstatetransition.md)]|  
|[ModifyAccess Action](../actions/modifyaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/modifyaccess.md](../actions/descriptions/modifyaccess.md)]|  
|[RetrievePrincipalAccess Function](../functions/retrieveprincipalaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrieveprincipalaccess.md](../functions/descriptions/retrieveprincipalaccess.md)]|  
|[RetrieveSharedPrincipalsAndAccess Function](../functions/retrievesharedprincipalsandaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrievesharedprincipalsandaccess.md](../functions/descriptions/retrievesharedprincipalsandaccess.md)]|  
|[RevokeAccess Action](../actions/revokeaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/revokeaccess.md](../actions/descriptions/revokeaccess.md)]|  

## Solutions
The following solutions include the msdyn_optimizationrequestbooking entity type.


|Name|Description |  
|----|------------|  
|[Resource Scheduling Optimization Solution](../solutions/resourceschedulingoptimization.md)|[!INCLUDE[../solutions/descriptions/resourceschedulingoptimization.md](../solutions/descriptions/resourceschedulingoptimization.md)]|    

[!INCLUDE[./remarks/msdyn_optimizationrequestbooking.md](./remarks/msdyn_optimizationrequestbooking.md)]

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