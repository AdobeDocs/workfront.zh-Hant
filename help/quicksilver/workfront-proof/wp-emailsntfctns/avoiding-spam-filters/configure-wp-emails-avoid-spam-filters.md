---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: 設定 [!DNL Workfront Proof] 封電子郵件以避免垃圾郵件篩選器
description: 您的電子郵件使用者端的垃圾郵件篩選器有一個重要的用途：保護您免受惱人的和可能的惡意垃圾郵件電子郵件的侵擾。 但是，如果垃圾郵件篩選器中沒有正確的設定，則可能會阻止您看到以下重要的 [!DNL Workfront Proof] 電子郵件：校訂電子郵件通知、電子報和特殊通訊。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 設定[!DNL Workfront Proof]封電子郵件以避免垃圾郵件篩選器

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

您的電子郵件使用者端的垃圾郵件篩選器有一個重要的用途：保護您免受惱人的和可能的惡意垃圾郵件電子郵件的侵擾。 但是，如果垃圾郵件篩選器中沒有正確的設定，可能會阻止您看到以下重要的[!DNL Workfront Proof]電子郵件：校訂電子郵件通知、電子報和特殊通訊。

為了確保您的[!DNL Workfront Proof]電子郵件一律被路由至您的收件匣，而不是您的垃圾郵件資料夾，您應該將以下內容新增至允許清單：

* [!DNL Workfront Proof]郵件伺服器： **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;電子郵件地址(例如，notification@proofhq.com)

如需有關要新增至允許清單的URL的詳細資訊，請參閱[設定防火牆允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)一文中的[設定防火牆允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## [!DNL Workfront Proof] &quot;[!UICONTROL 來自]&quot;電子郵件地址

根據您的電子郵件使用者端型別，您可能需要將[!DNL Workfront Proof]個[!UICONTROL 來自]的電子郵件地址新增至下列其中一項，以防止垃圾郵件篩選器日後將您的電子郵件路由至您的垃圾郵件資料夾：

* 您的連絡人清單
* 您的[!UICONTROL 安全寄件者]清單
* 您建立的篩選器，可將這些地址的電子郵件傳送到您的收件匣

您可能還需要從垃圾郵件資料夾中移除任何現有的[!DNL Workfront Proof]封電子郵件，並檢查是否有&quot;[!UICONTROL 來自]&quot;的位址在封鎖的位址清單中。 此說明頁面列出[!DNL Workfront Proof]個]的[!UICONTROL 位址，並顯示如何在下列電子郵件使用者端中將它們新增至垃圾郵件篩選器：

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>如果您對此處描述的程式有任何疑問，請檢視電子郵件使用者端的說明。

如需詳細資訊，請參閱[設定常見電子郵件使用者端的垃圾郵件設定](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md)。

## 要複製的[!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;電子郵件地址

若要確保您的[!DNL Workfront Proof]電子郵件送達您的收件匣，您需要將兩個[!DNL Workfront Proof]電子郵件地址分別新增到您的電子郵件使用者端的垃圾郵件篩選條件：

* 一般支援地址[!DNL support@proofhq.com]，[!DNL Workfront Proof]會從中傳送許多電子郵件通訊
* [!DNL Workfront Proof]傳送校樣通知電子郵件給校樣建立者和檢閱者（包含校樣連結）的通知地址。 這可能是一般地址、notification@support.proofhq.com，或者，如果您有自訂子網域或白色標籤網域，則可能是特定地址。

若要將[!DNL Workfront Proof]個[!UICONTROL 來自]的地址新增至電子郵件使用者端的篩選器：

1. 複製一般[!DNL Workfront Proof]支援「[!UICONTROL 來自]」電子郵件地址(support@proofhq.com)，並將其貼到您電子郵件使用者端所指定的欄位中。
1. 複製下列[!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;電子郵件地址中適當的一個，並將其個別貼到針對您的電子郵件使用者端所指定的欄位中：

   * notification@support.proofhq.com （如果您沒有自訂子網域或白色標籤網域）
   * notification@yoursubdomain.proofhq.com （如果您有自訂的子網域）；請在此位址中取代您的子網域名稱
   * notification@yoursubdomain.yourdomain.com （如果您有白色標籤網域）；請在此位址中取代您的子網域名稱和網域名稱

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
