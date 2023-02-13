---
title: 列出使用者的存取層級和授權
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 訪問，級別，許可
navigation-topic: access-levels
description: 您可以在使用者清單或報表中，查看指派給每位使用者的存取層級和授權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5d85509d-276a-411e-813c-8b1fa2f512db
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# 列出使用者的存取層級和授權

您可以在使用者清單或報表中，查看指派給每位使用者的存取層級和授權。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視使用者的存取權。 如需檢視使用者之存取權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 列出使用者的存取層級和授權

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者**.

   依預設，設為「作用中」的所有使用者都會顯示在清單中。

1. 在 **檢視** 下拉式功能表，選取 **授權**.

   「許可證」列顯示分配給每個用戶的許可證的名稱。

1. 在 **分組** 下拉式功能表，按一下 **許可證類型**.

   此檢視會將具有相同授權類型的使用者分組。

1. （選用）若要依特定授權篩選清單：

   1. 按一下 **篩選** 下拉式功能表，然後按一下 **新增篩選**.

   1. 按一下 **新增篩選規則**.
   1. 開始鍵入 **授權** 並在清單中出現時選取它。
   1. 使用 **等於** 修改量，開始鍵入要篩選清單的許可證名稱。

      您可以指定多個許可證類型。

   1. 按一下 **儲存篩選**.

      清單僅顯示與您在篩選器中指定的授權類型相關聯的使用者。
   >[!TIP]
   >
   >您也可以依授權類型將清單分組，或依特定授權進行篩選。

