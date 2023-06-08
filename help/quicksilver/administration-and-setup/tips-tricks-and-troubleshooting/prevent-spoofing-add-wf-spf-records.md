---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 防止詐騙並新增 [!DNL Adobe Workfront] SPF記錄
description: 如果使用者沒有收到 [!DNL Adobe Workfront] 電子郵件通知，您需要新增 [!DNL Workfront] SPF記錄至您的防火牆。 您必須與IT團隊合作，才能新增SPF記錄。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 防止詐騙並新增 [!DNL Adobe Workfront] SPF記錄

## 問題

如果使用者沒有收到 [!DNL Adobe Workfront] 電子郵件通知，您需要新增 [!DNL Workfront] SPF記錄至您的防火牆。 您必須與IT團隊合作，才能新增SPF記錄。

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
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完全管理存取權</a>.</p> <p><b>注意</b>：如果您還是無法存取，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需如何進行 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

如果您已將IP位址新增至生產環境的允許清單，如所述 [設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 而使用者仍然沒有收到電子郵件：

1. 將下列SPF記錄新增至防火牆：

   *spf.workfront.com*

   這會自動新增全部 [!DNL Workfront] 防火牆上允許清單的IP位址，並允許所有垃圾郵件篩選器（使用SPF記錄）進行驗證 [!DNL Workfront] 伺服器作為您網域的有效寄件者。

   >[!NOTE]
   >
   > SPF記錄是DNS區域檔案中的TXT記錄。 我們不支援修改您的DNS區域檔案。

1. 您必須指定需要設定的SPF記錄型別。 以下是有效的SPF記錄型別：

   * 全部(https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * 存在(https://dmarcian.com/spf-syntax-table/#exists)
   * 包含(https://dmarcian.com/spf-syntax-table/#include)

   例如，「v=spf1 a mx include： spf.workfront.com -all」

如果因為公司原則而無法將SPF記錄新增至防火牆，請與您的合作。 [!DNL Workfront] 支援代表。
