---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 錯誤：自動布建的使用者無法登入
description: 如果自動布建的使用者首次嘗試登入，並收到系統未指派存取層級的錯誤，這可能是因為您的系統缺少與請求授權關聯的存取層級。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 3%

---

# 錯誤：自動布建的使用者無法登入

當自動布建的使用者嘗試第一次登入時，他們會收到以下錯誤：

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## 問題

系統沒有為新使用者指派存取層級。

依預設，自動布建會使用請求授權型別。 當沒有具有「請求」授權的存取層級存在時，系統無法將存取層級指派給使用者。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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

使用請求授權建立基本存取層級：

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 存取層級]**。

1. 按一下&#x200B;**[!UICONTROL 新增存取層級]**。
1. 輸入&#x200B;**[!UICONTROL 名稱]**。
1. 在&#x200B;**[!UICONTROL 授權型別]**&#x200B;下拉式功能表中，選取[要求]。
1. 按一下「**[!UICONTROL 儲存變更]**」。

使用「要求」授權建立存取層級後，請讓使用者使用其SSO憑證登入。


