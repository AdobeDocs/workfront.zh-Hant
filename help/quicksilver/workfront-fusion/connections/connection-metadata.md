---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Adobe Workfront Fusion中的連線中繼資料
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Adobe Workfront Fusion中的連線中繼資料

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [連線中繼資料](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/connections/connection-metadata.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

>[!NOTE]
>
>除了[!DNL Adobe Workfront]授權之外，[!DNL Adobe Workfront Fusion]還需要[!DNL Adobe Workfront Fusion]授權。

並非所有連線都相同。 瞭解不同連線之間的差異對於瞭解其業務環境非常重要。 Fusion使用中繼資料來識別連線的重要屬性。

建立新連線時，可以設定連線中繼資料。 這些屬性位於用來設定連線的同一個對話方塊中：

![連線中繼資料](assets/connection-metadata-setup.png)

Fusion使用者可以從「連線」區域檢視及編輯連線。

![連線區域中的連線中繼資料](assets/connections-area-metadata.png)

## 環境型別

生產和非生產系統都可以使用Fusion連線。 瞭解差異對於保護生產環境非常重要。 請注意，環境型別（如同其他連線中繼資料）僅供參考之用。 使用者仍需負責準確設定此屬性。

## 驗證類型

Fusion連線可用於服務帳戶和個人帳戶。 當案例自動做為Fusion時，會使用服務帳戶進行驗證。 個人帳戶是根據特定人員的驗證。 使用的驗證型別取決於情境的需求。 個人帳戶應該用於自動使用者動作。 例如，如果Fusion案例自動進行特定人員的核准，則驗證型別應為該人員。 否則，Fusion將充當Fusion，型別應為「服務帳戶」。

請注意，與其他連線中繼資料一樣，型別僅供參考。 使用者仍需負責手動準確設定此屬性。

如需驗證型別的詳細資訊，請參閱Adobe驗證指南中的[驗證](https://developer.adobe.com/developer-console/docs/guides/authentication/)。
