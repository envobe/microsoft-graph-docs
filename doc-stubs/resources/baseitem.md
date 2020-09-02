---
title: "baseItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# baseItem resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List items](../api/site-list-items.md)|[baseItem](../resources/baseitem.md) collection|Get the baseItems from the items navigation property.|
|[Create items](../api/site-post-items.md)|[baseItem](../resources/baseitem.md)|Create a new items object.|
|[Update items](../api/site-update-items.md)|[baseItem](../resources/baseitem.md)|Update the properties of an items object.|
|[Get items](../api/site-get-baseitem.md)|[baseItem](../resources/baseitem.md)|Read the properties and relationships of a [baseItem](../resources/baseitem.md) object.|
|[Delete items](../api/site-delete-items.md)|None|Delete a [baseItem](../resources/baseitem.md) object.|
|[List baseItems](../api/baseitem-list.md)|[baseItem](../resources/baseitem.md) collection|Get a list of the [baseItem](../resources/baseitem.md) objects and their properties.|
|[Create baseItem](../api/baseitem-create.md)|[baseItem](../resources/baseitem.md)|Create a new [baseItem](../resources/baseitem.md) object.|
|[Get baseItem](../api/baseitem-get.md)|[baseItem](../resources/baseitem.md)|Read the properties and relationships of a [baseItem](../resources/baseitem.md) object.|
|[Update baseItem](../api/baseitem-update.md)|[baseItem](../resources/baseitem.md)|Update the properties of a [baseItem](../resources/baseitem.md) object.|
|[Delete baseItem](../api/baseitem-delete.md)|None|Deletes a [baseItem](../resources/baseitem.md) object.|
|[List createdByUser](../api/baseitem-list-createdbyuser.md)|[user](../resources/user.md) collection|Get the users from the createdByUser navigation property.|
|[Add createdByUser](../api/baseitem-post-createdbyuser.md)|[user](../resources/user.md)|Add createdByUser by posting to the createdByUser collection.|
|[Remove createdByUser](../api/baseitem-delete-createdbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List lastModifiedByUser](../api/baseitem-list-lastmodifiedbyuser.md)|[user](../resources/user.md) collection|Get the users from the lastModifiedByUser navigation property.|
|[Add lastModifiedByUser](../api/baseitem-post-lastmodifiedbyuser.md)|[user](../resources/user.md)|Add lastModifiedByUser by posting to the lastModifiedByUser collection.|
|[Remove lastModifiedByUser](../api/baseitem-delete-lastmodifiedbyuser.md)|None|Remove a [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|eTag|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|createdByUser|[user](../resources/user.md)|**TODO: Add Description**|
|lastModifiedByUser|[user](../resources/user.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.baseItem",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "eTag": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "webUrl": "String"
}
```
