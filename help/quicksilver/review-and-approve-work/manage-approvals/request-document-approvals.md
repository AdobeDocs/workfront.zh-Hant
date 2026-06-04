---
product-area: documents
navigation-topic: approvals
title: 請求舊版檔案核准
description: 您可以在Adobe Workfront中要求管理員或其他使用者核准檔案。 如果您的Workfront管理員已啟用此功能（如設定系統安全性偏好設定中所述），您也可以向沒有Workfront帳戶的人要求檔案核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
TQID: https://experienceleague.adobe.com/NQgXFcbc-4DiObeNE2nRgaW9iKeCKRD5v7J1PRfHkHU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 530
ht-degree: 3%

---

# 請求舊版檔案核准

您可以在Adobe Workfront中要求管理員或其他使用者核准檔案。 如果您的Workfront管理員已啟用此功能，您也可以向沒有Workfront帳戶的人要求檔案核准，如[設定系統安全性偏好設定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)中所述。

>[!NOTE]
>
>本文資訊是指舊版檔案核准。<br>
>如需新的統一檢閱和核准的相關資訊，請參閱[統一檢閱和核准總覽](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)。


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>貢獻或更高</p>
   <p>評論或以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案、任務、問題、範本、投資組合、計畫、報告、儀表板和行事曆、檔案的或更高存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理與請求存取或核准相關聯的物件存取權 </p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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

   ![重新提交核准](assets/nwe-resubmit-approval-350x149.png)

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
