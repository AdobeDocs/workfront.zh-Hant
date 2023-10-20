---
product-area: documents
navigation-topic: approvals
title: 請求檔案核准
description: 您可以在Adobe Workfront中要求管理員或其他使用者核准檔案。 如果您的Workfront管理員已啟用此功能（如設定系統安全性偏好設定中所述），您也可以向沒有Workfront帳戶的人要求檔案核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# 請求檔案核准

您可以在Adobe Workfront中要求管理員或其他使用者核准檔案。 如果您的Workfront管理員已啟用此功能（如所述），您也可以向沒有Workfront帳戶的人要求檔案核准 [設定系統安全性偏好設定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## 存取需求

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
   <td> <p>檢視專案、任務、問題、範本、Portfolio、方案、報告、儀表板和行事曆、檔案的或更高存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理與請求存取或核准相關聯的物件存取權 </p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 請求檔案核准

1. 前往包含檔案的專案、任務或問題，然後選取「 」 **檔案**.
1. 尋找您需要的檔案。

1. 向下捲動至 **核准** 區段，然後開始輸入 **新增核准者** 文字方塊。 您可以依名稱新增Workfront使用者，或透過電子郵件新增外部使用者。

1. 如果您的Adobe Workfront管理員已啟用與未使用Workfront的使用者共同作業的功能，如所述 [設定系統安全性偏好設定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)，您可以輸入其電子郵件地址來納入這些地址。

   您無法向團隊或群組要求核准。

1. 重複上一步驟以新增其他核准者。

## 在新版本上重新提交核准

上傳新版本時，檔案核准決定不會自動重設。 例如，如果您的檔案核准了變更，即使您上傳具有指定變更的新版本，決定仍會將「變更」顯示為決定。 如果您手動重新提交核准，則可以清除新版本上的決定。

1. 前往包含檔案的專案、任務或問題，然後選取「 」 **檔案**.
1. 尋找您需要的檔案。

1. 向下捲動至 **核准** 區段中的「摘要」，按一下「更多」圖示，然後按一下「重新提交」。

   ![](assets/nwe-resubmit-approval-350x149.png)

## 刪除檔案核准請求

1. 前往包含檔案的專案、任務或問題，然後選取「 」 **檔案**.
1. 尋找您需要的檔案。

1. 向下捲動至 **核准** 區段，然後按一下 **更多** 功能表內嵌核准者名稱並選取 **刪除**.

   核准請求會被移除，而核准者會收到不再需要其核准的通知。 也會移除其核准相關的共用存取權。

## 傳送提醒給核准者

您可以傳送訊息，提醒檔案核准者您正在等待他們的回饋意見。

1. 前往包含檔案的專案、任務或問題，然後選取「 」 **檔案**.
1. 尋找您需要的檔案。

1. 向下捲動至 **核准** 區段，然後按一下 **更多** 功能表內嵌核准者名稱並選取 **提醒**.

   核准者會收到通知，通知他們核准仍處於待定狀態。 如果已啟用，他們也會收到電子郵件提醒。
