---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 錯誤訊息： SAML 2.0驗證失敗：找不到使用者識別碼
description: 使用SAML 2.0時，「找不到SAML 2.0驗證失敗的使用者識別碼」錯誤表示未從ADFS宣告規則傳遞UID或NAME ID。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
TQID: https://experienceleague.adobe.com/YxLEE1OvD-Wo3FSd5ewXMfijsTaCjjCjzAx-EWWlBPE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 225
ht-degree: 8%

---

# 錯誤訊息： SAML 2.0驗證失敗：找不到使用者識別碼

## 問題

我在使用SAML 2.0時收到此錯誤：「SAML 2.0驗證失敗：找不到使用者識別碼。」

## 原因

當未從&#x200B;**ADFS宣告規則**&#x200B;傳遞&#x200B;**UID**&#x200B;或&#x200B;**名稱ID**&#x200B;時，就會發生這種情況。

在ADFS中，**信賴方信任**&#x200B;必須有傳遞&#x200B;**UID**&#x200B;或&#x200B;**名稱ID**&#x200B;值的&#x200B;**宣告規則**。 當您執行&#x200B;**[!DNL Workfront]測試連線**&#x200B;時，如果成功，應該會顯示此連線。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

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
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解決方案

1. 編輯&#x200B;**[!UICONTROL ADFS資訊]**&#x200B;時，在&#x200B;**[!UICONTROL 信賴方信任]** >選取物件>**[!UICONTROL 編輯宣告規則]**&#x200B;中。

1. **[!UICONTROL LDAP屬性]** （左欄）應該有&#x200B;**[!UICONTROL 電子郵件地址]** （或任何唯一識別碼）。

1. **[!UICONTROL 傳出宣告型別]** （右欄）應為&#x200B;**[!UICONTROL 名稱ID]**。

   >[!NOTE]
   >
   >它不一定要有LDAP屬性電子郵件地址。 可以使用任何可識別使用者的唯一識別碼，但必須將其傳入[!DNL Adobe Workfront]做為&#x200B;**名稱ID**。
