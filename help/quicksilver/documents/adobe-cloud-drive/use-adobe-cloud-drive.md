---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: 使用Adobe Cloud Drive
description: 直接從Finder或檔案總管使用Adobe Cloud Drive使用Adobe雲端儲存空間專案。 在任何應用程式中開啟和編輯檔案、離線工作以及解決衝突。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 19e1a78a32429ddba173583bf56af8acc5d72eb0
workflow-type: tm+mt
source-wordcount: '3955'
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

### 同步排除清單

Adobe Cloud Drive不會同步處理某些系統產生的暫存及鎖定檔案。 下列檔案型別和模式已排除：

| 類別 | 檔案型別/模式 | 說明 |
|---|---|---|
| 系統檔案 | `.DS_Store`, `Thumbs.db` | 作業系統中繼資料和縮圖快取檔案。 |
| 系統和虛擬記憶體檔案 | `*.sys` （例如，`hiberfil.sys`、`pagefile.sys`、`swapfile.sys`） | 用於虛擬記憶體、休眠或其他作業系統功能的大型系統檔案。 |
| macOS索引檔案 | `.Spotlight-V100`, `.fseventsd` | macOS Spotlight索引和檔案系統事件追蹤檔案。 |
| 暫存和備份檔案 | `*.tmp`, `*.swp`, `*~`, `*.bak` | 應用程式產生的暫時、暫時或備份檔案。 |

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
1. Select **永遠保留在此裝置上**。

   檔案或資料夾會下載至本機快取，即使離線也能使用。

### 移除離線存取以釋放空間

1. 以滑鼠右鍵按一下離線檔案或資料夾。
1. Select **釋放空間**。

   檔案或資料夾仍保留在雲端儲存空間，但已從本機快取中移除。

>[!NOTE]
>
>離線檔案和資料夾使用本機磁碟空間。 移除您不再需要釋放空間的檔案和資料夾的離線存取權。

## 將檔案複製到本機儲存空間

您可以將檔案從Adobe雲端磁碟機複製到本機磁碟機。 原始檔案會保留在Adobe Cloud Drive中，而復本會成為獨立的本機檔案。

1. 在Adobe Cloud Drive中的檔案上按一下滑鼠右鍵。
1. Select **複製**，然後將檔案貼到您本機磁碟機上您想要的位置。

   檔案會複製到目的地。 原始檔案仍儲存在Adobe Cloud Drive中。

>[!NOTE]
>
>複製到本機儲存體的檔案是獨立的復本。 您對本機復本進行的變更不會同步回Adobe雲端儲存空間。

<!-- Courtney check me: New sections below (Upload to Cloud through Open in Workfront) added for Adobe Cloud Drive v1.2.0, per helpxNewFeature.pdf from Pulkit Goel. Verify content, placement, and heading order. -->

## 上傳檔案至雲端（直接上傳） {#direct-upload}

<!-- Courtney check me: Source PDF calls this "Upload to Cloud (Direct Upload)". Confirm heading wording. -->

直接上傳會將檔案從您的電腦直接傳送到Adobe雲端儲存空間，無需先將檔案複製到Adobe雲端磁碟機資料夾。

<!-- Courtney check me: Removed folder mentions from the Direct Upload section (intro, heading, step 1, 500-file bullet, hidden files bullet, and the Sync Activity link text), per Pulkit: folder support isn't available yet. Confirm nothing else should change. -->

### 上傳檔案

1. 在Finder (Mac)或檔案總管(Windows)中的檔案上按一下滑鼠右鍵。
1. Select **上傳至雲端**。
1. 在目的地選擇器中，選取Adobe Cloud Drive中其中一個專案的位置，然後按一下&#x200B;**「上傳到這裡」**。
1. 在同步活動視窗的&#x200B;**直接上傳**&#x200B;區段中監視進度。

### 直接上傳須知事項

