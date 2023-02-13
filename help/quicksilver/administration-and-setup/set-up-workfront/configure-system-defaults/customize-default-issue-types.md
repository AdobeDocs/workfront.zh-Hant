---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 自訂預設問題類型
description: 您可以自訂每個預設問題類型的標籤，以更符合組織中使用的術語。 問題類型對於自訂問題狀態和建立請求佇列非常有用。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# 自訂預設問題類型

問題類型在下列情況中很實用：

* 自訂問題狀態時，如 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* 建立請求佇列時，如 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

您可以自訂每個預設問題類型的標籤，以更符合組織中使用的術語。

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

## 預設問題類型

若您有 [!DNL Adobe Workfront] [!UICONTROL 管理員] 存取，您可以設定並重新命名四種預設問題類型：

* **[!UICONTROL 錯誤報告]** 用於追蹤系統中報告的錯誤。
* **[!UICONTROL 變更順序]** 用於追蹤需要更新或修訂的問題。
* **[!UICONTROL 問題]** 中的物件 [!DNL Workfront] 傳達意外工作、出現的問題，或必須解決以便繼續執行任務的問題。
* **[!UICONTROL 要求]** 適用於使用者在Workfront中提出請求的請求佇列的問題類型。

![](assets/default-issue-types.png)

## 自訂問題類型

請考慮下列關於自訂問題類型的資訊：

* 您可以修改問題類型的標籤，但無法更改其函式。
* 您無法建立其他問題類型。
* 您無法更改問題類型名稱的篩選值。 因此，如果您在問題報表上建立篩選器，篩選器（索引鍵）的值不會反映問題類型的自訂名稱。
* 每個問題類型有三種預設狀態： [!UICONTROL 新增], [!UICONTROL 進行中]，和 [!UICONTROL 已關閉]. 您無法刪除這些狀態或從問題類型中刪除它們，但可以更名它們。
* 您可以針對每個問題類型重新排序下拉式功能表中顯示的選項。

若要自訂問題類型：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 專案偏好設定]** > **[!UICONTROL 狀態]**.

1. 按一下 **[!UICONTROL 問題]** 標籤。
1. 執行下列任一操作：

   * 將滑鼠指標暫留在您要自訂的問題類型上，按一下 [!UICONTROL 編輯] 圖示 ![](assets/edit-icon.png) 顯示在最右側，然後為問題類型鍵入新名稱。

      ![](assets/customize-issue-type.png)

   * 按一下 [!UICONTROL 問題類型] 若要列出其相關狀態，請拖曳控點，將游標暫留在控點上時顯示的控點，並依照您希望控制點在使用者問題中的顯示順序加以拖放 **[!UICONTROL 狀態]** 下拉式功能表。
