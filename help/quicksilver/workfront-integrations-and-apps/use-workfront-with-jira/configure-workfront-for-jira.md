---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 設定 [!DNL Adobe Workfront for Jira]
description: 您可以使用 [!DNL Adobe Workfront for Jira] 整合 [!DNL Jira] 和 [!DNL Workfront] 系統。
author: Becky
feature: Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: ddd1c964c4c885f71dfa30d1790cfbc6e26d6781
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 0%

---

# 設定[!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們已改用使用Workfront自動化與整合(Fusion)的現代、彈性整合方法。 在此轉換程式中，不再提供Jira整合&#x200B;**的Workfront**。
>
>根據貴組織與Jira的整合需求，我們建議使用Workfront自動化和整合。
>
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Jira的Workfront自動化與整合模組特定功能的相關資訊，請參閱[Jira軟體模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new)。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

<!--

You can use [!DNL Adobe Workfront for Jira] to integrate your [!DNL Jira] and [!DNL Workfront] systems.

After installing the add-on, you can define workflows that create [!DNL Jira] issues automatically when [!DNL Workfront] work items are created. The items in both applications become linked, and some of their information automatically updates in both systems.

All users in [!DNL Workfront] and [!DNL Jira] can benefit from this integration. They only need a license for the system in which they work the most, and not for both systems. 

This add-on is available for both the [!UICONTROL Server] and [!UICONTROL OnDemand] (or [!UICONTROL Cloud]) versions of [!DNL Jira] Software.

For a list of [!DNL Jira] versions that [!DNL Workfront for Jira] currently supports, see [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) at the [!DNL Atlassian Marketplace].

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira access</td> 
   <td> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in Jira and Workfront to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you can configure [!DNL Workfront for Jira], you must:

