---
product-area: projects
navigation-topic: approvals
title: Connect Workfront and Frame.io
description: Workfront uses Frame.io in the review and approval process to meet people where they want to work. The project management and approval process is managed in Workfront, and the review process is done in Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 8529b4d5-9732-4dd6-bf81-191aea1ed68c
---
# Connect Workfront and Frame.io

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Workfront uses Frame.io in the review and approval process to meet people where they want to work. The project management and approval process is managed in Workfront, and the review process is completed in Frame.io. You must complete all of the following sections to successfully set up the integration:

* [Connect a Workfront Group to a Frame.io Team](#connect-a-workfront-group-to-a-frameio-team)
* [Create a Workfront project and add a connected group ](#create-a-workfront-project-and-add-a-connected-group)



## Access requirements

* Your organization must be manually onboarded to the beta use the functionality described in this article. For more information, see [Adobe Workfront and Frame.io native integration beta](/help/quicksilver/review-and-approve-work/Documents/wf-frame-alpha.md).


## Connect a Workfront Group to a Frame.io Team

We are actively improving this feature for general availability in May.

### Prerequisites

* Create a Frame.io team to map to a Workfront group.
* Find the API developer token for the team. For more information, see [Developer tokens](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) on the Frame.io developer site.

### Connect a Workfront Group to a Frame.io Team

{{step-1-to-setup}}

1. In the left panel, click **Groups**.
1. Choose an existing group, or click **Create group**. 
1. In the left panel, click **Connect to Frame.io**. 
![](assets/connect-frame-group.png)
1. Enter the API developer token.
1. Click **Initiate Connection**.
1. (Conditional) If you are the administrator of more than one Frame.io account, select the account you want to use.

## Create a Workfront project and add a connected group 

After you've connected a Workfront Group to a Frame.io team, you must create a project with that connected group.

### Prerequisites

* You must have a Workfront group connected to a Frame.io team as explained in the previous section.

### Create a Workfront project and add a connected group 

{{step1-to-projects}}

1. Create a new project from scratch or a template. For information on how to create a project, see [Create a project](/help/quicksilver/manage-work/projects/create-projects/create-project.md). 

1. In the left panel, find **Project Details**. 

1. Find the **Group** field on the right side of the screen, and remove the Default group.  

1. In the drop-down menu, find the desired group. Groups connected with Frame.io display the Frame.io icon.
![](assets/add-frame-group.png)

1. Make any other project configuration changes. 

1. Click **Save Changes**.   

1. Continue to the next section.

### Add a task and set the integration status to Active 

>[!NOTE]
>
>Subtasks are not currently supported in connected Frame.io projects.


1. Create the tasks you need to populate in Frame.io 

1. Select the tasks you need, then click **Edit**. 

1. Scroll to the **Custom Forms** section, and find the Frame.io integration form.  

    >[!IMPORTANT]
    >
    >A connected Frame.io group must be assigned in the Project Details area for this form to appear. For more information see [Create a Workfront project and add a connected group](#create-a-workfront-project-and-add-a-connected-group) in this article.
    

1. Enable the **This task's integration status** checkbox, and choose **Active**. 
    ![](assets/frame-custom-form.png)

1. Click **Save Changes**. A Frame.io icon displays next to the project name. 

1. Assign users or teams to tasks. 

    >[!NOTE]
    >
    >Users or teams added to the tasks are also added to the Frame.io project. 

1. Upload any documents or creative briefs in the Project Documents area. 

The project is still not connected, you must continue to the next section to finish the integration. 

### Enable the project in Frame.io 

1. Change the Project status from **Planning** to **Current** or a custom status that equals current. This finishes the integration and generates the project, tasks, and any documents in Frame.io. 

The Frame.io icon next to the project name turns purple signaling the integration was successful. Users receive an email inviting them to the Frame.io project.

>[!IMPORTANT]
>
>Once the project is connected for Frame.io, changes made to the project group are not reflected in Frame.io.
