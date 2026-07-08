---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: 疑難排解Adobe Cloud Drive
description: 檢閱Mac和Windows上Adobe Cloud Drive的限制、效能考量事項，以及常見問題的解決方案。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 6ad89f8d00dd3a06eb160863c3213a9f80b1a44b
workflow-type: tm+mt
source-wordcount: 928
ht-degree: 0%

---

# 疑難排解Adobe Cloud Drive

本文說明Adobe Cloud Drive的限制、請記得的效能考量事項，以及您可能會遇到的常見問題的解決方案。

如需使用Adobe Cloud Drive的詳細資訊，請參閱[使用Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)。

## 限制

### 檔案和資料夾作業

* 專案資料夾的最上層為唯讀。 您無法從Adobe Cloud Drive重新命名、刪除或移動這些專案。 若要建立、重新命名或刪除專案，請使用Workfront網頁介面。
* 完全支援專案資料夾內的檔案和資料夾作業。

### 檔案和路徑限制

* 檔案名稱在任何平台上不得超過255個字元。
* 完整檔案路徑（所有資料夾名稱加上檔案名稱）不能超過1024個字元。 路徑長度超過此限制的檔案不會出現在Adobe Cloud Drive中，即使在Workfront Web介面中可看到這些檔案亦然。
* 如果您在檔案上看到&#x200B;**完整路徑太長**&#x200B;錯誤，請縮短資料夾名稱或減少資料夾巢狀深度，以將路徑置於限制之內。

### 儲存空間

* 儲存在Adobe Cloud Drive本機中的檔案會使用裝置上的磁碟空間。
* 僅限雲端的檔案不使用本機儲存空間。
* 移除您不再需要之檔案的離線存取權。 如需詳細資訊，請參閱[使用Adobe雲端磁碟機](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)中的[移除離線存取以釋放空間](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#remove-offline-access-to-free-up-space)。

## 效能考量事項

* **檔案大小：**&#x200B;同步所需的時間取決於檔案大小。 大型檔案通常需要較長的時間。
* **網路速度：**&#x200B;更快的連線可提供更好的同步效能。 同步會在中斷後自動繼續。
* **首次存取：**&#x200B;檔案在您第一次存取時會隨選下載。 後續存取的速度較快，因為檔案是快取在本機。

## 常見問題

### Adobe Cloud Drive未出現

**可能的原因：**

* 未安裝Adobe Cloud Drive。
* 安裝未順利完成。
* 您的組織未使用支援Adobe雲端儲存空間的Workfront版本。

**解決方案：**

* 確認已安裝Adobe Cloud Drive。 檢查&#x200B;**應用程式** (Mac)或&#x200B;**程式** (Windows)。
* 手動啟動Adobe Cloud Drive。
* 請聯絡您的Workfront管理員，確認您的組織使用支援Adobe雲端儲存空間的Workfront版本。
* 如有需要，請重新安裝Adobe Cloud Drive。 如需詳細資訊，請參閱[安裝Adobe雲端磁碟機](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)。

### 功能表列或工作列未顯示Adobe Cloud Drive圖示

**可能的原因：**

* 功能表列(Mac)或系統匣(Windows)的空間不足，無法顯示圖示。

**解決方案：**

* **Mac：**&#x200B;按住Cmd並拖曳現有的功能表列圖示，重新排列或移除它們，為Adobe Cloud Drive圖示建立空間。
* **Windows：**&#x200B;按一下工作列中的向上箭頭（**顯示隱藏圖示**）來尋找Adobe Cloud Drive圖示，然後將其拖曳到可見區域。

### 未顯示專案，或缺少部分專案

**可能的原因：**

* 您無權存取任何專案。
* 同步處理尚未完成。
* 您有網路連線問題。

**解決方案：**

* 在Workfront網頁介面中驗證您的專案存取權。
* 檢查您的網路連線。
* 登出Adobe Cloud Drive並重新登入。

### 檔案未同步

**可能的原因：**

* 您有網路連線問題。
* 檔案或資料夾發生同步處理錯誤。
* 您的磁碟空間不足。

**解決方案：**

* 檢查您的網際網路連線。
* 確認您有足夠的可用磁碟空間。
* 檢查檔案狀態指示器是否有同步錯誤。 如需詳細資訊，請參閱[使用Adobe雲端磁碟機](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)中的[檔案狀態指示器](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#file-status-indicators)。
* 重新啟動Adobe Cloud Drive。
* 在系統匣或功能表列(Mac)中檢查Adobe Cloud Drive狀態。

### 無法開啟檔案

**可能的原因：**

* 檔案是僅限雲端的，下載失敗。
* 未安裝開啟檔案所需的應用程式。
* 檔案已損毀。

**解決方案：**

* 檢查檔案狀態指示器。
* 請確定已安裝所需的應用程式。
* 用滑鼠右鍵按一下檔案，選取&#x200B;**永遠保留在此裝置上**，然後再次嘗試開啟。
* 確認Workfront網頁介面中的檔案未損毀。

### 同步處理緩慢

**可能的原因：**

* 檔案很大。
* 您的網路連線速度緩慢。
* 許多檔案同時進行同步。

**解決方案：**

* 對大型檔案請耐心等候。 同步可以恢復，因此會在中斷後從中斷的位置恢復。
* 檢查您的網路速度。
* 限制同時進行檔案作業的數目。
* 除非您需要離線存取，否則僅將大型檔案保留在雲端。

### 離線檔案佔用太多空間

**解決方案：**

* 用滑鼠右鍵按一下離線檔案，然後選取&#x200B;**釋放空間**。
* 請定期檢查您的磁碟空間。
* 保留您極少以雲端模式存取的大型檔案。

### 您無法建立、編輯或刪除檔案或資料夾

**可能的原因：**

* 您正在嘗試建立、重新命名或刪除專案資料夾。 專案資料夾的最上層為唯讀。
* 專案是唯讀的，因此您無法在其內建立、編輯或刪除檔案或資料夾。

**解決方案：**

* 若要建立、重新命名或刪除專案，請使用Workfront網頁介面。
* 要求專案所有者與您共用專案，並擁有編輯存取權。

## 取得協助

如有授權問題、專案存取問題或組織專屬設定，請聯絡您的Workfront管理員。

若要與Adobe支援共用記錄檔，請依照[執行Adobe記錄收集器工具](https://helpx.adobe.com/creative-cloud/apps/troubleshoot/diagnostics-repair-tools/run-log-collector-tool.html)中的步驟操作。

## 最佳做法

* **計畫離線工作。** 在旅行或在連線不佳的地區工作之前先下載檔案。
* **監視器同步處理狀態。** 關閉應用程式之前，請先檢查檔案指示器。
* **依照專案的資料夾結構進行。** 依照專案所有者的意圖，組織專案資料夾中的檔案。
* **使用描述性檔案名稱。** 協助您的團隊成員找到他們需要的內容。
* **避免建立重複專案。** 請勿複製不必要的檔案。
