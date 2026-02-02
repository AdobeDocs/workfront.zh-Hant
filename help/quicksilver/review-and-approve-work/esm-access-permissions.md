---
product-area: documents
navigation-topic: approvals
title: Adobe企業儲存模式的物件許可權和存取層級總覽
description: Adobe企業儲存許可權和存取許可權概覽
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---


# Adobe企業儲存模式的物件許可權和存取層級總覽

<!--linked in UI -->

Adobe企業儲存解決方案是雲端型儲存解決方案，可作為Adobe企業產品中資產的中央儲存庫。 使用Adobe企業儲存空間的Workfront環境與使用舊版Workfront檔案儲存空間的環境相比，物件許可權和存取層級行為稍有不同。

## 存取層級

Workfront存取層級僅適用於Workfront。 Workfront中的專案和檔案限制並不一定適用於其他Adobe應用程式。

### 同時使用Adobe企業儲存空間與舊版Workfront儲存空間的環境

視專案位於Adobe企業儲存空間或舊版Workfront儲存空間而定，檔案存取的行為會有所不同：

* **舊版Workfront儲存空間**：使用舊版Workfront儲存空間的專案、計畫、產品組合和範本會遵循標準Workfront存取層級邏輯進行檔案存取。 當存取層級為檔案選取&#x200B;**沒有存取權**&#x200B;時，他們無法在Workfront或其他Adobe產品(如Frame.io或Creative Cloud)中檢視檔案。
* **Adobe企業儲存空間**：使用Adobe企業儲存空間的專案、程式、產品組合和範本，會依循其他Adobe產品的Adobe企業儲存空間存取層級邏輯。


   * **專案、程式、產品組合及範本物件許可權**：當存取層級針對專案、程式、產品組合及範本選取&#x200B;**無存取權**，但物件已與他們共用，使用者無法在Workfront中檢視物件，但他們仍可在其他Adobe工具(例如Frame.io和Adobe Creative Cloud)中檢視物件名稱及任何關聯檔案。
   * **檔案許可權**：當存取層級為檔案選取&#x200B;**無存取權**&#x200B;時，使用者無法在Workfront中檢視專案上的檔案，但他們仍可在其他Adobe工具(例如Frame.io和Adobe Creative Cloud)中檢視和管理與其共用專案的檔案。 這是因為檔案存取權是由Adobe企業儲存中的專案層級許可權所決定，而非僅由Workfront存取層級所決定。

如果您的Workfront環境中啟用了Adobe企業儲存空間，您可以建立Adobe企業儲存空間專案和舊版Workfront儲存空間專案。 舊版Workfront儲存專案會在Workfront中顯示的專案名稱旁顯示圖示。 Adobe企業儲存體專案不會顯示圖示。

專案名稱旁的![舊版workfront儲存體圖示](assets/legacy-project-icon.png)


### 僅使用Adobe企業儲存空間的環境

您無法修改使用Adobe企業儲存空間的專案、程式和產品組合之存取層級的檔案許可權。

所有存取層級都有檔案的編輯存取權。 專案層級的許可權會決定其他Adobe工具中的檔案存取權。

您無法限制檔案繼承存取權。


### 僅使用舊版Workfront儲存空間的環境

檔案存取層級或行為沒有變更。


## 專案

具有專案層級許可權的使用者可以檢視及管理其他Adobe產品(例如Frame.io和Adobe Creative Cloud)中的專案檔案。

針對ESM專案，專案名稱也會顯示在Workfront外部。

針對ESM專案，財務資料不會顯示在Workfront之外。

## 任務和問題

檔案儲存在專案層級，但可視需要與個別任務和問題共用。 具有任務和問題存取許可權的使用者會自動繼承專案的檔案存取許可權。 您無法修改其存取層級。 使用者具有管理存取權或無權存取。