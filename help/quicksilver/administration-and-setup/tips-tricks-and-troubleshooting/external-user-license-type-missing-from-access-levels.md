---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 訪問級別中缺少外部用戶許可類型
description: 在「設定」的「存取層級」下，我無法再看到「外部使用者授權類型」。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 訪問級別中缺少外部用戶許可類型

## 問題

在「設定」的「存取層級」下，我無法再看到「外部使用者授權類型」。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 系統]** > **[!UICONTROL 偏好設定]**.

1. 在 **[!UICONTROL 安全性]** 區段，確定選項 **[!UICONTROL 使用無Workfront帳戶的使用者電子郵件地址與他們合作]** 啟用。

   如果未啟用此選項，外部用戶將不會顯示在訪問級別設定中。
