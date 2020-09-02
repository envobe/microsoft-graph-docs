---
title: "Update relation"
description: "Update the properties of a relation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update relation
Namespace: microsoft.graph.termStore

Update the properties of a [relation](../resources/termstore-relation.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /termStore/groups/{groupId}/sets/{setId}/relations/{relationId}
PATCH /termStore/groups/{groupId}/sets/{setId}/terms/{termId}/relations/{relationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [relation](../resources/termstore-relation.md) object.

The following table shows the properties that are required when you create the [relation](../resources/termstore-relation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/termstore-entity.md)|
|relationship|relationType|**TODO: Add Description**. Possible values are: `pin`, `reuse`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [relation](../resources/termstore-relation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_relation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets/{setId}/relations/{relationId}
Content-Type: application/json
Content-length: 89

{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "relationship": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "e113f41f-f41f-e113-1ff4-13e11ff413e1",
  "relationship": "String"
}
```
