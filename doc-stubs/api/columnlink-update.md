---
title: "Update columnLink"
description: "Update the properties of a columnLink object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update columnLink
Namespace: microsoft.graph

Update the properties of a [columnLink](../resources/columnlink.md) object.

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
PATCH /drive/list/contentTypes/{contentTypeId}/columnLinks/{columnLinkId}
PATCH /drives/{drivesId}/list/contentTypes/{contentTypeId}/columnLinks/{columnLinkId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [columnLink](../resources/columnlink.md) object.

The following table shows the properties that are required when you create the [columnLink](../resources/columnlink.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [columnLink](../resources/columnlink.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_columnlink"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/drive/list/contentTypes/{contentTypeId}/columnLinks/{columnLinkId}
Content-Type: application/json
Content-length: 73

{
  "@odata.type": "#microsoft.graph.columnLink",
  "name": "String"
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
  "@odata.type": "#microsoft.graph.columnLink",
  "id": "fa69663a-663a-fa69-3a66-69fa3a6669fa",
  "name": "String"
}
```
