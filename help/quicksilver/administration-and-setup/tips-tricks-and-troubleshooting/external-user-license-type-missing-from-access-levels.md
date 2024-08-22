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
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 1%

---

# 存取層級中缺少外部使用者授權型別

## 問題

我在「設定」的「存取層級」底下無法再看到外部使用者授權型別。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是[!DNL Workfront]管理員。 </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解決方案

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 系統]** > **[!UICONTROL 偏好設定]**。

1. 在&#x200B;**[!UICONTROL 安全性]**&#x200B;區段中，確定已啟用選項&#x200B;**[!UICONTROL 透過電子郵件地址與沒有Workfront帳戶的人合作]**。

   如果未啟用此選項，則外部使用者不會出現在存取層級設定中。
