---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 刪除或停用自訂表單
description: 您可以從系統中刪除或停用自訂表單。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 刪除或停用自訂表單

您可以從系統中刪除或停用自訂表單。

>[!CAUTION]
>
>刪除自訂表單也會刪除與表單關聯之物件上的所有自訂資料。 已刪除的資料無法恢復。 請考慮停用自訂表單 — 停用您不再使用的自訂表單時，您會保留所有相關的歷史資料。

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

## 刪除自訂表單

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms。**
1. 選取自訂表單，然後按一下 **刪除**.
1. 如果您確定要永久刪除自定義表單及其附加對象上的所有關聯資料，請按一下 **是，刪除它**.

## 停用自訂表單

您可以停用不再使用的自訂表單，同時不會遺失其相關聯的歷史資料。 用戶無法向對象添加非活動的自定義表單，但仍然可以查看資料並將其添加到已附加對象的欄位。

非使用中自訂表單上的欄位仍可用於檢視中的內嵌編輯。 如果使用者在內嵌編輯期間從非作用中自訂表單新增欄位，表單會自動附加至物件，即使自訂表單已停用亦然。

如果您重新啟用自訂表單，表單會保留先前的設定，且使用者可以像從未停用一樣與表單互動。

停用自訂表單：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下您要停用的自訂表單名稱。
1. 按一下 **表單設定** 標籤。
1. 停用 **活動** 選項。
1. 按一下 **儲存+關閉**.
