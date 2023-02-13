---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 設定請求類型
description: 處理專案時，您可能會發現發生非預期的事件。 您可以將這些意外事件記錄為特定專案或任務的問題。 您也可以提交請求，這些請求記錄為指定為「請求佇列」之專案上的問題。 在Adobe Workfront中，問題和請求可視為可互換。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 設定請求類型

處理專案時，您可能會發現發生非預期的事件。 您可以將這些意外事件記錄為特定專案或任務的問題。 您也可以提交請求，這些請求記錄為指定為「請求佇列」之專案上的問題。 在Adobe Workfront中，問題和請求可視為可互換。

如需在 [!DNL Workfront]，請參閱 [建立問題](../../../manage-work/issues/manage-issues/create-issues.md). 如需在中建立請求的相關資訊，請參閱 [!DNL Workfront]，請參閱 [建立和提交 [!DNL Adobe Workfront] 請求](../../../manage-work/requests/create-requests/create-submit-requests.md). 如需有關將請求類型與專案關聯的資訊，請參閱 [定義專案的請求類型](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## 自訂請求類型的名稱

As a [!DNL Workfront] 管理員，您可以在系統中設定請求類型的名稱。 新名稱會顯示在 [!DNL Workfront] 其中 **[!UICONTROL 問題類型]** 或 **[!UICONTROL 請求類型]** 欄位顯示：

* 在 **[!UICONTROL 隊列詳細資訊]** 接收問題或請求的專案區域。
* 若為「請求佇列」選取了多個請求類型，請在 **[!UICONTROL 新問題] 表單** 在 **[!UICONTROL 問題類型]** 欄位，在您建立新期刊或提交新請求時。

   如需在 [!DNL Workfront]，請參閱  [建立問題](../../../manage-work/issues/manage-issues/create-issues.md)

   如需在 [!DNL Workfront]，請參閱  [建立和提交 [!DNL Adobe Workfront] 請求](../../../manage-work/requests/create-requests/create-submit-requests.md).

* 在 **[!UICONTROL 隊列主題詳細資訊]** 表單中的「隊列主題」。\
   如需建立佇列主題的詳細資訊，請參閱 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

若要自訂請求類型的名稱：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 專案偏好設定]** > **[!UICONTROL 狀態]**.

1. 按一下 **[!UICONTROL 問題]** 標籤。
1. 在 **[!UICONTROL 問題]** 標籤中，將滑鼠指標暫留在請求類型的名稱上，然後按一下 **[!UICONTROL 編輯]** 表徵圖。

   ![](assets/edit-request-type-name-nwe.png)

1. 在出現的方塊中，輸入新名稱，然後按 **[!UICONTROL 輸入]**.

## 在不同請求類型中設定問題狀態

您可以將每個請求類型與不同的問題狀態關聯。 您也可以根據問題的類型，變更問題上狀態顯示的順序。

有關更改問題狀態的預設順序和配置問題狀態的詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) 區段 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
