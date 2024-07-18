---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 存取層級中缺少外部使用者授權型別
description: 我在「設定」的「存取層級」底下無法再看到外部使用者授權型別。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 存取層級中缺少外部使用者授權型別

## 問題

我在「設定」的「存取層級」底下無法再看到外部使用者授權型別。

## 存取需求

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。 如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> <p><b>注意</b>：如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 系統]** > **[!UICONTROL 偏好設定]**。

1. 在&#x200B;**[!UICONTROL 安全性]**&#x200B;區段中，確定已啟用選項&#x200B;**[!UICONTROL 透過電子郵件地址與沒有Workfront帳戶的人合作]**。

   如果未啟用此選項，則外部使用者不會出現在存取層級設定中。
