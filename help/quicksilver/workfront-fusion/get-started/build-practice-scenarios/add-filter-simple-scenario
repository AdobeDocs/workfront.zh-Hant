---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Add a filter to a basic scenario
description: Filters allow you to ensure that your scenario progresses only if certain conditions are met.
author: Becky
feature: Workfront Fusion
---
# Add a filter to a basic scenario  in [!DNL Adobe Workfront Fusion]

Filters allow you to ensure that your scenario progresses only if certain conditions are met. 

In this example, you will add a filter to your scenario that allows a new project to be created from a request only if the request was submitted to a specific request queue.

This example modifies the scenario created in [Create a basic scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront trigger modules include filters that allow a scenario to start only if certain conditions are met. However, because between-module filters are used for every non-trigger and non-Workfront use case, it is important to learn how to use filters between modules. This example uses a between-module filter for functionality that could be met with an in-module filter.

## Prerequisites

You must create the scenario described in [Create a basic scenario](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) before following this procedure.

## Add a filter 

### Prepare to add the filter

1. Open the first scenario.
1. In the **Outputs** area, select `Project`. 
   You should now have `ID`, `Name`, and `Project` selected.
1. Click OK to save the module settings.
1. Open Workfront. 
1. In Workfront, locate the project that represents the request queue that the Fusion scenario will be working with. 

   This project must be in the same Workfront account that the Fusion connection is set up for.
   
1. Make note of the project ID in the URL.

   Example: https://\<MyDomain\>.my.workfront.com/project/\<ProjectID\>/tasks

### Add and configure the filter

1. Open the scenario in the scenario editor.
1. Click the wrench icon ![Wrench icon](assets/wrench-icon.png) between the first and second module, and select **Set up a filter**.
1. In the Label field, enter a label for this filter, such as "Filter for request queue."
1. In the **Condition** area, in the top field, map the `projectID` from the first module.

   ![Map project ID](assets/map-proj-id.png)
1. Leave the **Condition** operator as Equal to.
1. In the bottom field of the **Condition** area, paste in the project ID that you made note of from the project URL in [Prepare to add the filter](#prepare-to-add-the-filter).
1. Click **OK** to save the filter settings.

### Test and activate

1. Go to the Workfront environment that Fusion is connecting to and add an issue to the project that you specified in the filter. Add another issue to a different project. 
1. Click **[!UICONTROL Run once]** in the lower-left corner of the scenario editor.
1. Examine the output to ensure that the scenario ran as expected.

   Both issues should appear in the output of the first scenario, but only the issue in the specified project should appear as input into the second scenario,
1. When you are satisfied that the scenario is working as expected, click the **Scheduling** toggle in the lower-left of the screen to **On**.

   This activates the scenario. 
1. In [!DNL Workfront Fusion], click **[!UICONTROL Save]** near the lower-left corner to save your progress on the scenario.

   >[!IMPORTANT]
   >
   >Save often as you hone and test a scenario.

## Resources

* For more information on filters, see [Add a filter to a scenario](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

