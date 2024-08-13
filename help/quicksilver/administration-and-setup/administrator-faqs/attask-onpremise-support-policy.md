---
title: AtTask OnPremise支援原則
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
description: Adobe Workfront改採100%軟體即服務模式，並於2011年12月31日停止銷售內部部署軟體。 自2014年起，除了授權金鑰相關問題外，不再支援AtTask OnPremise。 內部部署應用程式無法再下載或安裝。
feature: System Setup and Administration
role: Admin
exl-id: 37c65360-6587-43b3-8eaf-4f1a9b375c1d
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# AtTask OnPremise支援原則

Adobe Workfront改採100%軟體即服務模式，並於2011年12月31日停止銷售內部部署軟體。 自2014年起，除了授權金鑰相關問題外，不再支援AtTask OnPremise。 內部部署應用程式無法再下載或安裝。

如果您已經有應用程式且需要重新安裝OnPremise，請下載安裝指南。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">OnPremise optimization tips can be found.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more about reporting in AtTask OnPremise, click.</p>
-->

下載有關SSL/TSL設定的指示。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。 如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 更新OnPremise授權金鑰

如果您需要新的授權金鑰，請致電844-306-HELP(4357)，聯絡Workfront客戶支援。

取得新的授權金鑰後，

1. 停止atTask伺服器。
1. 重新命名目前的license.key檔案（位於AtTaskDoc資料夾）。
1. 將新的license.key檔案複製到適當位置。
1. 重新啟動atTask伺服器。

本文包含下列附件：
