---
product-area: workfront-integrations
keywords: google，doc，檔案，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 適用於Google Workspace的Workfront中的隱私權與許可權
description: 適用於Google Workspace的Workfront中的隱私權與許可權
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 適用於Google Workspace的Workfront中的隱私權與許可權

>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，下列Google Workspace適用的Workfront功能在&#x200B;**2026年2月28日**&#x200B;後將無法使用：
>
>* 從Workfront存取Google Workspace功能
>
>* 從Gmail或Google行事曆網站面板檢視和管理Workfront工作
>
>為了滿足貴組織與Google Workspace的整合需求，我們建議您使用Workfront自動化和整合。
>
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Google Workspace之Workfront自動化與整合模組的特定功能相關資訊，請參閱[Gmail模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)和[Google行事曆模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)。

由於客戶隱私權很重要，Adobe Workfront不會儲存或收集任何因Google外掛程式應用程式的第三方授權而產生的識別客戶資料。 Google Workspace的Workfront使用從Google API收到的資訊並傳輸到任何其他應用程式時，將遵守[Google API服務使用者資料原則](https://developers.google.com/terms/api-services-user-data-policy)，包括有限使用要求。

我們需要下列許可權，才能讓適用於Google Workspace的Workfront外掛程式提供最大價值：

* **當附加元件執行時，檢視您的電子郵件訊息**： Google適用的Workfront Workspace外掛程式可將電子郵件轉換為Workfront中的新工作，並自動將電子郵件的主旨與內文填入工作的標題與說明，讓使用者省下無數小時的重複工作。 此外掛程式也可讓您將電子郵件作為新評論發佈至Workfront。 外掛程式必須在執行附加元件時檢視您的電子郵件訊息，才能傳遞此值。
* **以Gmail附加元件執行/不敏感**： Workfront需要許可權，Google Workspace附加元件才能在Gmail環境中運作。 外掛程式需要Gmail環境才能運作，因此需要`Run as a Gmail add-on / non-sensitive`許可權。
* **當附加元件執行時，檢視您的電子郵件訊息中繼資料**：為了改善工作流程，Google Workspace的Workfront外掛程式會確認電子郵件是否為Workfront通知，並識別Workfront通知的型別（新工作要求、核准要求、新註解等）。 外掛程式需要`View your email message metadata when the add-on is running`許可權才能傳遞此值。
* **外掛程式必須以Calendar附加元件執行/不敏感**：適用於Google Workspace的Workfront外掛程式會連線至您的行事曆，以便您以視覺效果呈現工作對排程的影響。 外掛程式需要`Run as a Calendar add-on / non-sensitive`許可權才能執行此操作。
* **連線到外部服務許可權：**&#x200B;外掛程式最終需要連線到Workfront API，這是外掛程式值的骨幹。 Workfront API是Google外部的服務，所以外掛程式需要`Connect to an external service permission`才能讓外掛程式運作。

如需有關Adobe Workfront致力於客戶隱私權的詳細資訊，請參閱[Workfront的隱私權通知](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf)。

如需詳細資訊，請參閱[Google API服務使用者資料原則](https://developers.google.com/terms/api-services-user-data-policy)。
