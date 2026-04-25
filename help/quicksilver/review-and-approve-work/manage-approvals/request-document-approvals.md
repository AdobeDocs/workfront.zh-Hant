---
product-area: documents
navigation-topic: approvals
title: 請求舊版檔案核准
description: 您可以在Adobe Workfront中要求管理員或其他使用者核准檔案。 如果您的Workfront管理員已啟用此功能（如設定系統安全性偏好設定中所述），您也可以向沒有Workfront帳戶的人要求檔案核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 3%

---

# 請求舊版檔案核准

您可以在Adobe Workfront中要求管理員或其他使用者核准檔案。 如果您的Workfront管理員已啟用此功能，您也可以向沒有Workfront帳戶的人要求檔案核准，如[設定系統安全性偏好設定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)中所述。

>[!NOTE]
>
>本文資訊是指舊版檔案核准。 <br>
>如需有關新的統一檢閱和核准的資訊，請參閱[統一檢閱和核准總覽](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)。


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

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show &quot;changes&quot; as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。
1. 尋找您需要的檔案。

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)

## Delete a document approval request

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。
1. 尋找您需要的檔案。

1. Scroll down to the **Approvals** section in the Summary, then click the **More** menu inline with the approver&#39;s name and select **Delete**.

   The approval request is removed and the approver receives a notification that their approval is no longer needed. Their approval-related share access is also removed.

## Send a reminder to an approver

You can send a message to remind document an approver that you&#39;re waiting for their feedback.

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。
1. 尋找您需要的檔案。

1. Scroll down to the **Approvals** section in the Summary, then click the **More** menu inline with the approver&#39;s name and select **Remind**.

   The approver receives a notification informing them the approval is still pending. They may also receive an email reminder if they have that enabled.
