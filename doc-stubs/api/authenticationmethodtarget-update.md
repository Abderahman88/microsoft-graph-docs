---
title: "Update authenticationMethodTarget"
description: "Update the properties of an authenticationMethodTarget object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update authenticationMethodTarget
Namespace: microsoft.graph

Update the properties of an [authenticationMethodTarget](../resources/authenticationmethodtarget.md) object.

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
PATCH /authenticationMethodTarget
PATCH /fido2AuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
PATCH /emailAuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [authenticationMethodTarget](../resources/authenticationmethodtarget.md) object.

The following table shows the properties that are required when you update the [authenticationMethodTarget](../resources/authenticationmethodtarget.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|targetType|authenticationMethodTargetType|**TODO: Add Description**. Possible values are: `user`, `group`, `unknownFutureValue`.|
|isRegistrationRequired|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [authenticationMethodTarget](../resources/authenticationmethodtarget.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_authenticationmethodtarget"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/authenticationMethodTarget
Content-Type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "targetType": "String",
  "isRegistrationRequired": "Boolean"
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
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "id": "c490170f-170f-c490-0f17-90c40f1790c4",
  "targetType": "String",
  "isRegistrationRequired": "Boolean"
}
```

