---
product-area: workfront-integrations
keywords: google,doc，文檔，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: Workfront for G套裝的隱私權和權限
description: Workfront for G套裝的隱私權和權限
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 0862af846ca77c33132ec631cf1e3eae253d3cd8
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Workfront for G套裝的隱私權和權限

由於客戶隱私權很重要，Adobe Workfront不會儲存或收集因第三方授權Google外掛程式應用程式而產生的任何識別客戶資料。

我們需要下列權限，Workfront for G Suite外掛程式才能提供其最大值：

* **在載入項運行時查看您的電子郵件**:Workfront for G Suite外掛程式可將電子郵件轉換為Workfront中的新工作，並自動以電子郵件的主旨和內文填入工作的標題和說明，借此節省使用者數以萬計的重複工作時間。 外掛程式也可讓您將電子郵件以新留言形式發佈至Workfront。 外掛程式執行時需要檢視您的電子郵件訊息才能傳送此值。
* **執行as a Gmail附加元件/不敏感**:需要Workfront for G Suite附加元件的權限，才能在Gmail環境中運作。 外掛程式需要Gmail環境才能運作，因此需要 `Run as a Gmail add-on / non-sensitive` 權限。
* **執行附加元件時檢視您的電子郵件訊息中繼資料**:為了改善工作流程，Workfront for G Suite外掛程式會確認電子郵件是否為Workfront通知，並識別Workfront通知的類型（新工作請求、核准請求、新留言等）。 外掛程式需要 `View your email message metadata when the add-on is running` 傳遞此值的權限。
* **外掛程式需要以日曆附加元件/非敏感狀態執行**:Workfront for G Suite外掛程式可連線至您的日曆，讓您將工作對排程的影響視覺化呈現。 外掛程式需要 `Run as a Calendar add-on / non-sensitive` 權限。
* **連接到外部服務權限：** 最終，外掛程式需要連線至Workfront API，而API是外掛程式值的骨幹。 Workfront API是Google外部的服務，因此外掛程式需要 `Connect to an external service permission` 讓外掛程式正常運作。

如需Adobe Workfront致力於保護客戶隱私的詳細資訊，請參閱 [Workfront的隱私聲明](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

