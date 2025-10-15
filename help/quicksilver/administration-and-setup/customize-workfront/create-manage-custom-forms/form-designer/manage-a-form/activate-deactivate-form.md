---
title: 停用或重新啟用自訂表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以重新啟用或停用自訂表單。 建議您停用自訂表單，不要刪除您不再用來保留歷史資料的表單。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# 停用或重新啟用自訂表單

您可以重新啟用或停用自訂表單。 建議您停用自訂表單，不要刪除您不再用來保留歷史資料的表單。

>[!NOTE]
>
>如果自訂表單已停用，但仍屬於佇列主題或請求佇列定義，則會將其附加到新請求。 如果您不希望表單出現在請求中，則必須從請求佇列中手動將其移除。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr>  
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 停用自訂表單

您可以停用不再使用的自訂表單，而不會失去其關聯的歷史資料。 使用者無法新增非使用中的自訂表單至物件，但他們仍可檢視資料，並將資料新增至已附加該資料的物件上的欄位。

非作用中自訂表單上的欄位也仍然可以在檢視中進行內嵌編輯。 如果使用者在內聯編輯期間從非使用中自訂表單新增欄位，即使自訂表單已停用，該表單也會自動附加到物件。

若要停用自訂表單：

{{step-1-to-setup}}

1. 在左側面板中，選擇&#x200B;**自訂Forms**。
1. 在&#x200B;**Forms**&#x200B;區域中，選取您要停用的自訂表單。
1. 在[為使用中]欄中，選擇&#x200B;**False**，然後按一下退出該欄。 此表單已不在使用中。

## 重新啟用自訂表單

如果您重新啟用自訂表單，它會保留之前擁有的設定，使用者可以像從未停用它一樣與它互動。

{{step-1-to-setup}}

1. 在左側面板中，選擇&#x200B;**自訂Forms**。
1. 在&#x200B;**Forms**&#x200B;區域中，選取您要重新啟用的自訂表單。
1. 在[為使用中]欄中，選擇&#x200B;**True**，然後按一下退出該欄。 此表單現在為使用中。
