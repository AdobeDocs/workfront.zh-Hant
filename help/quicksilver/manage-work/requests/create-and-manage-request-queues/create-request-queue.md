---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立請求佇列
description: 您可以設定請求佇列，讓使用者可輸入專案上未計畫工作的臨時請求。 例如，服務檯請求佇列可設定為擷取所有來到IT部門的使用者請求。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: 6311526ddf9143c4a979d8bbac96312a3b0e8151
workflow-type: tm+mt
source-wordcount: '2855'
ht-degree: 2%

---


# 建立請求佇列

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

<!--hide/ comment out the entire "create requests in Production" section and just edit and leave  only the preview section when it releases to Production; also remove the template blurb when the queue details is unshimmed for templates-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


您可以設定請求佇列，讓使用者可輸入專案上未計畫工作的臨時請求。 例如，服務檯請求佇列可設定為擷取所有來到IT部門的使用者請求。

請求成為Adobe Workfront中的問題，並會新增至專案。

設定請求佇列可協助將新增至專案之問題的相關資訊正規化。 所有提交至專案的問題都將以相同方式提交，並遵循相同路徑完成。

您可以在Workfront中將下列物件設定為請求佇列：

* 專案
* 範本。 從設定為請求佇列的範本建立的專案將變成請求佇列。

若要將專案或範本設定為請求佇列，您必須編輯專案或範本的佇列詳細資訊區域。

本文說明如何將專案設定為請求佇列，讓使用者可以在其中提交請求。 為範本設定佇列詳細資訊類似於在專案上設定它們。

