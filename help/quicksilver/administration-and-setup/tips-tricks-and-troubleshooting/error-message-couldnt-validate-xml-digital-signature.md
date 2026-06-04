---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 錯誤訊息：無法驗證XML數位簽章
description: 您無法成功建立與ADFS的連線。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
TQID: https://experienceleague.adobe.com/lPAWprUiJA2ZJFUEdzXNTMTM1oXHEKNpc5VAadI-yqI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 274
ht-degree: 8%

---

# 錯誤訊息：無法驗證XML數位簽章

## 問題

您無法成功建立與ADFS的連線。

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>如果您建立了成功的測試連線，但仍遇到問題，則屬性對應可能不正確，或是同盟ID有問題。 如有疑問，請聯絡客戶支援。

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
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 原因1：憑證不正確

### 解決方案

手動從ADFS伺服器擷取簽署憑證：

1. 在[!DNL Windows]中，按一下&#x200B;**[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**。\
   隨即顯示「ADFS 2.0管理」對話方塊。

1. 在左窗格中選取&#x200B;**[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信任]**。

1. 用滑鼠右鍵按一下&#x200B;**[!UICONTROL 信賴方信任]**，然後選取&#x200B;**[!UICONTROL 內容]**。

1. 按一下&#x200B;**[!UICONTROL 簽章]**&#x200B;標籤。
1. 按一下簽署憑證的名稱，然後按一下[檢視]。****
1. 按一下[複製到&#x200B;**[!UICONTROL 檔案]**...]，然後選取&#x200B;**[!UICONTROL 下一步]**。

1. 選取&#x200B;**[!UICONTROL Base-64編碼的x.509 (CER)]**，然後按一下&#x200B;**[!UICONTROL 下一步]**。

1. 指定檔案名稱，然後按一下&#x200B;**[!UICONTROL 下一步]**。
1. 按一下「**[!UICONTROL 完成]**」。
1. 在[!DNL Adobe Workfront]中，瀏覽至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 系統]** > **[!UICONTROL 單一登入(SSO)]**，並手動上傳簽署憑證。

## 原因2：當[!DNL Workfront]需要RSA簽章時，使用DSA簽署憑證

### 解決方案

重新建立憑證並使用RSA簽章而非DSA。

## 原因3： XML資料不正確

### 解決方案

從ADFS管理系統重新匯出及重新匯入XML中繼資料。

## 原因4：由於SAML端發生錯誤，無法執行請求

### 解決方案

請聯絡您的SAML提供者。
