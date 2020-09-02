---
title: "group resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# group resource type

Namespace: microsoft.graph.termStore

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List groups](../api/group-list.md)|[group](../resources/termstore-group.md) collection|Get a list of the [group](../resources/group.md) objects and their properties.|
|[Create group](../api/termstore-group-create.md)|[group](../resources/termstore-group.md)|Create a new [group](../resources/termstore-group.md) object.|
|[Get group](../api/termstore-group-get.md)|[group](../resources/termstore-group.md)|Read the properties and relationships of a [group](../resources/termstore-group.md) object.|
|[Update group](../api/termstore-group-update.md)|[group](../resources/termstore-group.md)|Update the properties of a [group](../resources/termstore-group.md) object.|
|[Delete group](../api/termstore-group-delete.md)|None|Deletes a [group](../resources/termstore-group.md) object.|
|[List sets](../api/termstore-group-list-sets.md)|[set](../resources/termstore-set.md) collection|Get the sets from the sets navigation property.|
|[Create sets](../api/termstore-group-post-sets.md)|[set](../resources/termstore-set.md)|Create a new sets object.|
|[Get sets](../api/termstore-group-get-set.md)|[set](../resources/termstore-set.md)|Read the properties and relationships of a [set](../resources/set.md) object.|
|[Update sets](../api/termstore-group-update-sets.md)|[set](../resources/termstore-set.md)|Update the properties of a sets object.|
|[Delete sets](../api/termstore-group-delete-sets.md)|None|Delete a [set](../resources/termstore-set.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/termstore-entity.md)|
|scope|termGroupScope|**TODO: Add Description**. Possible values are: `global`, `system`, `siteCollection`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sets|[set](../resources/termstore-set.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.group",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.group",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "scope": "String"
}
```