如需有關如何提交新請求至請求佇列的資訊，請參閱[複製並提交請求](../create-requests/copy-and-submit-requests.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>新授權： Standard </p>
   或
   <p>目前授權：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p> 管理專案的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 請求佇列總覽

您可以將請求佇列設定為專案。 將專案指定為請求佇列時，可從Adobe Workfront的請求區域存取佇列。 自訂「請求佇列」時，也會自訂使用者提交請求時填寫的表單。

本文會說明如何從現有專案建立請求佇列。 不過，若要為請求擷取流程建立一致性，或為其中新增多個層級以用於報告和更好的管理，您也可以設定請求佇列的其他建置區塊，如下表所述。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">佇列詳細資訊</td> 
   <td> <p>您必須在「佇列詳細資訊」區域將專案設定為請求佇列。 此步驟為必要步驟。 </p> <p>如需詳細資訊，請參閱本文中的<a href="#create-a-request-queue" class="MCXref xref">建立請求佇列</a>一節。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">主題群組</td> 
   <td> <p>它們是額外的選單，可依據常見功能來分類請求。 例如，對於IT要求佇列，您可能想要有「現場」和「遠端」主題群組。 </p> <p>如需詳細資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">建立主題群組</a>。 </p> <p>這是選擇性的。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">佇列主題</td> 
   <td> <p>它們是額外的功能表，可根據常見功能將屬於相同主題群組的請求分類。 一個主題群組可以包含數個佇列主題。 </p> <p>例如，IT要求佇列的「現場」主題群組可能包含「硬體」、「軟體」和「網路」佇列主題。 </p> <p>如需詳細資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">建立佇列主題</a>。 </p> <p>這是選擇性的。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">路由規則</td> 
   <td> <p>它們可讓您將每個請求路由至使用者、工作角色、團隊或專案。 </p> <p>如需詳細資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">建立路由規則</a>。 </p> <p>這是選擇性的。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立請求佇列

<!--at production release on April 10, do the following: take the first sentence here out; hide/ comment out the first section (Create a Request Queue in the Production environment); remove the title of the "Create a Request Queue in the Preview environment and leave that section as the only way to create request queues; search for any visible references of production/ preview and remove them from the entire article-->

建立請求佇列會依您使用的環境而有所不同。

<!--

### Create a Request Queue in the Production environment

This section describes how you can define Queue Details for the following objects:

* A project in the Production environment
* A template in the Production or Preview environment

When you set up a project as a Request Queue, the project status must be Current in order to display in the Requests area of Workfront.

>[!TIP]
>
>Your Workfront or group administrator might assign you to a custom Layout Template that might not include some of the sections described in the following steps.


To create a Request Queue:

1. Go to the project that you want to set up as a Request Queue.
1. (Optional) Click **Project Details** in the left panel and add a **Description** to the project in the **Overview** area. This information displays on all new requests.
1. Click **Queue Details** in the left panel. You might need to click **Show More**, then **Queue Details**.

   This opens the Queue Details section.

   ![Queue Details top of the section](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)   

1. Specify the following information:

   * **Publish as Help Request Queue:** Select this option to identify this project as a request queue. All incoming issues are considered Requests.  
     When this option is not selected, the project behaves like a standard project in Workfront and all incoming issues are issues.
   
   * **Who can add requests to this queue:** Select which users have access to add requests to this queue. You can allow the following groups of people to see the Request Queue in their Requests area of the Global Navigation Bar when they add a new request:

     |Who can enter requests | Description|
     |---|---|
     | Anyone  |Any Workfront user with an active account can view this request queue and add requests to it |
     | People with view access to this project |Users with View permissions to the project can view and add requests to this queue |
     | People in this project's company |Users who belong to the company associated with this project can view and add requests to this queue. If there is a company associated with the project, the name of the company is listed in parentheses after this setting.  |
     | People in this project's group |Users who belong to the group associated with this project can view and add requests to this queue. If there is a group associated with the project, the name of the group is listed in parentheses after this setting, in gray font.  |

   * **Share with these links:** The following options enable you to provide direct access to the Request Queue and the forms associated with it to users outside of Workfront or to Workfront users using an external page. For information about embedding a request queue in a dashboard as an external page, see [Embed a request queue in a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Users must already have access rights to the Request Queue in order to gain direct access. Using either option described here does not automatically grant access to users.

     >[!TIP]
     >
     >Users must first log in to Workfront before gaining access to the request queue when they access the Request Queue page from another application.

      * **Direct Access URL:** When a user accesses this URL from a browser, the user is taken directly to the New Request  section in the Requests area and this request is selected by default for them.

        ![Share request queue with direct URL embedded in dashboard](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >You can display a Request Queue in a dashboard as an external page. In this case, the request queue is preselected, but you can select any other request queue from the Request Type field. users can change the Request Type. Navigation components of the Requests also display.

      * **Embed Code:** Use this HTML code to embed the request queue form as an iframe within any HTML page.  
        If users are not already authenticated to Workfront when they view the page where the code is embedded, the Workfront login dialog box is displayed. After users log in, the Request Queue form is displayed.

        >[!NOTE]
        >
        >When displaying a Request Queue in an iframe, only the request form displays, the request name is preselected and dimmed. User cannot change the Request type. Navigation components of the Requests area do not display.

        In order for the request queue form to be displayed when using this embed code, you must enable the "Allow embedding of Workfront in an iframe" setting in your system setup. For more information about enabling embedding of Workfront in an iframe, see [Configure system security preferences](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). If this setting is not enabled, the iframe is displayed as blank.

        You can adjust various aspects of how the embedded form is displayed, as follows:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Functionality</strong> </p> </th> 
           <th> <p><strong>Solution</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Adjust the size of the frame</p> </td> 
           <td> <p>Modify the "width" and "height" attributes.</p> <p>By default, the width is "500" and the height is "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direct users to a specific Queue Topic or Topic Group</p> </td> 
           <td> <p>Add the "path" parameter to the src URL. You can find the path parameter by navigating to the desired Queue Topic or Topic Group in the non-embedded form and inspecting the URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Show and allow users to change the pre-configured Topic Group drop-down list</p> </td> 
           <td> <p>Use the "path" parameter by adding the <code>showPreSelectedOptions=true</code> parameter to the <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detect when the form has been submitted</p> </td> 
           <td> <p>Add a "message" event listener to your web page's window and checking if <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> will be set to the ID of the created issue.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Request Types:** Select from the default options below.

     The Workfront administrator can rename the default request types. For more information about renaming the request types, see [Customize default issue types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Bug Report
      * Change Order
      * Issue
      * Request

        This is a required field and you must select at least one option.

     >[!NOTE]
     >
     >Request Types display as a selection in the Requests area only if the Request Type is selected in both the Queue Details and the Queue Topic pages. For information about setting up the Queue Details area of a project, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Each type selected here will be available on the form (you can select more than one). Selecting more than one type can help organize multiple requests coming in.  
     For example, if you are using the form on a request queue for an IT project, the following request types can come in to the queue: hardware, software, bug fixes, and issues.

   * **Default Duration:** The default duration is the length of time it typically takes to complete an issue. This becomes the default for all incoming issues and can be modified manually. Duration is generally set in hours, days, or weeks. The Default Duration of an issue is the same as the Planned Hours on the issue. The Planned Completion Date of the issue calculates based on this field.  
     The default for the issue Duration is 1 day or 8 hours. If your Workfront administrator set the Typical Hours per Work Day as less than 8 hours, the Default Duration for issues is still 8 hours. For example, if the Typical Hours per Work Day is set to 7 hours, the Default Duration for issues is 1.14 Days or 8 hours. For more information about how to set up the system Typical Hours per Work Day, see the "Timeline Calculations" section in the article [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
   
   * **People from the same company will inherit the same permissions for all requests.:** When selected, all requests submitted to the queue are visible for users in the same company. Users can view these requests in the All Requests  section , located within the Requests area. At the time that this setting is enabled or disabled, it impacts all future requests; it does not retroactively impact information. 
   * **When someone makes a request, automatically grant:** When a user makes a request to the request queue, the user is automatically granted the level of permission that you choose to that request. Select from the following permissions levels: 

      * **View Access** 
      * **Contribute Access**. This is the default selection.
      * **Manage Access**

     For information about the Workfront permissions model, see [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).   
     Setting permissions here saves time, rather than having to grant permissions for each individual incoming request. Choosing this option impacts all future requests, but does not retroactively impact existing requests. 
   
   * **Default Approval**: Associate an approval process with this request queue. Only Issue Approval Processes are visible in this drop-down menu. All issues submitted to this queue will be associated with this approval process. Your Workfront administrator must define system-level approval processes before you can associate them with request queues. Users with administrative access to Approval processes can also create group-specific approval processes.

     >[!IMPORTANT]
     >
     >If the group of the project changes, the group-specific approval process attached to existing issues becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see [How group and approval process changes affect assigned approval processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     If you have multiple queue topics associated with a request queue, we recommend that you associate approval processes with the queue topics instead. For more information about creating queue topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md). 
   
     Consider the following when adding approval processes to request queues:

      * Only active approval processes display in the list. 
      * System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.

   * **Default Route**: Associate a Routing Rule with this request queue. Use Routing Rules to automatically assign new issues submitted to a Request Queue to the correct resource (user, job role, or team), and to the correct project. All issues submitted to this queue will be associated with this Routing Rule. You must configure Routing Rules before they display in the Queue Details section and before you can associate them with request queue.  
     If you have multiple queue topics associated with a request queue, we recommend that you associate routing rules with the queue topics instead. For more information about creating routing rules, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
   
   * **New Issue Fields:** In the **Show the following selected fields to all users** section, select any fields that you want to be visible to all users who submit a request to the project or add an issue to the project or the tasks.

     >[!TIP]
     >
     >New Issue Fields selected in the Queue Details section are also associated with any new issue added to the project <!--this is confusing: or to the tasks in the Issues section-->.

<!--     When you enable any of the Assigned to, Job Role, or the Team fields, they are always renamed to Assignments in the request form, but you can only specify the type of assignment selected here.

      >[!NOTE]
      >
      >If you selected Assigned To in the Queue Details area, you can enter only users in the Assignments field on the request form. In this case, you cannot enter job roles or a team. 
   
   * **Documents**: If you select to display the Documents section in the new request form, select where the document uploading section should be positioned. Select from the following:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">After custom forms</td> 
        <td><span>The Documents section displays at the bottom of the request form.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Before custom forms</td> 
        <td> <p><span>The Documents section displays between the Workfront fields and the custom fields of the request form.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>   
   
     ![New issue fields area with documents](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Show all selected and unselected fields to:** Select which users you want to see all the fields on the new request form. The following options control the access to the fields on the form.
    
      |Which users can see all fields on the request form | Description|  
      |---|---| 
      | All Users (Plan Licenses) |All users who have a Plan license can see the selected as well as the unselected fields. |
      | People with view access to this project (Plan License) |Those users with a Plan license that also have View rights to this project can see the selected as well as the unselected fields. The rest of the users who can submit requests to this project can see just the selected fields. |
      | No Users |No users can see the unselected fields. All users who can submit requests to this project can only see the fields selected.  |
  
   * **Custom Forms**: Select a custom form to associate with the Request Queue. Only Issue Custom Forms are available to select from this drop-down menu. All issues submitted to the Request Queue will have the selected forms associated with them. You must create issue custom forms before you can see them displayed in the Queue Details section. 
     If you have multiple Queue Topics associated with a Request Queue, we recommend that you associate custom forms with the Queue Topics instead. For more information about creating sub-sections for the Request Queue, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Custom forms on Queue Details](assets/custom-forms-on-queue-details.png)

     If you have multiple custom forms associated with the Request Queue, drag and drop the forms to sort them in the desired order, in the **Reorder Forms** section.

     >[!TIP]
     >
     >Custom forms added to the Queue Details section are also associated with any new issue added to the project <!--this is confusiong: or the tasks in the Issues  section-->.

<!--1. Continue selecting information for the settings in the **Email Queue Settings** area, to allow users to email requests to the request queue project. 

    For more information, see [Enable users to email an issue into a Request Queue project](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Click **Save**.  
   Your project has now been configured to be a Request Queue and users can now add requests to it. 

1. (Optional) To enhance the Request Queue functionality, build additional sub-sections for your queue, as well as rules to route the incoming requests to the correct team, assignee or project.

   * For information about creating sub-sections for the Request Queue, see the articles [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) and [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).  
   * For information about routing the requests to the appropriate assignee, team, and appropriate project, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   -->


### 建立請求佇列

將專案設定為請求佇列時，專案狀態必須為目前才能顯示在Workfront的請求區域中。

>[!TIP]
>
>您的Workfront或群組管理員可能會將您指派給自訂配置範本，該範本可能不包括下列步驟中說明的某些區段。

若要建立「請求佇列」：

1. 前往您要設定為「請求佇列」的專案。
1. （選擇性）按一下左側面板中的「**專案詳細資料**」，然後將「**描述**」新增至「**概觀**」區域中的專案。 此資訊會顯示在所有新請求上。
1. 按一下左側面板中的&#x200B;**佇列詳細資料**。 您可能需要按一下&#x200B;**顯示更多**，然後按一下&#x200B;**佇列詳細資料**。

   這會開啟佇列詳細資訊區段。

   佇列詳細資料區域中的![佇列型別區段](assets/unshimmed-queue-type-section-queue-details-area.png)

1. 指定下列資訊：

   * **以說明要求佇列發佈**：選取此選項可將此專案識別為要求佇列。 所有傳入問題都視為請求。\
     若未選取此選項，專案的運作方式會類似Workfront中的標準專案，而所有傳入的問題都會是問題。

   * **誰可以新增要求至此佇列？**：選取哪些使用者有權將要求新增至此佇列。 您可以允許下列群組的人在新增新請求時，於全域導覽列的「請求」區域中看到「請求佇列」：

     | 誰可以輸入請求 | 說明 |
     |---|---|
     | 任何人 | 任何擁有有效帳戶的Workfront使用者都可以檢視此請求佇列並新增請求 |
     | 擁有此專案檢視權限的人員 | 擁有專案檢視許可權的使用者可以檢視及新增請求至此佇列 |
     | 專案公司中的人員 | 屬於與此專案相關聯之公司的使用者可以檢視請求並將其新增至此佇列。 如果專案有關聯的公司，則在此設定後方括弧內會列出公司名稱。 |
     | 此專案群組中的人員 | 屬於與此專案相關聯的群組的使用者可以檢視請求並將其新增到此佇列。 如果有與專案相關聯的群組，則該群組的名稱會以灰色字型列在此設定之後的括弧中。 |

     {style="table-layout:auto"}

   * 使用下列選項，讓Workfront外部的使用者或使用內嵌外部頁面的Workfront使用者直接存取請求佇列及與其關聯的表單。

   如需將請求佇列內嵌到儀表板做為外部頁面的詳細資訊，請參閱[將請求佇列內嵌到儀表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md)。

   使用者必須先擁有請求佇列的許可權，才能直接存取許可權。 使用此處說明的任一選項都不會自動授予使用者存取權。

   >[!TIP]
   >
   >使用者從其他應用程式存取「請求佇列」頁面時，必須先登入Workfront，才能存取請求佇列。

   * **直接存取URL：**&#x200B;當使用者從瀏覽器存取此URL時，會直接將使用者帶到[要求]區域的[新增要求]區段，而且預設會為其選取此要求。

     ![來自直接URL共用的新要求方塊](assets/new-request-box-from-direct-url-share.png)

     >[!NOTE]
     >
     >您可以在控制面板中將「請求佇列」顯示為外部頁面。 在此情況下，會預先選取請求佇列，但您可以從「請求型別」欄位中選取任何其他請求佇列。 提交請求的使用者可以選取其他請求型別。 主題群組和佇列主題也會顯示。

   * **內嵌程式碼：**&#x200B;使用此HTML程式碼將請求佇清單單內嵌為任何HTML頁面中的iframe。\
     如果使用者在檢視內嵌程式碼所在的頁面時，尚未通過Workfront驗證，則會顯示「Workfront登入」對話方塊。 使用者登入後，畫面會顯示「請求佇列」表單。

     >[!NOTE]
     >
     >在iframe中顯示「請求佇列」時，只會顯示請求表單，請求名稱會預先選取並變暗。 使用者無法變更請求型別。 請求區域的導覽元件不顯示。

     為了在使用此內嵌程式碼時顯示請求佇清單單，您的Workfront管理員必須在系統設定區域中啟用「允許在iframe中內嵌Workfront」設定。

     如需在iframe中啟用Workfront內嵌的詳細資訊，請參閱[設定系統安全性偏好設定](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)。 如果未啟用此設定，iframe會顯示為空白。

     您可以調整內嵌表單顯示方式的各個方面，如下所示：

     <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>功能</strong> </p> </th> 
           <th> <p><strong>解決方案</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>調整框架大小</p> </td> 
           <td> <p>修改「寬度」和「高度」屬性。</p> <p>依預設，寬度是"500"，高度是"600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>將使用者導向至特定佇列主題或主題群組</p> </td> 
           <td> <p>將「path」引數新增至src URL。 您可以導覽至非內嵌表單中所需的佇列主題或主題群組，並檢查URL來尋找path引數。</p> </td> 
          </tr> 
          <tr> 
           <td> <p>顯示並允許使用者變更預先設定的主題群組下拉式清單</p> </td> 
           <td> <p>將<code>showPreSelectedOptions=true</code>引數新增至<code>src URL</code>以使用「path」引數。</p> </td> 
          </tr> 
          <tr> 
           <td> <p>偵測表單何時已提交</p> </td> 
           <td> <p>將「訊息」事件接聽程式新增至網頁的視窗，並檢查<code>event.data.type</code>是否為<code>requestSubmitted</code>。 <code>event.data.newIssueID</code>將設定為已建立問題的識別碼。</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **要求型別：**&#x200B;在&#x200B;**佇列屬性**&#x200B;區段中，從下列選項中選取：

   * 錯誤報告
   * 變更順序
   * 問題
   * 請求

   這是必填欄位，您必須至少選取一個選項。

   Workfront管理員可重新命名預設請求型別。 如需重新命名要求型別的詳細資訊，請參閱[自訂預設問題型別](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md)。

   >[!NOTE]
   >
   >使用者從「請求」區域存取請求佇列時，只有在「佇列詳細資訊」和「佇列主題」頁面中同時選取「請求型別」時，「請求型別」才會顯示為選取專案。
   >
   >如需有關設定專案佇列主題區域的資訊，請參閱[建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

   此處選取的每個型別都可在表單上使用（您可以選取多個型別）。 選取多個型別有助於組織傳入的多個請求。\
   例如，如果您在IT專案的請求佇列上使用表單，佇列中可能會有下列請求型別：硬體、軟體、錯誤修正和問題。

   * **預設期間：**&#x200B;輸入期間的數字，然後從下拉式功能表中選取下列其中一個期間單位：

      * 天
      * 時數
      * 分鐘
      * 週

   預設期間是完成提交至此請求佇列的問題通常所需的時間。 這會成為所有傳入問題的預設值，並可手動修改。
問題的預設期間與問題的計畫時數相同。 問題的計畫完成日期會根據此欄位來計算。\
   若維持不變，問題「持續時間」的預設為1天或8小時。
如果您的Workfront管理員在「設定」區域中將「每工作日一般時數」設定為少於8小時，則問題的預設期間仍為8小時。
例如，如果在Workfront的「設定」區域中將「每工作日一般時數」設定為7小時，則問題的預設期間為1.14天或8小時。
如需有關如何設定系統「每個工作日一般時數」的詳細資訊，請參閱[設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)一文中的「時間表計算」一節。

   * **來自相同公司的人員將會為所有要求繼承相同的許可權。**：選取時，所有提交至佇列的請求對同一公司的使用者可見。 使用者可以在所有請求區段（位於請求區域）中檢視這些請求。 啟用或停用此設定時，將會影響所有未來的請求；而不會回溯影響資訊。
   * **當有人提出要求時，自動授予……：**&#x200B;當使用者對要求佇列提出要求時，會自動授予使用者您選擇該要求的許可權等級。 按一下「存取」按鈕，從下列許可權層級選取：

      * **檢視存取權**
      * **貢獻存取權**。 這是預設選取專案和「存取」按鈕的名稱。
      * **管理存取權**

     如需Workfront許可權模型的相關資訊，請參閱[物件許可權共用簡介](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。\
     在此設定許可權可節省時間，而不必針對每個傳入請求個別授予許可權。 選擇此選項會影響所有未來的請求，但不會影響現有請求。

   * **預設核准**：按一下下拉式功能表，以選取此請求佇列的核准流程。 此下拉式選單中只會顯示問題核准流程。 提交至此佇列的所有問題都將與此核准流程相關聯。 您的Workfront管理員必須定義系統層級的核准流程，您才能將其與請求佇列相關聯。 擁有核准流程管理存取權的使用者也可以建立群組特定的核准流程。

     >[!IMPORTANT]
     >
     >如果專案的群組變更，則附加至現有問題的群組特定核准流程會變成單一使用核准流程。 如需關於專案群組的變更或核准程式變更如何影響核准設定的詳細資訊，請參閱[群組和核准程式變更如何影響指派的核准程式](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md)。

     如果您有多個與請求佇列相關聯的佇列主題，建議您改為將核准流程與佇列主題相關聯。

     如需建立佇列主題的詳細資訊，請參閱[建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

     將核准流程新增至請求佇列時，請考量下列事項：

      * 清單中僅顯示有效問題核准流程。
      * 系統範圍及群組專屬問題核准流程會顯示在清單中。 與專案群組以外的群組相關聯的核准程式不會顯示在清單中。

   * **預設路由**：按一下下拉式功能表，為此請求佇列選取路由規則。 路由規則會自動將提交至請求佇列的新問題指派給正確的資源（使用者、工作角色或團隊），並指派給正確的專案。 提交至此佇列的所有問題都將與此路由規則相關聯。 您必須先設定「路由規則」，才能將其顯示在「佇列詳細資訊」區段中，以及將其與請求佇列產生關聯。\
     如果您有多個與請求佇列相關聯的佇列主題，建議您改為將路由規則與佇列主題相關聯。 如需有關建立路由規則的詳細資訊，請參閱[建立路由規則](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)。

   * **新問題欄位：**&#x200B;在&#x200B;**向所有使用者顯示以下選取的欄位**&#x200B;區段中，選取您希望向專案提交請求或向此專案或專案任務新增問題的所有使用者都可見的欄位。

     >[!NOTE]
     >
     >* 當您啟用任何「指派至」、「工作角色」或「團隊」欄位時，當使用者提交請求時，這些欄位一律會在請求表單中重新命名為「指派」。 您只能在佇列詳細資訊區域中指定指派型別。
     >
     >* 如果您在「佇列詳細資料」區域選取了「指定給」，則只能在請求表單的「工作總攬」欄位中輸入使用者。 在這種情況下，您無法輸入職位角色或團隊。

   * **檔案**：選取此選項以在新的請求表單中顯示[檔案]區段，然後選取檔案上傳區段應該放置的位置。 從下列選項中選取：

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">在自訂表單之後</td> 
        <td><span>檔案區段會顯示在要求表單的底部。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">在自訂表單之前</td> 
        <td> <p><span>檔案區段會顯示在Workfront欄位與請求表單的自訂欄位之間。</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![佇列詳細資料中的新問題欄位和檔案](assets/new-issue-fields-and-documents-on-queue-details.png)

   * **將所有選取和未選取的欄位顯示給：**&#x200B;選取哪些使用者應該看到新要求表單上的所有欄位。 以下選項可控制對表單上欄位的存取。

     | 哪些使用者可以檢視請求表單上的所有欄位 | 說明 |
     |---|---| 
     | 所有使用者（計畫授權） | 所有擁有Plan授權的使用者都可以看到所選以及未選取的欄位。 |
     | 擁有此專案檢視存取權限的人員（計劃授權） | 擁有計畫授權且擁有此專案檢視許可權的使用者可以檢視所選及未所選欄位。 其他可以提交請求至此專案的使用者只能看到選取的欄位。 |
     | 無使用者 | 沒有使用者可以看到未選取的欄位。 所有可以提交請求至此專案的使用者只能看到選取的欄位。 這是預設選取範圍。 |

   * **自訂Forms**：從下拉式功能表中選取要與請求佇列關聯的自訂表單。 您可以選取多個表單，然後以您想要它們在請求表單中顯示的順序拖放它們。
只有問題自訂表單可從此下拉式選單中選取。 提交至此請求佇列、新增至專案或其任務的所有問題，都會有與其關聯的選定表單。
您必須先建立問題自訂表單，才能看到它們顯示在佇列詳細資料區段中。
如果您有多個與請求佇列相關的佇列主題，建議您改將自訂表單與佇列主題相關聯。
如需詳細資訊，請參閱[建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

     佇列詳細資料上的![自訂表單方塊](assets/custom-forms-box-on-queue-details.png)

1. 繼續選取&#x200B;**電子郵件佇列設定**&#x200B;區域中設定的資訊，以允許使用者透過電子郵件將要求傳送到要求佇列專案。

   如需詳細資訊，請參閱[讓使用者透過電子郵件將問題傳送到請求佇列專案](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md)。

1. 按一下「**儲存**」。\
   您的專案現在已設定為請求佇列，使用者現在可以在其中新增請求。

1. （可選）若要增強「請求佇列」功能，請為您的佇列建立其他子區段，以及將傳入的請求路由到正確團隊、受指派人或專案的規則。

   * 如需有關為「請求佇列」建立子區段的資訊，請參閱下列文章
   * [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)
   * [建立主題群組](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)。

     如需將請求路由傳送給適當的受指派人、小組和適當的專案的資訊，請參閱[建立路由規則](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)。

