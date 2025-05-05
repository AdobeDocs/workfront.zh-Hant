---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 延遲校訂電子郵件
description: 當校訂接近截止日期或到達截止日期時，將向收件者傳送延遲校訂電子郵件。 這些型別的電子郵件無法在校訂層級停用，但可在帳戶和使用者個人設定層級設定。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL 延遲校訂]電子郵件

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

當校訂接近截止日期或到達截止日期時，會傳送[!UICONTROL 延遲校訂]電子郵件給收件者。 這些型別的電子郵件無法在校訂層級停用，但可在帳戶和使用者個人設定層級設定。

* [!UICONTROL 延遲校訂]當校訂到達截止日期且並非所有評論或決定都已完成時，會自動傳送電子郵件給檢閱者。

  這些電子郵件預設為啟用，且無法針對整個帳戶進行調整，但使用者可以在其「校訂」預設值中停用它們。

* 當校訂接近截止日期時，會向稽核者傳送風險電子郵件。 預設會停用，並可在[!UICONTROL 帳戶設定]中啟用。 啟用後，它們也可以在[!UICONTROL 校訂預設值]中調整。

無法自訂這些通知。

收到通知的人員包括：

* 擁有者，只有在[!UICONTROL 電子郵件]警示時驗證延遲，在[!UICONTROL 擁有者的驗證預設值]中才會核取。
* 尚未對校訂做出決定的任何核准者。 如需決定的相關資訊，請參閱[在校訂檢視器中對校訂做出決定](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>如果[!UICONTROL 帳戶設定]中的電子郵件通知已停用為預設值，即使檢閱者和核准者尚未提交其評論和決定，也不會傳送任何[!UICONTROL 延遲校訂]電子郵件。 您也可以在校訂預設值中停用[!UICONTROL 延遲校訂]電子郵件。

關於校樣通知，請考慮以下事項：

* 您的[!DNL Workfront]管理員或[!DNL Workfront Proof]管理員可以在您的電子郵件通知中包含您組織的標誌，如[品牌化 [!DNL Workfront Proof] 網站](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md)中所述。
* 如果您需要與相同檢閱者共用多個校樣，並且不希望他們收到多個電子郵件，您可以同時上傳他們。 所有檢閱者都會收到一封電子郵件，詳細說明所有校訂，並包含每個校訂的個人URL。

  >[!NOTE]
  >
  >校訂的建立者會收到每個已建立校訂的個別[!UICONTROL 校訂]電子郵件。 如需詳細資訊，請參閱[校訂內容]電子郵件(../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)。

* 如果您或您的檢閱者沒有收到預期的電子郵件通知，請參閱[設定 [!DNL Workfront Proof] 電子郵件以避免垃圾郵件篩選器](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md)。