* 直接上傳會將專案複製到雲端。 原始專案會保留在其目前位置。
* 您可以選取多個專案一次上傳。
* 「直接上傳」區段只會列出個別檔案，上限為500個。
* 您可以從使用者主目錄或任何附加的外部磁碟機上傳專案。 不支援其他雲端儲存位置，例如iCloud磁碟機或`~/Library/CloudStorage`。
* 您必須使用已授權的Adobe帳戶登入。 您不需要網際網路連線即可開始上傳。 如果沒有連線，上傳會維持佇列中。
* 暫停同步會取消進行中的上傳。 當您繼續同步時，已排入佇列的上傳會自動繼續。
* 如果您在上傳期間結束Adobe Cloud Drive，進行中的上傳會標示為已取消。 當您重新啟動應用程式時，已排入佇列的上傳會自動繼續。
* 不支援隱藏的檔案、符號連結和別名。
* Adobe Cloud Drive可控制同時執行的上傳數量。 其餘的上傳會一直排入佇列，直到插槽可供使用為止。
* 會顯示即時上傳計數，包括失敗的上傳，例如「3個檔案上傳」。 當所有上傳成功完成時，計數會變更為摘要，例如「3個檔案已上傳」。 Select **關閉**&#x200B;以將其移除。

<!-- Courtney check me: "Pausing sync cancels uploads in progress" and the quit behavior are from the PDF. Confirm with dev that both are intended. -->

### 上傳狀態

<!-- Courtney check me: Icons extracted from the PDF (48x48 px, low resolution) and named by table order. Verify each icon matches its status and ask Pulkit's team for higher-resolution originals. Add alt text review too. -->

| 圖示 | 狀態 | 說明 | 可用動作 |
| --- | --- | --- | --- |
| ![已排入佇列的圖示](assets/acd-upload-status-queued.png) | 已排入佇列 | 上傳正在等待開始。 | **取消**&#x200B;取消此專案。 |
| ![正在上傳圖示](assets/acd-upload-status-uploading.png) | 正在上傳 | 上傳進行中。 | **取消**&#x200B;取消此專案。 |
| ![已完成圖示](assets/acd-upload-status-completed.png) | 已完成 | 上載已成功完成。 | 在Workfront中&#x200B;**開啟**&#x200B;會在Workfront網頁介面中開啟資產。 |
| ![失敗的圖示](assets/acd-upload-status-failed.png) | 失敗 | 無法完成上傳。 | **顯示來源檔案**&#x200B;會顯示原始檔案。 **重試**&#x200B;重試上傳。 重試僅適用於特定故障。 |
| ![已取消圖示](assets/acd-upload-status-cancelled.png) | 已取消 | 上傳已由您或系統停止。 | 無。 取消的上傳不會重試。 您必須開始新的上傳。 |

若要檢視失敗的原因，請將游標停留在失敗的專案上。

### 管理上傳清單

每個動作僅在套用時可用。

* **取消所有上傳：**&#x200B;上傳排入佇列或進行中時可用。 取消所有欄位。
* **重試失敗的上傳：**&#x200B;當存在可以重試的失敗的上傳時可用。 請重試所有步驟。 無法重試的上傳將維持不變。
* **清除：**&#x200B;當沒有佇列或進行中的上傳時可用。 移除所有已完成、失敗和取消的專案。 已上傳的本機檔案和內容不受影響。
* **自動清除：**&#x200B;已完成、失敗和取消的專案會在上次更新後24小時自動移除。 排入佇列及進行中的專案永遠不會自動移除。

## 暫停並繼續同步 {#pause-resume-sync}

如果您不想讓Adobe Cloud Drive上傳或下載檔案，例如透過緩慢或計量的網際網路連線，您可以暫停該裝置。 同步暫停時，您的變更不會傳送至雲端，且雲端的變更不會下載至您的電腦。 同步處理會保持暫停狀態，直到您恢復為止。

### 暫停同步

