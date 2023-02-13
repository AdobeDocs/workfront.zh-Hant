---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 刪除自訂表單上的物件類型
description: 在現有的自訂表單中，您可以刪除與表單相關聯的物件類型。 完成此操作後，用戶無法再將表單附加到該類型的對象。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 刪除自訂表單上的物件類型

在現有的自訂表單中，您可以刪除與表單相關聯的物件類型。 完成此操作後，用戶無法再將表單附加到該類型的對象。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 刪除自訂表單上的物件類型

您可以從現有的自訂表單中刪除物件類型。

自訂表單至少必須有一個物件類型。

>[!CAUTION]
>
>如果已將自定義表單附加到您要刪除的類型的對象中，並將資料添加到該對象中，則在您刪除表單上的該對象類型時，該資料將被永久刪除。 其中可能包含使用者日後需要的歷史資訊。
>
>一般而言，建議您將編輯已使用中自訂表單的次數減到最少。 沒有通知系統可提醒使用自訂表單的使用者您所做的變更。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms** 中。
1. 選取您要編輯的自訂表單，然後按一下 **編輯**.
1. 按一下 **物件類型** 從表單中刪除，然後按一下 **刪除** 顯示的警告訊息。

   ![](assets/click-x-object-types.jpg)

1. （可選）對要從表單中刪除的任何其他對象類型重複上一步。
1. 按一下 **完成**，然後按一下 **關閉並儲存**.
