---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 防止欺騙並添加 [!DNL Adobe Workfront] SPF記錄
description: 如果使用者未收到 [!DNL Adobe Workfront] 電子郵件通知，您需要新增 [!DNL Workfront] SPF記錄到防火牆。 您必須與IT團隊合作，以新增SPF記錄。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 防止欺騙並添加 [!DNL Adobe Workfront] SPF記錄

## 問題

如果使用者未收到 [!DNL Adobe Workfront] 電子郵件通知，您需要新增 [!DNL Workfront] SPF記錄到防火牆。 您必須與IT團隊合作，以新增SPF記錄。

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

如果您已將IP位址新增至生產環境的允許清單，如 [配置防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 和使用者仍未收到電子郵件：

1. 將以下SPF記錄添加到防火牆：

   *spf.workfront.com*

   這會自動新增所有 [!DNL Workfront] 防火牆上允許清單的IP地址，允許驗證所有垃圾郵件過濾器（使用SPF記錄） [!DNL Workfront] 伺服器作為域的有效發件人。

   >[!NOTE]
   >
   > SPF記錄是DNS區域檔案的一部分的TXT記錄。 不支援修改您的DNS區域檔案。

1. 必須指定需要配置的SPF記錄類型。 以下是有效的SPF記錄類型：

   * all(https://dmarcian.com/spf-syntax-table/#all)
   * ip4(https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6(https://dmarcian.com/spf-syntax-table/#ip6)
   * a(https://dmarcian.com/spf-syntax-table/#a)
   * mx(https://dmarcian.com/spf-syntax-table/#mx)
   * ptr(https://dmarcian.com/spf-syntax-table/#ptr)
   * 存在(https://dmarcian.com/spf-syntax-table/#exists)
   * 包括(https://dmarcian.com/spf-syntax-table/#include)

   例如，&quot;v=spf1 a mx包括： [spf.workfront.com](http://spf.workfront.com/) -all」

如果由於公司策略而無法將SPF記錄添加到防火牆，請與您的 [!DNL Workfront] 支援代表。
