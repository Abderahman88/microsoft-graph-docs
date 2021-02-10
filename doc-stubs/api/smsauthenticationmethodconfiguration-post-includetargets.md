---
title: "Create smsAuthenticationMethodTarget"
description: "Create a new smsAuthenticationMethodTarget object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create smsAuthenticationMethodTarget
Namespace: microsoft.graph

Create a new smsAuthenticationMethodTarget object.

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
POST /smsAuthenticationMethodConfiguration/includeTargets
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) object.

The following table shows the properties that are required when you create the [smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|targetType|authenticationMethodTargetType|**TODO: Add Description** Inherited from [authenticationMethodTarget](../resources/authenticationmethodtarget.md). Possible values are: `user`, `group`, `unknownFutureValue`.|
|isRegistrationRequired|Boolean|**TODO: Add Description** Inherited from [authenticationMethodTarget](../resources/authenticationmethodtarget.md)|
|isUsableForSignIn|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_smsauthenticationmethodtarget_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/smsAuthenticationMethodConfiguration/includeTargets
Content-Type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodTarget",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "isUsableForSignIn": "Boolean"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.smsAuthenticationMethodTarget"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodTarget",
  "id": "db071d8a-1d8a-db07-8a1d-07db8a1d07db",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "isUsableForSignIn": "Boolean"
}
```