1. 按一下系統匣中的Adobe Cloud Drive圖示(Windows)或功能表列(Mac)。
1. 按一下Adobe Cloud Drive視窗右上角的&#x200B;**功能表**&#x200B;圖示(≡)。
1. Select **暫停同步**。

   >[!TIP]
   >
   >在Adobe Cloud Drive視窗開啟的狀態下，您也可以按下Ctrl+P (Windows)或Command+P (Mac)。

   Adobe Cloud Drive視窗顯示&#x200B;**同步處理已暫停**，而且訊息&#x200B;**在您繼續之前，檔案將不會同步**。 當您將游標暫留在Adobe Cloud Drive圖示上時，會顯示&#x200B;**Adobe Cloud Drive （已暫停）**。

>[!NOTE]
>
>暫停同步只會在您登入且已連線Adobe Cloud Drive時提供。

### 繼續同步

1. 按一下系統匣中的Adobe Cloud Drive圖示(Windows)或功能表列(Mac)。
1. 執行下列其中一項：

   * 按一下&#x200B;**繼續**。
   * 按一下&#x200B;**功能表**&#x200B;圖示(≡)，然後選取&#x200B;**繼續同步**。 開啟視窗後，您也可以按Ctrl+R (Windows)或Command+R (Mac)。

   Adobe Cloud Drive會再次開始同步，包括同步暫停時所進行的所有變更。

## 檢視及管理版本記錄 {#version-history}

您可以使用Adobe Cloud Drive中的「版本記錄」來瀏覽已儲存的支援檔案雲端版本、檢視版本詳細資料和縮圖，以及回覆成先前的版本。 如果您擁有必要的許可權，也可以編輯版本的名稱和說明。

### 檢視版本記錄

1. 在Finder或檔案總管中導覽至您的Adobe Cloud Drive資料夾。
1. Select為支援的檔案。
1. 在檔案上按一下滑鼠右鍵，然後選取&#x200B;**版本記錄**。
1. Select版本可檢視其可用詳細資料和縮圖。

   如果檔案沒有舊版，則顯示&#x200B;**沒有舊版**。 縮圖可能無法用於每個檔案或版本。

### 編輯版本資訊

1. 開啟檔案的版本記錄。
1. Select您要更新的版本。
1. 開啟版本的選項功能表，並選取&#x200B;**編輯版本資訊**。
1. 輸入&#x200B;**版本名稱**&#x200B;或&#x200B;**描述**。
1. 選取&#x200B;**「儲存」**。

   更新後的資訊會儲存並在您重新開啟「版本記錄」時顯示。

### 還原至較早的版本

1. 開啟檔案的版本記錄。
1. Select您要還原的版本。
1. Select **還原為此版本** （如果可用）。
1. 等候同步處理完成。
1. 重新開啟檔案，確認所選版本的內容目前為最新版本。

## 管理本機儲存空間 {#manage-local-storage}

您可以使用Adobe Cloud Drive中的「管理本機儲存空間」來監視本機磁碟使用量、設定儲存空間限制，以及檢視標示為&#x200B;**永遠在此裝置上**&#x200B;的檔案。

<!-- Courtney check me: PDF says "Always on this device" here but this article uses "Always Keep On This Device" for the right-click option. Confirm which label the UI shows in each place. -->

### 檢視本機儲存空間使用量

1. Select Adobe Cloud Drive圖示，並開啟其選項功能表。
1. Select **管理本機儲存空間**。
1. 檢閱目前的儲存使用情況以及此裝置&#x200B;**上標示為**&#x200B;永遠的檔案清單。
1. 依&#x200B;**名稱**&#x200B;或&#x200B;**大小**&#x200B;排序檔案清單，以尋找特定檔案。

### 變更本機儲存限制

1. 從Adobe Cloud Drive選項功能表開啟&#x200B;**管理本機儲存空間**。
1. 輸入所需的儲存空間限制。
1. Select **儲存**&#x200B;以套用變更。

>[!NOTE]
>
>設定儲存限制時，請確定裝置上有足夠的可用磁碟空間。

## 檢視同步活動 {#sync-activity}

同步活動會顯示您電腦上的Adobe雲端磁碟機資料夾與Adobe雲端儲存空間之間的最近活動。 用它來監視上傳和下載、檢閱完成的變更，並識別無法同步的專案。

