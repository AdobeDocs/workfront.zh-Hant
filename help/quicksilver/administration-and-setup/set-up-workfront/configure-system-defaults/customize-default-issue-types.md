---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 自訂預設問題型別
description: 您可以自訂每個預設問題型別的標籤，以更符合貴組織中使用的術語。 問題型別對於自訂問題狀態和建立請求佇列很有用。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 自訂預設問題型別

問題型別在下列情況下很有用：

* 自訂問題狀態時，如[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)中所述。
* 建立要求佇列時，如[建立要求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)中所述。

您可以自訂每個預設問題型別的標籤，以更符合貴組織中使用的術語。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[！UICONTROL標準]</p>
       <p>[！UICONTROL計畫]</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 預設問題型別

如果您有[!DNL Adobe Workfront] [!UICONTROL 管理員]存取權，您可以設定並重新命名四種預設問題型別：

* **[!UICONTROL 錯誤報告]**&#x200B;用於追蹤系統中報告的錯誤。
* **[!UICONTROL 變更順序]**&#x200B;用於追蹤需要更新或修訂的問題。
* **[!UICONTROL 問題]** [!DNL Workfront]中的物件，會傳達未計畫的工作、發生的問題或為了繼續工作而必須解決的事項。
* **[!UICONTROL 要求]**&#x200B;適用於使用者在Workfront中提出要求的要求佇列的問題型別。

![預設問題型別](assets/default-issue-types.png)

## 自訂問題型別

關於自訂問題型別，請考慮以下事項：

* 您可以修改問題型別的標籤，但無法變更其功能。
* 您無法建立其他問題型別。
* 您無法變更問題型別名稱的篩選值。 因此，如果您在問題報告上建立篩選器，篩選器（索引鍵）的值不會反映問題型別的自訂名稱。
* 每個問題型別有三種預設狀態： [!UICONTROL New]、[!UICONTROL In Progress]和[!UICONTROL Closed]。 您無法刪除這些狀態或從問題型別中移除它們，但您可以重新命名它們。
* 您可以重新排序出現在每個問題型別下拉式選單上的選項。

若要自訂問題型別：

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 專案偏好設定]** > **[!UICONTROL 狀態]**。

1. 按一下&#x200B;**[!UICONTROL 問題]**&#x200B;標籤。
1. 執行下列任一項作業：

   * 暫留在您要自訂的問題型別上，按一下最右側出現的[!UICONTROL 編輯]圖示![編輯圖示](assets/edit-icon.png)，然後為問題型別輸入新名稱。

     ![自訂問題型別](assets/customize-issue-type.png)

   * 按一下[!UICONTROL 問題型別]以列出其相關聯的狀態，然後拖曳將滑鼠游標停留在其中時出現的控制代碼，並依照您希望它們在使用者問題&#x200B;**[!UICONTROL 狀態]**&#x200B;下拉式功能表中出現的順序放置它們。
