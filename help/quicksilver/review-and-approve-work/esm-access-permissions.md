---
product-area: documents
navigation-topic: approvals
title: Adobe企業儲存模式的物件許可權和存取層級總覽
description: Adobe企業儲存許可權和存取許可權概覽
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
source-git-commit: 8b8f638f089ff967fe7d4fb641b23f5836ac86b5
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---

# Adobe企業儲存模式的物件許可權和存取層級總覽

<!--linked in UI -->

Adobe企業儲存解決方案是雲端型儲存解決方案，可作為Adobe企業產品中資產的中央儲存庫。 使用Adobe企業儲存空間的Workfront環境與使用舊版Workfront檔案儲存空間的環境相比，物件許可權和存取層級行為稍有不同。

## 存取層級

Workfront存取層級僅適用於Workfront。 Workfront中的專案和檔案限制並不一定適用於其他Adobe應用程式。

### 同時使用Adobe企業儲存空間與舊版Workfront儲存空間的環境

視專案位於Adobe企業儲存空間或舊版Workfront儲存空間而定，檔案存取的行為會有所不同：

* **舊版Workfront儲存空間**：使用舊版Workfront儲存空間的專案、計畫、產品組合和範本會遵循標準Workfront存取層級邏輯進行檔案存取。 當存取層級為檔案選取&#x200B;**沒有存取權**&#x200B;時，他們無法在Workfront或其他Adobe產品（如Frame.io或Creative Cloud）中檢視檔案。
* **Adobe企業儲存空間**：使用Adobe企業儲存空間的專案、程式、產品組合和範本，會依循其他Adobe產品的Adobe企業儲存空間存取層級邏輯。


   * **專案、程式、產品組合及範本物件許可權**：當存取層級針對專案、程式、產品組合及範本選取&#x200B;**無存取權**，但物件已與他們共用，使用者無法在Workfront中檢視物件，但他們仍可在其他Adobe工具（例如Frame.io和Adobe Creative Cloud）中檢視物件名稱及任何關聯檔案。
   * **檔案許可權**：當存取層級為檔案選取&#x200B;**無存取權**&#x200B;時，使用者無法在Workfront中檢視專案上的檔案，但他們仍可在其他Adobe工具（例如Frame.io和Adobe Creative Cloud）中檢視和管理與其共用專案的檔案。 這是因為檔案存取權是由Adobe企業儲存中的專案層級許可權所決定，而非僅由Workfront存取層級所決定。

如果您的Workfront環境中啟用了Adobe企業儲存空間，您可以建立Adobe企業儲存空間專案和舊版Workfront儲存空間專案。 舊版Workfront儲存專案會在Workfront中顯示的專案名稱旁顯示圖示。 Adobe企業儲存體專案不會顯示圖示。

專案名稱旁的![舊版workfront儲存體圖示](assets/legacy-project-icon.png)


### 僅使用Adobe企業儲存空間的環境

您無法修改使用Adobe企業儲存空間的專案、程式和產品組合之存取層級的檔案許可權。

所有存取層級都有檔案的編輯存取權。 專案層級的許可權會決定其他Adobe工具中的檔案存取權。

您無法限制檔案繼承存取權。


### 僅使用舊版Workfront儲存空間的環境

檔案存取層級或行為沒有變更。

## 物件許可權

物件許可權會決定您能在Workfront中檢視與處理專案、任務、問題和檔案的內容。 當有人與您共用物件時，就會指派許可權。

>[!IMPORTANT]
>
>在Adobe企業儲存體中，檔案許可權的運作方式與舊版Workfront儲存體不同。 檔案會繼承其連結的專案、任務或問題的許可權。


### 檔案許可權的運作方式

檔案許可權是由檔案所連結的物件所驅動。 您無法在個別檔案上設定許可權。

當您將檔案上傳到任務或問題時，系統會使用任務或問題名稱建立系統產生的資料夾。 此資料夾已連結至任務或問題並繼承其許可權。

您可以在系統產生的資料夾中建立子資料夾，以進一步組織檔案。 所有子檔案夾都從父檔案夾繼承許可權。 在專案層級，您可以在資料夾之外上傳檔案，但只有具有專案層級存取許可權的使用者才能看到這些檔案。

在專案層級，系統產生的資料夾會顯示連結物件。 這通常是任務或問題名稱，也是系統如何知道應在該資料夾上看到哪個任務或問題的方式。

### 專案許可權

當您擁有專案層級的許可權時，可以在Workfront和其他Adobe產品（例如Frame.io和Adobe Creative Cloud）中檢視和管理該專案的檔案。 這些工具中也會顯示專案名稱。 Workfront外部不會顯示其他專案資料。

### 任務和問題許可權

任務和問題繼承來自專案的許可權。 當您擁有任務或問題層級的許可權時，可以在Workfront和其他Adobe產品（例如Frame.io和Adobe Creative Cloud）中檢視和管理連結到該任務或問題的檔案。

**系統產生的資料夾**

* 從任務或問題中移除使用者不會自動移除其資料夾存取權。 他們可能仍可透過專案層級的許可權進行存取。
* 子任務不會從父任務繼承系統產生的檔案夾許可權。 您必須直接新增至子任務，才能存取其系統產生的資料夾。
* 將使用者新增到任務或問題共用該物件的系統產生的資料夾。

**正在移動和重新命名系統產生的資料夾：**

* 系統產生的資料夾可以重新命名和移動。
* 如果系統產生的資料夾移至其他位置，其連結物件會更新為新物件。 然後，許可權會從新的父物件繼承。

請求遵循與任務和問題相同的行為。

### 核准

將您新增至檔案核准工作流程後，無論專案許可權為何，您都可以看到以下內容：

* 專案名稱
* 文件名稱
* 文件縮圖