### 檢視同步活動

1. Select功能表列(Mac)或系統匣(Windows)中的Adobe雲端磁碟機圖示。
1. 使用同步活動狀態摘要旁邊的箭頭展開同步活動區段。
1. 檢閱列出的專案及其狀態指示器。 將游標停留在狀態指標上可檢視傳輸進度、完成的作業或錯誤訊息。
1. Select專案旁的更多動作功能表，可檢視可用於該專案的動作。

### 同步活動的相關須知事項

* 一般同步會追蹤透過Adobe Cloud Drive資料夾進行的變更，包括上傳、下載、建立、重新命名、移動和刪除。
* 一般同步清單包含最多500個最近的專案。 新的或更新專案會顯示在頂端。 當清單達到其限制時，可能會移除較舊的專案。
* 正在解析專案名稱或中繼資料時，專案一開始可以顯示&#x200B;**正在準備……**。
* 摘要會顯示目前同步處理的專案數。 **同步處理完成**&#x200B;表示目前沒有作用中的專案。 檢查清單中失敗或排除的專案，而不是將此摘要視為每個專案都成功的確認。
* 從同步中排除的檔案和資料夾會出現錯誤，說明不支援的名稱、不支援的型別或其他排除原因。
* 當您登出時，活動會被清除。 此清單是活動檢視，而非永久稽核歷史記錄。

### 同步狀態

<!-- Courtney check me: The PDF has two sync status tables (page 7 with 4 statuses, page 8 with 3 statuses and icons). I used the page 8 icons with the page 7 descriptions where they overlap. Confirm and decide whether to keep both tables. -->

| 圖示 | 狀態 | 說明 | 可用動作 |
| --- | --- | --- | --- |
| 等候指標 | 正在等候同步 | 專案正在等待其作業開始。 | 在Finder **(Mac)中顯示**&#x200B;或在Explorer **(Windows)中顯示** （如果適用）。 |
| ![正在上傳圖示](assets/acd-sync-status-uploading.png) | 上傳/下載 | 正在傳輸檔案內容。 將滑鼠指標暫留在指標上，可檢視轉移方向和百分比（可用時）。 在100%時，工具提示可能會顯示&#x200B;**正在完成……**，直到處理完成。 | **在Finder中顯示**&#x200B;或&#x200B;**在Explorer中顯示** （如果適用）。 |
| ![已完成圖示](assets/acd-sync-status-completed.png) | 已同步/完成的作業 | 操作已完成。 工具提示可以在雲端上識別已上傳、已下載、已建立、已重新命名、已重新命名、已移動、已刪除或已刪除。 | 在尋找器&#x200B;**中顯示**&#x200B;或在總管&#x200B;**中顯示**&#x200B;未刪除的專案。 在Workfront中&#x200B;**開啟**，以取得合格的已完成且未刪除的專案。 |
| ![失敗的圖示](assets/acd-sync-status-failed.png) | 同步失敗/已排除 | 專案無法同步或已從同步處理中排除。 將游標停留在指標上可檢視原因。 | **在Finder中顯示**&#x200B;或&#x200B;**在Explorer中顯示** （如果適用）。 在預期專案要同步之前，先解決報告的問題。 |

已刪除的專案無法在本機顯示，也無法透過其活動專案在Workfront中開啟。

### 管理活動清單

| 動作 | 說明 |
| --- | --- |
| 展開或摺疊 | 使用同步摘要旁邊的箭頭可顯示或隱藏個別專案。 |
| 在Finder中顯示/在Explorer中顯示 | 在Adobe Cloud Drive資料夾中找到未刪除的專案。 |
| 在Workfront中開啟 | 在瀏覽器的Workfront中開啟合格的已完成專案。 此動作不適用於作用中、失敗或刪除的正常同步專案。 |
| 清除 | 沒有作用中的正常同步專案時可用。 從活動檢視中清除完成的專案，包括失敗的專案。 清除記錄不會刪除本機檔案或雲端內容，也無法解決同步失敗。 |
| 關閉 | 清除完成的批次後，可能會顯示同步專案摘要。 Select的關閉按鈕可關閉摘要。 |

