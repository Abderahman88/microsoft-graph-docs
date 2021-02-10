---
title: "print resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# print resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get print](../api/print-get.md)|[print](../resources/print.md)|Read the properties and relationships of a [print](../resources/print.md) object.|
|[Update print](../api/print-update.md)|[print](../resources/print.md)|Update the properties of a [print](../resources/print.md) object.|
|[List reportRoot](../api/print-list-reports.md)|[reportRoot](../resources/reportroot.md) collection|Get the reportRoot resources from the reports navigation property.|
|[Create reportRoot](../api/print-post-reports.md)|[reportRoot](../resources/reportroot.md)|Create a new reportRoot object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|settings|[printSettings](../resources/printsettings.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|connectors|[printConnector](../resources/printconnector.md) collection|**TODO: Add Description**|
|operations|[printOperation](../resources/printoperation.md) collection|**TODO: Add Description**|
|printers|[printer](../resources/printer.md) collection|**TODO: Add Description**|
|printerShares|[printerShare](../resources/printershare.md) collection|**TODO: Add Description**|
|reports|[reportRoot](../resources/reportroot.md)|**TODO: Add Description**|
|services|[printService](../resources/printservice.md) collection|**TODO: Add Description**|
|shares|[printerShare](../resources/printershare.md) collection|**TODO: Add Description**|
|taskDefinitions|[printTaskDefinition](../resources/printtaskdefinition.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.print",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.print",
  "settings": {
    "@odata.type": "microsoft.graph.printSettings"
  }
}
```

