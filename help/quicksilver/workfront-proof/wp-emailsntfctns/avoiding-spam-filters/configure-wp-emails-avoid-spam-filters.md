---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: 設定 [!DNL Workfront Proof] 避免垃圾郵件過濾器的電子郵件
description: 「您的電子郵件用戶端的垃圾郵件篩選器有重要用途：保護您免受煩人且可能惡意垃圾郵件的侵擾。 但是，如果您的垃圾郵件篩選器中沒有正確的設定，則可能會阻止您看到以下重要資訊 [!DNL Workfront Proof] 電子郵件：校樣電子郵件通知、電子報和特殊通訊。」
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 設定 [!DNL Workfront Proof] 避免垃圾郵件過濾器的電子郵件

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

您的電子郵件用戶端的垃圾郵件篩選器有重要用途：保護您免受煩人且可能惡意垃圾郵件的侵擾。 但是，如果您的垃圾郵件篩選器中沒有正確的設定，則可能會阻止您看到以下重要資訊 [!DNL Workfront Proof] 電子郵件：校樣電子郵件通知、電子報和特殊通訊。

確保您的 [!DNL Workfront Proof] 電子郵件一律會路由至您的收件匣，而非垃圾郵件資料夾，您應將下列項目新增至允許清單：

* [!DNL Workfront Proof] 郵件伺服器： **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL 從]「電子郵件地址(例如， notification@proofhq.com)

如需要新增至允許清單之URL的詳細資訊，請參閱 [配置防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 在文章中 [配置防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL 從]「電子郵件地址」

視您的電子郵件用戶端類型而定，您可能需要新增 [!DNL Workfront Proof] &quot;[!UICONTROL 從]「電子郵件地址，用於防止垃圾郵件過濾器在將來將電子郵件路由到垃圾郵件資料夾：

* 您的聯繫人清單
* 您的 [!UICONTROL 安全發件人] 清單
* 您建立的篩選器，用於將電子郵件從這些地址傳送至收件匣

您也可能需要移除任何現有 [!DNL Workfront Proof] 從垃圾郵件資料夾發送電子郵件，並檢查「[!UICONTROL 從]「地址在被阻止的地址清單上。 此說明頁面會列出 [!DNL Workfront Proof] &quot;[!UICONTROL 從]」地址並顯示如何將這些地址添加到以下電子郵件客戶端中的垃圾郵件過濾器：

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>如果您對此處描述的程式有任何疑問，請查看您的電子郵件客戶的幫助。

如需詳細資訊，請參閱 [配置常見電子郵件客戶端的垃圾郵件設定](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## 此 [!DNL Workfront Proof] &quot;[!UICONTROL 從]&quot;複製的電子郵件地址

確保您的 [!DNL Workfront Proof] 電子郵件到達收件匣時，您需要新增兩個 [!DNL Workfront Proof] 電子郵件地址分別指向電子郵件客戶端的垃圾郵件過濾器：

* 一般支助地址， [!DNL support@proofhq.com]，從 [!DNL Workfront Proof] 發送了許多電子郵件
* 來自的通知地址 [!DNL Workfront Proof] 傳送校樣通知電子郵件給校樣建立者和具有校樣連結的審核者。 如果您有自訂的子網域或白標籤網域，則這可能是一般位址、notification@support.proofhq.com或特定位址。

若要新增 [!DNL Workfront Proof] &quot;[!UICONTROL 從]「 」電子郵件用戶端篩選器的地址：

1. 複製一般 [!DNL Workfront Proof] 支援&quot;[!UICONTROL 從]「電子郵件地址(support@proofhq.com)，並貼到您電子郵件用戶端所指示的欄位中。
1. 複製下列適當項目之一 [!DNL Workfront Proof] &quot;[!UICONTROL 從]「電子郵件地址並個別貼到您電子郵件用戶端所指示的欄位中：

   * notification@support.proofhq.com如果您沒有自訂的子網域或白標籤網域，
   * notification@yoursubdomain.proofhq.com（如果您有自訂的子網域）;在此位址取代您的子網域名稱
   * notification@yoursubdomain.yourdomain.com（如果您有白標籤域）;在此位址中取代您的子網域名稱和網域名稱

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
