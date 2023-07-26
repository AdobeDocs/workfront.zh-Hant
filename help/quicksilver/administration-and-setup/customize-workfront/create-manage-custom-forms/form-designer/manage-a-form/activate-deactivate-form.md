---
title: 停用或重新啟用自訂表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以重新啟用或停用自訂表單。 建議您停用自訂表單，不要刪除您不再用來保留歷史資料的表單。
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# 停用或重新啟用自訂表單

您可以重新啟用或停用自訂表單。 建議您停用自訂表單，不要刪除您不再用來保留歷史資料的表單。

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
   <td> <p>管理自訂表單的存取權</p> <p>如需Workfront管理員如何授予此存取許可權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取層級設定，請聯絡Workfront管理員。

## 停用自訂表單

您可以停用不再使用的自訂表單，而不會失去其關聯的歷史資料。 使用者無法新增非使用中的自訂表單至物件，但他們仍可檢視資料，並將資料新增至已附加該資料的物件上的欄位。

非作用中自訂表單上的欄位也仍然可以在檢視中進行內嵌編輯。 如果使用者在內聯編輯期間從非使用中自訂表單新增欄位，即使自訂表單已停用，該表單也會自動附加到物件。

若要停用自訂表單：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).
1. 在左側面板中，選擇 **自訂Forms**.
1. 在 **Forms** 索引標籤中，選取您要停用的自訂表單。
1. 在「作用中」欄中，選擇 **假** 並按一下以離開欄。 此表單已不在使用中。

## 重新啟用自訂表單

如果您重新啟用自訂表單，它會保留之前擁有的設定，使用者可以像從未停用它一樣與它互動。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).
1. 在左側面板中，選擇 **自訂Forms**.
1. 在 **Forms** 索引標籤中，選取您要重新啟用的自訂表單。
1. 在「作用中」欄中，選擇 **真** 並按一下以離開欄。 此表單現在為使用中。