* Install [!DNL Workfront for Jira].
   For instructions on installing [!DNL Workfront for Jira], see [Install [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configure [!DNL Workfront for Jira]

By configuring [!DNL Workfront for Jira], you can:

* Define triggers that will create [!DNL Jira] items when [!DNL Workfront] items are created.
* Specify which fields should synchronize between items linked between [!DNL Jira] and [!DNL Workfront].

>[!NOTE]
>
>* After you configure [!DNL Workfront for Jira] on your [!DNL Jira] environment, all [!DNL Jira] users see a [!DNL Workfront] right panel on all [!DNL Jira] items. The panel contains information about the items that might be linked from [!DNL Workfront] or specifies that no [!DNL Workfront] items are linked to [!DNL Jira] items. 
>* When using the [!DNL Jira Server] installation, only the issues that are associated with projects identified as triggers for the Workfront integration display the Workfront panel. For more information about setting up triggers for the [!DNL Workfront to Jira] workflow, see [Configure triggers for automatically linking items between [!DNL Jira] and [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

To configure [!DNL Workfront for Jira]:

1. Log in to [!DNL Jira] as a [!DNL Jira] administrator.
1. Click **[!UICONTROL Settings]** in the main [!DNL Jira] menu.
1. Click **[!UICONTROL Add-ons]**, then click **[!UICONTROL Manage add-ons]**.

1. Expand the **[!DNL Workfront]** add-on.
1. Click **[!UICONTROL Configure]**.
1. Follow the prompts to log in to [!DNL Workfront].

   >[!NOTE]
   >
   >The user must have a valid `apiKey` in [!UICONTROL Workfront] to create a successful connection.

   You must log in to [!DNL Workfront] as a [!DNL Workfront] administrator to continue the configuration.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] connects to [!DNL Jira] using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.
   >* When you are prompted to enter the domain of your [!DNL Workfront] account, type it using this format: *yourCompany'sDomain.my.workfront.com*. Your company's domain is usually the name of your company.
   >* Enhanced Authentication is not available until a [!DNL Workfront] administrator enables it for this integration.

1. In Jira, select the **[!UICONTROL Triggers]** tab to configure the automatic creation of [!DNL Jira] items as new [!DNL Workfront] items are created.

   For more information about setting up triggers for the Workfront to [!DNL Jira] workflow, see [Configure triggers for automatically linking items between [!DNL Jira] and [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Select the **[!UICONTROL Setup]** tab to configure the synchronization of fields between linked [!DNL Jira] and [!DNL Workfront] items.

   For more information about setting up the synchronization of fields between [!DNL Jira] and [!DNL Workfront], see [Configure field synchronization between [!DNL Jira] and [!DNL Workfront] Items](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >After you define the triggers and the synchronization of fields between the two applications, any [!DNL Workfront] user who can create tasks or issues could potentially trigger the creation of an item in [!DNL Jira]. The user can create an item if the criteria on the item they create match the triggers in [!DNL Jira], even if the user does not have a [!DNL Jira] license. Also, any [!DNL Jira] user can immediately start working on the [!DNL Jira] item, and their updates are visible in [!DNL Workfront], without them having a [!DNL Workfront] license. Any updates in [!DNL Workfront] are also visible on the [!DNL Jira] items. 

1. (Optional) Select the **[!UICONTROL Activity Log]** tab to review any errors that might have occurred during the integration.

   For more information about the [!UICONTROL Activity Log], see [View the [!DNL Jira] [!UICONTROL Activity Log]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configure triggers for automatically linking items between [!DNL Jira] and [!DNL Workfront] 

As the [!DNL Jira] system administrator, you can define triggers that would automatically create issues in [!DNL Jira] when an item in [!DNL Workfront] meets certain criteria.

>[!NOTE]
>
>It could take up to 10 minutes for the integration to create new issues in [!DNL Jira].

Consider the following when configuring triggering the creation of [!DNL Jira] items as [!DNL Workfront] items are created:

* The integration is unidirectional: You can only trigger items that you create in [!DNL Workfront] to be automatically created in [!DNL Jira]. You cannot trigger items that you create in [!DNL Jira] to automatically be created in [!DNL Workfront]. 
* There is no limit to how many triggers you can have. 
* If an item that you create in [!DNL Workfront] matches more than one of the triggers, only one item is created in [!DNL Jira]. The item is created in [!DNL Jira] according to the first trigger (in the order that they have been defined in [!DNL Jira]). All other triggers are ignored. 
* Only one item in [!DNL Workfront] can be linked to one item in Jira. You can never link one [!DNL Workfront] item to multiple [!DNL Jira] issues, or one [!DNL Jira] issue to multiple [!DNL Workfront] items. 

To configure triggers for automatically creating items in [!DNL Jira]: 

1. Log in to [!DNL Jira] as a system administrator.
1. Click **[!UICONTROL Settings]** in the main [!DNL Jira] menu.
1. Click **[!UICONTROL Add-ons]**, then **[!UICONTROL Manage add-ons]**.
1. Expand the **[!DNL Workfront]** add-on.
1. Click **[!UICONTROL Configure]**.
1. Log in to [!DNL Workfront] as a system administrator.

   The **[!UICONTROL Triggers]** tab is selected by default in Jira.

1. Click **[!UICONTROL Add trigger]** to add a new trigger.
1. In the **[!UICONTROL Workfront team/user/role]** field, specify the name of a [!DNL Workfront] team, user, or job role, then click to select it when it displays in the list. 

   >[!NOTE]
   >
   >You cannot have multiple triggers for the same team, user, or role.

   When someone creates a task or an issue and assigns it to one of these entities, an issue is automatically created in [!DNL [!DNL Jira]].

1. In the **[!UICONTROL [!DNL Jira] project]** field, start typing the name of a [!DNL Jira] project, then click to select it when it displays in the list.

   When the [!DNL Jira] issue is created, it is placed on the project you chose here.

1. Select an **I[!UICONTROL ssue type]** from the drop-down menu.

   This indicates the issue type that is created in [!DNL Jira] when the conditions of this trigger are met, based on your settings for that specific project in [!DNL Jira].

1. Click **[!UICONTROL Save]**. 

   With this configuration, every time a [!DNL Workfront] user creates an item that matches the specified triggers, a new issue is created in [!DNL Jira].

## Configure field synchronization between [!DNL Jira] and [!DNL Workfront] Items 

As the [!DNL Jira] administrator, you can define which fields should automatically synchronize on items that are linked between [!DNL Workfront] and Jira. Certain fields can synchronize from the [!DNL Workfront] to the [!DNL Jira] item, and others synchronize from Jira to Workfront. 

To define what fields should automatically synchronize on items linked between the two applications:

1. Log in to [!DNL Jira] as a Jira administrator.
1. Click **[!UICONTROL Settings]** in the main [!DNL Jira] menu.
1. Click **[!UICONTROL Add-ons]**, then **[!UICONTROL Manage add-ons]**.
1. Expand the **[!DNL Workfront]** add-on.
1. Click **[!UICONTROL Configure]**.
1. Log in to [!DNL Workfront] as a Workfront administrator.
1. In Jira, click the **[!UICONTROL Setup]** tab.
1. In the **[!UICONTROL Synchronize from Workfront to Jira]** section, select the fields that you want to update in [!DNL Jira] when they are updated in Workfront. 

   1. Select any of the following frequencies with which the fields are synchronized:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>The fields you specify are synchronized between the linked Workfront and [!DNL Jira] items when the item is created in Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>The fields you specify are synchronized between the linked Workfront and [!DNL Jira] items when the fields are updated in Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>The fields you specify are never synchronized between the linked [!DNL Workfront] and [!DNL Jira] items. There is no indication in [!DNL Jira] that the field was updated in [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Select any of the following to synchronize the fields from [!DNL Workfront] to [!DNL Jira]: 

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>The name of a task or an issue in [!DNL Workfront] becomes the name of the issue to which it is linked in [!DNL Jira].</p><p>Note: When new items are created in [!DNL Jira] automatically, the [!DNL Workfront] Name always updates on the [!DNL Jira] item, regardless of whether this field is enabled here or not. When a [!DNL Jira] item is manually linked to a [!DNL Workfront] item, the Name of the [!DNL Workfront] item only updates in [!DNL Jira] when you select to <strong>Always</strong> synchronize this field. For more information about linking items manually or automatically, see <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Link items between [!DNL Adobe Workfront] and [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>The description of a task or an issue in [!DNL Workfront] becomes the description of the issue to which it is linked in [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documents</td>
         <td><p>Documents attached to a task or an issue in [!DNL Workfront] are also attached to the issue to which it is linked in Jira. New document versions from [!DNL Workfront] are added as separate documents to Jira and are appended with <i>_v&lt;version number></i> to indicate the numbered version in Workfront. </p><p>For example, if the name of a document in [!DNL Workfront] is <strong>Main Ad</strong>, and you add a new version to it in [!DNL Workfront], the new version is transferred to [!DNL Jira] as a new document with the name <strong>Main Ad_v2</strong>.</p><p>Important: <p>Consider the following when syncing documents:</p>
           <ul>
            <li><p>Documents larger than 5MB do not sync. If a document sync fails because the document is too large, an error is logged in the activity log. </p><p>For more information on the activity log, see <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">View the Jira Activity Log</a>.</p></li>
            <li><p>Documents that are linked to tasks and issues from external servers are not transferred to the [!DNL Jira] items. Only documents uploaded directly on the task or the issue in [!DNL Workfront] are transferred to the linked issue in [!DNL Jira].</p></li>
            <li><p>To create a proof from a document, you must generate the proof in [!DNL Workfront]. </p><p>For more information on generating a proof, see <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Create a proof for an existing document </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Create a proof for a document</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Planned Completion Date]</td>
         <td><p>The [!UICONTROL Planned Completion Date] of a task or an issue in [!DNL Workfront] becomes the [!UICONTROL Due Date] of the issue to which it is linked in [!DNL Jira].</p><p>Note: Ensure that you display <strong>[!UICONTROL Due Date]</strong> on [!DNL Jira] issues, for this value to synchronize.</p></td>
        </tr>
       </tbody>
      </table>

1. In the **[!UICONTROL Synchronize from [!DNL Jira] to [!DNL Workfront]]** section, select the fields that you want to update in [!DNL Workfront] when they are updated in [!DNL Jira]. 

   1. Select any of the following frequencies with which the fields are synchronized:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>The fields you specify are always synchronized between the linked [!DNL Workfront] and [!DNL Jira] items when the fields are updated in [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>The fields you specify are never synchronized between the linked [!DNL Workfront] and [!DNL Jira] items. There is no indication in [!DNL Workfront] that the field was updated in [!DNL Jira]. </p><p>Note: When you select Never, [!DNL Workfront] fields can still be manually updated from [!DNL Jira] in the left [!DNL Workfront] panel of the [!DNL Jira] issue. Those updates appear only on [!DNL Workfront] items in [!DNL Jira] and [!DNL Workfront] and not on [!DNL Jira] items.</p></td>
        </tr>
       </tbody>
      </table>

   1. Select to synchronize any of the following fields from [!DNL Jira] to [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>The [!UICONTROL Status] of an issue in [!DNL Jira] becomes the [!UICONTROL Status] of the task or issue to which it is linked in [!DNL Workfront].<br>For more information about [!DNL Workfront] statuses, see <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>The [!UICONTROL Assignee] of an issue in [!DNL Jira] becomes the [!UICONTROL Assignee] of the task or issue to which it is linked in [!DNL Workfront].</p><p>Important: When you assign an item in [!DNL Jira] to a user who does not have a [!DNL Workfront] account, the integration creates a new active user in [!DNL Workfront] only when <strong>Automatically create a user in [!DNL Workfront] if the [!DNL Jira] user does not have a [!DNL Workfront] account</strong> is set to <strong>[!UICONTROL Always]</strong>. This user does not occupy a [!DNL Workfront] license. Active users can be assigned to work items in [!DNL Workfront], but cannot be included in updates. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Attachments of an issue in [!DNL Jira] are also attached to the task or issue to which it is linked in [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>A comment on a [!DNL Jira] issue is also posted on the linked [!DNL Workfront] item in the [!UICONTROL Updates] area. Conversely, a comment posted in the [!UICONTROL Updates] area for a [!DNL Workfront] task or issue syncs to [!DNL Jira]'s native comment stream for the linked issue. </p><p>This is set to <strong>[!UICONTROL Always]</strong> by default. If you select <strong>[!UICONTROL Never]</strong> here, you can still post comments manually on a linked item either in [!DNL Workfront] or in [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. In the **[!UICONTROL OTHER]** section, select which additional fields should be updated between linked items. 

   1. Select an option to determine whether the fields you specify **[!UICONTROL Always]** or **[!UICONTROL Never]** update in [!DNL Jira] or [!DNL Workfront] when they are modified.

   1. Select from the following fields and updates:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Custom Data in the right panel in [!DNL Jira]]</td>
         <td><p>Displays the [!DNL Workfront] Custom Data of an item in the [!DNL Workfront] right panel.</p><p>Note:  Custom Form sections are displayed in the [!DNL Workfront] right panel with the access level of the [!DNL Workfront] System Administrator.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Priority in the right panel in [!DNL Jira]]</td>
         <td>Displays the [!DNL Workfront] Priority of an item in the [!DNL Workfront] right panel.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Add an update in the [!DNL Workfront] Updates tab about Due Date changes in [!DNL Jira]]</td>
         <td>Adds a comment in the [!UICONTROL Update] tab of the [!DNL Workfront] item when the [!UICONTROL Due Date] changes in linked [!DNL Jira] item.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Automatically create a user in [!DNL Workfront] if the [!DNL Jira] user does not have a [!DNL Workfront] account]</td>
         <td><p>The following scenarios exist:</p>
          <ul>
           <li>When you select <strong>[!UICONTROL Always]</strong>, you enable the integration to create a new Workfront user every time a [!DNL Jira] user without a [!DNL Workfront] account performs the following actions on a linked [!DNL Jira] issue:
            <ul>
             <li>Is assigned to a [!DNL Jira] issue</li>
             <li><p>Logs time to a [!DNL Jira] issue</p><p>This new user does not occupy a [!DNL Workfront] license. The default setting is Always. The user created this way in [!DNL Workfront] has "[!UICONTROL Jira]" added to their name.</p></li>
            </ul></li>
           <li>When you select <strong>[!UICONTROL Never]</strong>, the following things happen:
            <ul>
             <li>You are not able to see any [!DNL Jira] assignments on the [!DNL Workfront] items. In this case, only assignments made in [!DNL Workfront] display on the [!DNL Workfront] items.</li>
             <li>The time logged to a linked [!DNL Jira] issue by a user without a [!DNL Workfront] account does not automatically transfer to the linked [!DNL Workfront] item. You can still log time on the [!DNL Workfront] item in the right panel of the [!DNL Jira] issue.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Click **[!UICONTROL Save]**.

   Now, every time a user updates any of the fields specified in this configuration on an item in either [!DNL Jira] or [!DNL Workfront], the linked item in the other application is updated as well. 

## Troubleshooting

### Items cannot be created in [!DNL Jira] because of trigger fields marked "[!UICONTROL Couldn't be found]"

#### Problem

When an error occurs with the [!DNL Workfront for Jira] application, [!DNL Workfront] disables the triggers to prevent further complications. When those triggers are disabled, they display as "[!UICONTROL Couldn't be found]."

#### Solution

Locate the error that disabled the triggers. You can find the error in the [!DNL Workfront for Jira] [!UICONTROL Activity Log].

The most common cause of this behavior is the error "[!UICONTROL Field 'duedate' cannot be set. It is not on the appropriate screen, or unknown.]"

This error means that you are attempting to sync the "[!UICONTROL Planned Completion Date]" from [!DNL Workfront] to [!DNL Jira]. In order to do this, you must ensure that your [!DNL Jira] objects have a field called "[!UICONTROL Due Date]." If they do not have this field, [!DNL Workfront] is unable to sync the planned completion date from [!DNL Workfront] and disables your triggers.

To resolve this error, try one of the following:

* Ask your [!DNL Jira] administrator to update the affected [!DNL Jira] objects to ensure that they have a due date field.
* Disable the synchronization of [!DNL Workfront]'s planned completion date in the Workfront [!UICONTROL Setup] page.

-->
