---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
	.ReapplyFilters()
	.Request()
	.PostAsync();

```