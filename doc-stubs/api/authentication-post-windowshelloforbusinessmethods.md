---
title: "Create windowsHelloForBusinessAuthenticationMethod"
description: "Create a new windowsHelloForBusinessAuthenticationMethod object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create windowsHelloForBusinessAuthenticationMethod
Namespace: microsoft.graph

Create a new windowsHelloForBusinessAuthenticationMethod object.

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
POST /users/{usersId}/authentication/windowsHelloForBusinessMethods
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.

The following table shows the properties that are required when you create the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|keyStrength|authenticationMethodKeyStrength|**TODO: Add Description**. Possible values are: `normal`, `weak`, `unknown`.|



## Response

If successful, this method returns a `201 Created` response code and a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windowshelloforbusinessauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/authentication/windowsHelloForBusinessMethods
Content-Type: application/json
Content-length: 141

{
  "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "displayName": "String",
  "keyStrength": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "id": "3006d5ec-d5ec-3006-ecd5-0630ecd50630",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "keyStrength": "String"
}
```

