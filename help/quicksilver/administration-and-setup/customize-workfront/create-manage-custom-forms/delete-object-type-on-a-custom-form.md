---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 刪除自訂表單上的物件型別
description: 您可以在現有的自訂表單上刪除與表單相關聯的物件型別。 執行此操作後，使用者無法再將表單附加到該型別的物件。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 刪除自訂表單上的物件型別

您可以在現有的自訂表單上刪除與表單相關聯的物件型別。 執行此操作後，使用者無法再將表單附加到該型別的物件。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>管理自訂表單的存取權</p> <p>如需Workfront管理員如何授予此存取許可權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取層級設定，請聯絡Workfront管理員。

## 刪除自訂表單上的物件型別

您可以從現有的自訂表單中刪除物件型別。

自訂表單必須至少有一個物件型別。

>[!CAUTION]
>
>如果人員已將自訂表單附加到您要刪除的物件型別並新增資料，當您刪除表單上的該物件型別時，該資料將會永久刪除。 其中可能包含使用者稍後所需的歷史資訊。
>
>一般而言，建議您儘可能減少編輯已使用中的自訂表單的次數。 沒有通知系統可提醒使用自訂表單的人員您的變更。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms** 在左側面板中。
1. 選取您要編輯的自訂表單，然後按一下 **編輯**.
1. 按一下任何頁面上的X **物件型別** ，然後按一下「 」 **刪除** 在顯示的警告訊息上。

   ![](assets/click-x-object-types.jpg)

1. （可選）針對您要從表單中移除的任何其他物件型別，重複上一步驟。
1. 按一下 **完成**，然後按一下 **關閉並儲存**.
