---
title: 停用或重新啟用自訂表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以重新啟用或停用自訂表單。 建議您停用自訂表單，而非刪除您不再用於保留歷史資料的表單。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: c0082dd73e3db8123f9cc08f1798ef8e70730625
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# 停用或重新啟用自訂表單

您可以重新啟用或停用自訂表單。 建議您停用自訂表單，而非刪除您不再用於保留歷史資料的表單。

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
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 停用自訂表單

您可以停用不再使用的自訂表單，同時不會遺失其相關聯的歷史資料。 用戶無法向對象添加非活動的自定義表單，但仍然可以查看資料並將其添加到已附加對象的欄位。

非使用中自訂表單上的欄位仍可用於檢視中的內嵌編輯。 如果使用者在內嵌編輯期間從非作用中自訂表單新增欄位，表單會自動附加至物件，即使自訂表單已停用亦然。

停用自訂表單：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).
1. 在左側面板中，選擇 **自訂Forms**.
1. 在 **Forms** 頁簽，選擇要停用的自定義表單。
1. 在「活動」列中，選擇 **False** 然後按一下欄外。 表單不再作用中。

## 重新啟用自訂表單

如果您重新啟用自訂表單，表單會保留先前的設定，使用者可以像從未停用一樣與表單互動。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).
1. 在左側面板中，選擇 **自訂Forms**.
1. 在 **Forms** 頁簽，選擇要重新激活的自定義表單。
1. 在「活動」列中，選擇 **True** 然後按一下欄外。 表單現在已啟用。