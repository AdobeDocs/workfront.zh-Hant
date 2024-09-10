---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 設定請求型別
description: 處理專案時，您可能會發現發生未預期的事件。 您可以將這些非預期事件記錄為特定專案或任務的問題。 您也可以提交請求，這些請求會記錄為指定為「請求佇列」專案上的問題。 在Adobe Workfront中，問題和請求被視為可互換。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# 設定請求型別

處理專案時，您可能會發現發生未預期的事件。 您可以將這些非預期事件記錄為特定專案或任務的問題。 您也可以提交請求，這些請求會記錄為指定為「請求佇列」專案上的問題。 在Adobe Workfront中，問題和請求被視為可互換。

如需在[!DNL Workfront]中建立問題的相關資訊，請參閱[建立問題](../../../manage-work/issues/manage-issues/create-issues.md)。 如需有關在[!DNL Workfront]中建立要求的資訊，請參閱[建立和提交 [!DNL Adobe Workfront] 要求](../../../manage-work/requests/create-requests/create-submit-requests.md)。 如需將請求型別與專案建立關聯的資訊，請參閱[定義專案的請求型別](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td><p>新增：[！UICONTROL Standard]</p>
   或
   <p>目前： [！UICONTROL計畫]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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

## 自訂請求型別的名稱

作為[!DNL Workfront]管理員，您可以在系統中設定要求型別的名稱。 新名稱會顯示在[!DNL Workfront]中任何顯示&#x200B;**[!UICONTROL 問題型別]**&#x200B;或&#x200B;**[!UICONTROL 請求型別]**&#x200B;欄位的區域中：

* 在將會接收問題或要求的專案的&#x200B;**[!UICONTROL 佇列詳細資料]**&#x200B;區域中。
* 若為「請求佇列」選取了多個請求型別，當您建立新問題或提交新請求時，請在&#x200B;**[!UICONTROL 問題型別]**&#x200B;欄位的&#x200B;**[!UICONTROL 新問題]表單**&#x200B;中。

  如需在[!DNL Workfront]中建立問題的詳細資訊，請參閱[建立問題](../../../manage-work/issues/manage-issues/create-issues.md)

  如需有關在[!DNL Workfront]中建立要求的詳細資訊，請參閱[建立和提交 [!DNL Adobe Workfront] 要求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

* 在&#x200B;**[!UICONTROL 佇列主題詳細資料]**&#x200B;表單上，設定佇列主題時。\
   如需建立佇列主題的詳細資訊，請參閱[建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

若要自訂請求型別的名稱：

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 專案偏好設定]** > **[!UICONTROL 狀態]**。

1. 按一下&#x200B;**[!UICONTROL 問題]**&#x200B;標籤。
1. 在&#x200B;**[!UICONTROL 問題]**&#x200B;索引標籤頂端，暫留在要求型別的名稱上，然後按一下出現的&#x200B;**[!UICONTROL 編輯]**&#x200B;圖示。

   ![](assets/edit-request-type-name-nwe.png)

1. 在出現的方塊中，輸入新名稱，然後按&#x200B;**[!UICONTROL Enter]**。

## 設定不同請求型別中的問題狀態

您可以將每個請求型別與不同的問題狀態建立關聯。 您也可以根據問題型別來變更狀態在問題上的顯示順序。

如需有關變更問題狀態的預設順序和設定問題狀態的詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)中的[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)區段。
