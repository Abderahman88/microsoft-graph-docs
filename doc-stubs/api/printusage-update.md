---
title: "Update printUsage"
description: "Update the properties of a printUsage object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update printUsage
Namespace: microsoft.graph

Update the properties of a [printUsage](../resources/printusage.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
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
PATCH /printUsage
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [printUsage](../resources/printusage.md) object.

The following table shows the properties that are required when you update the [printUsage](../resources/printusage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|usageDate|Date|**TODO: Add Description**|
|completedBlackAndWhiteJobCount|Int64|**TODO: Add Description**|
|completedColorJobCount|Int64|**TODO: Add Description**|
|incompleteJobCount|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [printUsage](../resources/printusage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_printusage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/printUsage
Content-Type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.printUsage",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer"
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
  "@odata.type": "#microsoft.graph.printUsage",
  "id": "72c831e9-31e9-72c8-e931-c872e931c872",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer"
}
```

