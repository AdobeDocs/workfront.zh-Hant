---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 延遲校樣電子郵件
description: 當校樣接近截止日期或接近截止日期時，會傳送「延遲校樣」電子郵件給收件者。 這些類型的電子郵件無法在校樣層級停用，但可在帳戶和使用者個人設定層級設定。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL 延遲校樣] 電子郵件

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

此 [!UICONTROL 延遲校樣] 當校樣接近截止日期或接近截止日期時，會傳送電子郵件給收件者。 這些類型的電子郵件無法在校樣層級停用，但可在帳戶和使用者個人設定層級設定。

* [!UICONTROL 延遲校樣] 當校樣達到截止日期且並非所有審核或決定均已完成時，系統會自動傳送電子郵件給審核者。

   這些電子郵件預設為啟用，且無法針對整個帳戶進行調整，但使用者可在其校對預設值中停用這些電子郵件。

* 在風險情況下，當證明接近截止日期時，會傳送電子郵件給審核者。 預設會停用，並可在 [!UICONTROL 帳戶設定]. 啟用後，也可在 [!UICONTROL 校對預設值].

無法自訂這些通知。

將收到通知的人員包括：

* 擁有者，只有 [!UICONTROL 電子郵件] 校樣延遲時的警報已勾選 [!UICONTROL 所有者校對預設值].
* 任何尚未對校樣做決定的批准者。 如需決策的相關資訊，請參閱 [在校對檢視器中決定校樣](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>如果 [!UICONTROL 帳戶設定]，否 [!UICONTROL 延遲校樣] 即使審核者和批准者尚未提交其評論和決定，也會發送電子郵件。 您也可以停用 [!UICONTROL 延遲校樣] 校對預設值中的電子郵件。

請考量下列校樣通知：

* 您的 [!DNL Workfront] 管理員或 [!DNL Workfront Proof] 管理員可在電子郵件通知中加入貴組織的標誌，如 [品牌 [!DNL Workfront Proof] 網站](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* 如果您需要與同一位審核者共用多個校樣，但不希望他們收到多封電子郵件，則可同時上傳。 所有審核者都會收到一封電子郵件，其中詳細說明所有校樣，並包含每個校樣的個人URL。

   >[!NOTE]
   >
   >校樣的建立者會收到個別的 [!UICONTROL 證明] 針對所建立的每個校樣傳送電子郵件。 如需詳細資訊，請參閱 [此 [!UICONTROL 製作校樣] 電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* 如果您或您的審核者未收到預期的電子郵件通知，請參閱  [設定 [!DNL Workfront Proof] 避免垃圾郵件過濾器的電子郵件](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
