---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeView = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
	.Range("A1:Z10")
	.VisibleView()
	.Request()
	.GetAsync();

```