---
title: AtTask OnPremise支援政策
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
description: Adobe Workfront改用100%的「軟體即服務」模式，並於2011年12月31日停止銷售內部部署軟體。 自2014年起，不再支援AtTask OnPremise，但許可證密鑰相關問題除外。 無法再下載或安裝內部部署應用程式。
feature: System Setup and Administration
role: Admin
exl-id: 37c65360-6587-43b3-8eaf-4f1a9b375c1d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# AtTask OnPremise支援政策

Adobe Workfront改用100%的「軟體即服務」模式，並於2011年12月31日停止銷售內部部署軟體。 自2014年起，不再支援AtTask OnPremise，但許可證密鑰相關問題除外。 無法再下載或安裝內部部署應用程式。

如果您已擁有應用程式且需要重新安裝OnPremise，請下載安裝指南。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">OnPremise optimization tips can be found.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more about reporting in AtTask OnPremise, click.</p>
-->

下載SSL/TSL設定的指示。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 更新OnPremise授權密鑰

如果您需要新的許可證密鑰，請致電844-306-HELP(4357)，與Workfront客戶支援聯繫。

一旦你獲得了新的許可證密鑰，

1. 停止atTask伺服器。
1. 更名當前的license.key檔案（位於AtTaskDoc資料夾中）。
1. 將新的license.key檔案複製到位。
1. 重新啟動atTask伺服器。

本文包含下列附件：
