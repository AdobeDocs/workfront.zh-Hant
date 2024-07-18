---
product-area: documents
navigation-topic: approvals
title: 請求文件核准
description: 您可以在Adobe Workfront中要求管理員或其他使用者核准檔案。 如果您的Workfront管理員已啟用此功能（如設定系統安全性偏好設定中所述），您也可以向沒有Workfront帳戶的人要求檔案核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 9a32fcc876efd5d5250b515c1c285f5375615510
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---

# 請求文件核准

您可以在Adobe Workfront中要求管理員或其他使用者核准檔案。 如果您的Workfront管理員已啟用此功能，您也可以向沒有Workfront帳戶的人要求檔案核准，如[設定系統安全性偏好設定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)中所述。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視專案、任務、問題、範本、Portfolio、方案、報告、儀表板和行事曆、檔案的或更高存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理與請求存取或核准相關聯的物件存取權 </p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

+++

## 請求檔案核准

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。
1. 尋找您需要的檔案。

1. 向下捲動至[摘要]中的&#x200B;**核准**&#x200B;區段，並開始輸入&#x200B;**新增核准者**&#x200B;文字方塊。 您可以依名稱新增Workfront使用者，或透過電子郵件新增外部使用者。

1. 如果您的Adobe Workfront管理員已啟用與未使用Workfront的人員共同作業的功能（如[設定系統安全性偏好設定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)中所述），您可以輸入他們的電子郵件地址來加入他們。

   您無法向團隊或群組要求核准。

1. 重複上一步驟以新增其他核准者。

## 在新版本上重新提交核准

上傳新版本時，檔案核准決定不會自動重設。 例如，如果您的檔案核准了變更，即使您上傳具有指定變更的新版本，決定仍會將「變更」顯示為決定。 如果您手動重新提交核准，則可以清除新版本上的決定。

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。
1. 尋找您需要的檔案。

1. 向下捲動至[摘要]中的&#x200B;**核准**&#x200B;區段，按一下[更多]圖示，然後按一下[重新提交]。

   ![](assets/nwe-resubmit-approval-350x149.png)

## 刪除檔案核准請求

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。
1. 尋找您需要的檔案。

1. 向下捲動至摘要中的&#x200B;**核准**&#x200B;區段，然後按一下內嵌核准者名稱的&#x200B;**更多**&#x200B;功能表並選取&#x200B;**刪除**。

   核准請求會被移除，而核准者會收到不再需要其核准的通知。 也會移除其核准相關的共用存取權。

## 傳送提醒給核准者

您可以傳送訊息，提醒檔案核准者您正在等待他們的回饋意見。

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。
1. 尋找您需要的檔案。

1. 向下捲動至摘要中的&#x200B;**核准**&#x200B;區段，然後按一下內嵌核准者名稱的&#x200B;**更多**&#x200B;功能表並選取&#x200B;**提醒**。

   核准者會收到通知，通知他們核准仍處於待定狀態。 如果已啟用，他們也會收到電子郵件提醒。
