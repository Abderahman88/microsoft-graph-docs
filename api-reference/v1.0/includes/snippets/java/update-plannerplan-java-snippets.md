---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerPlan plannerPlan = new PlannerPlan();
plannerPlan.title = "title-value";

graphClient.planner().plans("{plan-id}")
	.buildRequest( requestOptions )
	.patch(plannerPlan);

```