---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 存取層級中缺少外部使用者授權型別
description: 我在「設定」的「存取層級」底下無法再看到外部使用者授權型別。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 2%

---

# 存取層級中缺少外部使用者授權型別

## 問題

我在「設定」的「存取層級」底下無法再看到外部使用者授權型別。

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

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 系統]** > **[!UICONTROL 偏好設定]**。

1. 在&#x200B;**[!UICONTROL 安全性]**&#x200B;區段中，確定已啟用選項&#x200B;**[!UICONTROL 透過電子郵件地址與沒有Workfront帳戶的人合作]**。

   如果未啟用此選項，則外部使用者不會出現在存取層級設定中。
