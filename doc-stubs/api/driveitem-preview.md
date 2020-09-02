---
title: "driveItem: preview"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# driveItem: preview
Namespace: microsoft.graph

**TODO: Add Description**

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
POST /drive/root/preview
POST /drives/{drivesId}/root/preview
POST /shares/{sharesId}/root/preview
POST /drive/items/{driveItemId}/preview
POST /shares/{sharesId}/driveItem/preview
POST /drive/bundles/{driveItemId}/preview
POST /drive/special/{driveItemId}/preview
POST /drive/following/{driveItemId}/preview
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|viewer|String|**TODO: Add Description**|
|chromeless|Boolean|**TODO: Add Description**|
|allowEdit|Boolean|**TODO: Add Description**|
|page|String|**TODO: Add Description**|
|zoom|Double|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [itemPreviewInfo](../resources/itempreviewinfo.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_preview"
}
-->
``` http
POST https://graph.microsoft.com/beta/drive/root/preview

Content-Type: application/json
Content-length: 123

{
  "viewer": "String",
  "chromeless": "Boolean",
  "allowEdit": "Boolean",
  "page": "String",
  "zoom": "Double"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPreviewInfo"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": {
    "@odata.type": "microsoft.graph.itemPreviewInfo"
  }
}
```
