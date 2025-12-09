---
title: 列出使用者的存取層級和授權
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，層級，授權
navigation-topic: access-levels
description: 您可以在使用者清單或報告中檢視指派給每個使用者的存取層級和授權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5d85509d-276a-411e-813c-8b1fa2f512db
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 5%

---

# 列出使用者的存取層級和授權

>[!NOTE]
>
>本文資訊參考舊版存取層級。 如需新存取層級的資訊，請參閱[新存取層級概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。

您可以在使用者清單或報告中檢視指派給每個使用者的存取層級和授權。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

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
   <td>規劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視對使用者的存取權。 如需有關檢視使用者存取許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 列出使用者的存取層級和授權

{{step-1-to-users}}

依預設，所有被設定為「作用中」的使用者都會顯示在清單中。

1. 在&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**授權**。

   「許可證」欄顯示指派給每個使用者的許可證名稱。

1. 在&#x200B;**群組**&#x200B;下拉式功能表中，按一下&#x200B;**授權型別**。

   此檢視會將擁有相同授權型別的使用者分組。

1. （選擇性）若要依特定授權篩選清單：

   1. 按一下&#x200B;**篩選器**&#x200B;下拉式功能表，然後按一下&#x200B;**新增篩選器**。

   1. 按一下&#x200B;**新增篩選規則**。
   1. 開始輸入&#x200B;**授權**，並在它出現在清單中時選取它。
   1. 選取&#x200B;**Equal**&#x200B;修飾元後，開始輸入您要用來篩選清單的授權名稱。

      您可以指定多個授權型別。

   1. 按一下「**儲存篩選器**」。

      清單僅顯示與您在篩選器中指定的授權型別相關聯的使用者。

   >[!TIP]
   >
   >您也可以依授權型別將清單分組，或依特定授權篩選。