>[!NOTE]
>
>Normal-sync資料列不提供直接上傳使用的每個專案&#x200B;**重試**&#x200B;或&#x200B;**取消**&#x200B;動作。 如需直接上傳的相關資訊，請參閱[將檔案上傳至雲端（直接上傳）](#direct-upload)。

## 在Workfront中開啟專案 {#open-in-workfront}

在Workfront中開啟會將Adobe Cloud Drive中的專案帶往瀏覽器中Workfront中的對應位置。 使用此外掛程式來繼續使用Workfront中的雲端專案，而不需手動搜尋。

### 從「尋找器」或「檔案總管」開啟專案

1. 在Finder (Mac)或檔案總管(Windows)中開啟Adobe Cloud Drive資料夾。
1. Select與Workfront專案相關聯的單一檔案或資料夾。
1. 以滑鼠右鍵按一下專案，然後選取&#x200B;**在Workfront中開啟**。

   您的瀏覽器會開啟對應的Workfront位置。 如果出現提示，請以可存取該專案的帳戶登入。

### 從同步活動開啟專案

1. Select功能表列(Mac)或系統匣(Windows)中的Adobe雲端磁碟機圖示。
1. 展開同步活動區段。
1. 針對符合條件的已完成且未刪除的專案，請開啟[更多動作]功能表，然後選取[在Workfront中開啟] ****。
1. 對於透過直接上傳上傳上傳的檔案，在&#x200B;**直接上傳**&#x200B;區段中對其已完成的專案使用相同的動作。

### 關於Workfront中Open的須知事項

* Select一次只能一個專案。 不支援在Workfront中開啟多個選取的專案。
* 在「檔案總管」中，對於Adobe Cloud Drive資料夾之外的專案以及磁碟機根目錄本身，命令是隱藏的。 選取多個專案時，此功能就會停用。
* 專案必須有相對應的Workfront位置。 某些資料夾或其他專案可能沒有Workfront對應，即使它們在Adobe Cloud Drive中可見。
* 尚未完成上傳的新本機專案可能還沒有Workfront連結。 請等候上傳完成，然後再試一次。
* 在一般同步活動中，此動作僅提供給合格的已完成專案。 未提供作用中、失敗或刪除的專案使用。
* 在直接上傳中，動作是針對已完成的上傳提供，而非針對已排入佇列、上傳、失敗或已取消的專案。
* 您必須登入Adobe Cloud Drive。 Workfront可能會要求您另外在瀏覽器中登入，但您的Workfront許可權仍適用。
* 您需要網際網路連線來擷取未快取的連結，並存取Workfront。 先前解析的連結不會提供對Workfront的離線存取。
* 此動作會在瀏覽器中開啟Workfront。 它不會在其案頭應用程式中開啟檔案、上傳另一個復本，或變更其本機離線可用性。

### 在Workfront可用性中開啟

| 專案或狀態 | 在Workfront行為中開啟 | 該做什麼 |
| --- | --- | --- |
| Adobe Cloud Drive中的單一合格專案 | 開啟對應的Workfront位置。 | Select **在Workfront**&#x200B;中開啟。 |
| 多個選取的專案 | 不支援開啟多個專案。 檔案總管會停用此指令。 | Select單一專案。 |
| 新專案仍在上傳 | Workfront連結可能還無法使用。 | 請等候上傳完成，然後再試一次。 |
| 已完成一般同步處理專案 | 當專案符合資格且尚未刪除時可用。 | 使用專案的更多動作功能表。 |
| 已完成直接上傳專案 | 上傳完成後可用。 | 使用專案的更多動作功能表。 |
| 沒有Workfront對應的專案 | 訊息會指出該專案在Workfront中無法使用。 | 直接在Workfront中檢查專案，或選擇其他支援的專案。 |
| 已刪除normal-sync專案 | 動作無法使用。 | 如果您需要調查已刪除的專案，請直接使用Workfront。 |

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

