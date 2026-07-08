---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: 使用Adobe Cloud Drive
description: 直接從Finder或檔案總管使用Adobe Cloud Drive使用Adobe雲端儲存空間專案。 在任何應用程式中開啟和編輯檔案、離線工作以及解決衝突。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: d5dd769447e81d5d95b4907f8a01016b118f2322
workflow-type: tm+mt
source-wordcount: 1723
ht-degree: 1%

---

# 使用Adobe Cloud Drive

安裝Adobe Cloud Drive後，您可以直接從Finder或檔案總管使用Adobe雲端儲存空間專案。 您可以在任何應用程式中開啟及編輯檔案、離線工作，以及讓Adobe Cloud Drive將您的變更同步至雲端。

如需有關安裝Adobe Cloud Drive的資訊，請參閱[安裝Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront版本</td> 
   <td>工作流程Ultimate，已啟用Adobe雲端儲存空間</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>
      <p>檢視專案的存取權，以便在Adobe Cloud Drive中檢視</p>
      <p>編輯專案的存取權以新增、編輯或刪除專案中的檔案</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 存取您的專案

1. 開啟Finder (Mac)或檔案總管(Windows)。
1. 導覽至&#x200B;**Adobe Cloud Drive**。
1. 在Workfront中瀏覽您有權存取的專案清單。 開啟任何專案資料夾以檢視其檔案和子資料夾。

   >[!NOTE]
   >
   >* 專案資料夾的最上層為唯讀。 您無法重新命名、刪除或移動專案資料夾本身。
   >* 您可以處理專案資料夾內的檔案和資料夾 — 開啟、編輯、建立、刪除等等。
   >* 舊版Workfront專案不會出現在Adobe Cloud Drive中。 只有儲存在Adobe雲端儲存空間中的專案才可使用。

## 檔案狀態指示器

Adobe Cloud Drive使用視覺指示器來顯示檔案同步處理狀態。 圖示在Windows和Mac之間有所不同。

### Windows上的檔案狀態指示器

| 圖示 | 狀態 | 檔案含義 | 資料夾含義 |
| --- | --- | --- | --- |
| ![僅限線上圖示](assets/acd-windows-online-only.png) | 僅限線上 | 檔案已同步，但只能線上上使用。 | 內的所有檔案都可線上上取得。 |
| ![正在同步處理圖示](assets/acd-windows-syncing.png) | 同步中 | 檔案的最新更新正在同步至本機快取或Adobe雲端儲存空間。 | 資料夾中至少有一個檔案正在同步。 |
| ![可用的離線圖示](assets/acd-windows-available-offline.png) | 可離線使用 | 檔案已同步且可離線使用。 | 資料夾中至少有一個檔案可離線使用。 |
| ![釘選圖示](assets/acd-windows-pinned.png) | 已固定（永遠保留在裝置上） | 檔案已同步且一律保持離線。 Adobe Cloud Drive不會自動清除釘選內容。 | 資料夾中的所有檔案都位於本機快取中，並可離線存取。 |
| ![唯讀圖示](assets/acd-windows-read-only.png) | 唯讀 | 檔案是唯讀的。 | 資料夾是唯讀的。 |
| ![同步處理錯誤圖示](assets/acd-windows-sync-error.png) | 同步錯誤 | 無法同步檔案。 將滑鼠指標暫留在圖示上即可檢視詳細資訊。 | 資料夾無法同步。 將滑鼠指標暫留在圖示上即可檢視詳細資訊。 |
| ![同步處理排除的圖示](assets/acd-windows-sync-excluded.png) | 已排除同步 | 檔案無法同步，因為型別或名稱不受支援。 | 資料夾無法同步，因為名稱不受支援。 |

### Mac上的檔案狀態指示器

| 圖示 | 狀態 | 檔案含義 | 資料夾含義 |
| --- | --- | --- | --- |
| （無圖示） | 可離線使用 | 檔案已同步且可離線使用。 | 所有檔案都可以離線存取。 |
| ![僅限線上圖示](assets/acd-mac-online-only.png) | 僅限線上 | 檔案已同步且僅可線上上使用。 | 資料夾中至少有一個檔案是線上檔案。 |
| ![正在同步處理圖示](assets/acd-mac-syncing.png) | 同步中 | 檔案的最新更新正在同步至本機快取或Adobe雲端儲存空間。 | 資料夾內容正在同步。 |
| ![同步處理錯誤圖示](assets/acd-windows-sync-error.png) | 同步錯誤 | 檔案無法更新或同步。 將滑鼠指標暫留在圖示上即可檢視詳細資訊。 | 資料夾無法更新或同步。 將滑鼠指標暫留在圖示上即可檢視詳細資訊。 |
| ![同步處理排除的圖示](assets/acd-windows-sync-excluded.png) | 已排除同步 | 檔案已從同步中排除。 | 已從同步處理中排除資料夾。 |
| ![唯讀圖示](assets/acd-mac-read-only.png) | 唯讀 | 檔案是唯讀的。 | 資料夾是唯讀的。 |
| ![釘選圖示](assets/acd-windows-pinned.png) | 已固定（永遠保留在裝置上） | 檔案已釘選為可離線使用。 Adobe Cloud Drive不會自動清除釘選內容。 | 資料夾已釘選為可離線使用。 |

### 錯誤工具提示

發生同步錯誤或問題時，將滑鼠移至檔案或資料夾圖示上，即可檢視說明問題的工具提示。

| 錯誤類別 | 工具提示 | 含義 |
|---|---|---|
| 已排除同步 | 不受支援的檔案類型 | Adobe Cloud Drive不支援此檔案型別。 |
| 已排除同步 | 不支援的檔案名稱 | Adobe Cloud Drive不支援此檔案名稱。 |
| 已排除同步 | 父專案已刪除 | 父Workfront專案已刪除。 |
| 同步處理已暫停 | 不支援的檔案內容 | 無法同步檔案內容（例如，偵測到安全性問題）。 |
| 同步處理已暫停 | 檔案名稱中的字元無效 | 檔案名稱包含無效的字元。 |
| 同步處理已暫停 | 完整路徑太長 | 檔案路徑超過允許的最大長度。 |
| 同步處理已暫停 | 沒有寫入許可權 | 您對此檔案或專案的寫入許可權已撤銷。 |
| 同步錯誤 | 驗證問題 | 您的登入認證發生問題。 |
| 同步錯誤 | 雲端儲存空間無法使用 | Adobe雲端服務暫時無法使用。 |
| 同步錯誤 | 雲端儲存空間已滿 | 您的雲端儲存空間配額已滿。 |
| 同步錯誤 | 本機磁碟已滿 | 您的本機磁碟沒有足夠的可用空間。 |
| 同步錯誤 | 沒有網際網路連線 | 您的裝置未連線到網際網路。 |
| 同步錯誤 | 意外錯誤 | 同步處理期間發生未預期的錯誤。 |
| 同步錯誤 | 帳戶已封鎖 | 服務已封鎖您的帳戶。 |

>[!NOTE]
>
>系統層級的錯誤（例如中斷連線、驗證失敗、網路無法使用、本機磁碟已滿或雲端儲存空間已滿）會顯示在系統匣或功能表列(Mac)中，而不是顯示在個別檔案中。

## 開啟檔案

1. 在Adobe Cloud Drive中，導覽至檔案。
1. 連按兩下檔案。

   檔案會在其預設應用程式中開啟。

Adobe Cloud Drive支援電腦上安裝的應用程式可開啟的任何檔案型別，包括：

* Adobe Creative Cloud格式（PSD、AI、INDD、PROJ、AEP等）
* Microsoft Office檔案(DOCX、XLSX、PPTX)
* 影像（JPG、PNG、GIF等）
* 視訊檔案（MP4、MOV等）

>[!NOTE]
>
>當您透過Adobe Cloud Drive存取Cloud檔案格式（PDC、AIDC等）時，這些格式會開啟為它們的標準對應專案（PSD、AI等）。

## 編輯並儲存檔案

1. 從Adobe雲端磁碟機開啟檔案。
1. 在應用程式中進行變更。
1. 選取&#x200B;**檔案** > **儲存**，或按Ctrl+S (Windows)或Cmd+S (Mac)來儲存檔案。

   您的變更會自動同步至Adobe雲端儲存空間。

>[!IMPORTANT]
>
>使用&#x200B;**檔案** > **儲存**&#x200B;或鍵盤快速鍵儲存檔案。 避免使用&#x200B;**另存新檔**&#x200B;來建立復本，因為它會在磁碟機中產生重複的檔案。

## 建立或新增檔案

您可以直接在專案中建立新檔案，或從本機儲存空間中新增現有檔案。

### 從應用程式建立新檔案

1. 開啟您要用來建立檔案的應用程式。
1. 建立檔案，如同您一般的作法。
1. 儲存時，請選擇Adobe Cloud Drive專案資料夾中的位置。

   檔案會顯示在Adobe Cloud Drive中，並同步至Adobe雲端儲存空間。

### 將現有檔案新增至專案

1. 在Finder (Mac)或檔案總管(Windows)中，開啟Adobe Cloud Drive中的專案資料夾。
1. 將檔案從本機存放區拖曳或複製到專案資料夾中。

   檔案會自動同步至Adobe雲端儲存空間。

## 讓檔案和資料夾可離線使用

當檔案或資料夾可以離線使用時，您無需網際網路連線即可開啟及編輯。 離線檔案使用本機磁碟空間。

### 在裝置上保留檔案或資料夾

1. 在Adobe Cloud Drive中的檔案或資料夾上按一下滑鼠右鍵。
1. 選取&#x200B;**永遠保留在此裝置上**。

   檔案或資料夾會下載至本機快取，即使離線也能使用。

### 移除離線存取以釋放空間

1. 以滑鼠右鍵按一下離線檔案或資料夾。
1. 選取&#x200B;**釋放空間**。

   檔案或資料夾仍保留在雲端儲存空間，但已從本機快取中移除。

>[!NOTE]
>
>離線檔案和資料夾使用本機磁碟空間。 移除您不再需要釋放空間的檔案和資料夾的離線存取權。

## 將檔案複製到本機儲存空間

您可以將檔案從Adobe雲端磁碟機複製到本機磁碟機。 原始檔案會保留在Adobe Cloud Drive中，而復本會成為獨立的本機檔案。

1. 在Adobe Cloud Drive中的檔案上按一下滑鼠右鍵。
1. 選取「**複製**」，然後將檔案貼到您本機磁碟機上您想要的位置。

   檔案會複製到目的地。 原始檔案仍儲存在Adobe Cloud Drive中。

>[!NOTE]
>
>複製到本機儲存體的檔案是獨立的復本。 您對本機復本進行的變更不會同步回Adobe雲端儲存空間。

## 登出Adobe Cloud Drive

如果您登出Adobe Cloud Drive，該磁碟機仍會顯示在「尋找器」或「檔案總管」中。 不過，您登出時在磁碟機內所做的任何變更，以及在登出前未同步處理的任何變更，都不會同步處理至雲端。

接下來發生的事情取決於您使用哪個帳戶重新登入。

### 使用相同帳戶重新登入

當您登出時，Adobe Cloud Drive會保留本機掛載的資料夾。 如果您使用相同的認證重新登入：

* Adobe Cloud Drive會自動重複使用現有的掛載。
* 您登出前所做的任何未同步變更都會保留，並在連線恢復後同步。
* 您無需執行任何動作。

### 使用其他帳戶登入

如果您在登出後使用其他Adobe帳戶登入：

* 目前掛載的資料夾會自動重新命名並備份。 備份資料夾名稱使用此格式： `Adobe Cloud Drive <usermail>_<short_guid> (backup yyyy-MM-dd HH-mm-ss)`。
* 如往常一樣，對應至新帳戶的Adobe Cloud Drive可在Finder或File Explorer中使用。
* 在移除備份資料夾之前，您可以手動復原任何未同步的工作。

>[!NOTE]
>
>備份資料夾儲存在Mac上的`~/Library/CloudStorage`和Windows上的`C:\Users\<user>\`中。 如果您多次切換帳戶，則會建立多個時間戳記備份資料夾。 定期檢閱及清理備份，以釋放磁碟空間。

## 解決檔案衝突

衝突可能發生在以下任何情況中：

* 多位使用者同時編輯或刪除相同的檔案。
* 當其他使用者開啟檔案時，該檔案會被修改。
* 網路中斷會導致同步問題。

### Adobe Cloud Drive如何解決衝突

Adobe Cloud Drive使用複製策略來處理衝突：

* **沒有檔案鎖定。** 多位使用者可同時編輯檔案。
* **自動複製。** Adobe Cloud Drive偵測到衝突時，會保留兩個版本。
* **清除命名。** 衝突檔案包含下列格式的使用者名稱和時間戳記： `filename (Conflicted copy from username on date_time).extension`。 例如: `hero-banner (Conflicted copy from John on 2026-02-10_16-06-44).psd`。

### 手動解決衝突

1. 識別衝突檔案。 衝突檔案的檔案名稱中有「衝突的副本」。
1. 請檢閱兩個版本以判斷哪一個是正確的。
1. 保留正確的版本，並刪除其他版本。
1. 為保留的檔案指定適當的名稱。

>[!TIP]
>
>若要將衝突最小化：
>
>* 請先檢查同步狀態，然後再編輯檔案。
>* 與團隊成員溝通誰正在編輯哪些檔案。
>* 經常儲存，以便立即同步變更。
>* 完成編輯後關閉檔案。
