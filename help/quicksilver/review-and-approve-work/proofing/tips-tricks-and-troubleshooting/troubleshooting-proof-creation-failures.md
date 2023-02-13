---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: 疑難排解校樣建立失敗
description: 校樣建立過程包括導入和校樣生成。 在建立校樣時，有時會無法匯入檔案，或在匯入檔案後無法產生校樣。
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# 疑難排解校樣建立失敗

校樣建立過程包括導入和校樣生成。 在建立校樣時，有時會無法匯入檔案，或在匯入檔案後無法產生校樣。

>[!NOTE]
>
> 如果您嘗試證明的檔案不符合本節所列的任何標準，請聯絡Adobe Workfront支援以進行進一步調查。

## 匯入失敗的原因

* 您已建立包含50多個檔案的合併校樣。

## 證明生成失敗的原因

* 不支援檔案類型。\
   如需支援的檔案類型清單，請參閱 [支援的校對檔案類型和大小限制概觀](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* 檔案結構是檔案類型的非標準結構。
* 檔案受密碼保護，或內容複製已禁用。

   與其他類型的檔案不同，如果PDF上的內容複製安全設定設為「允許」，則PDF檔案可以生成為校樣。

* 頁面長度或頁數超過限制。

   光柵化後允許的最大頁面長度為195英吋；單一校樣的允許頁數上限為1,000頁。

* 檔案損壞或損壞。
* 新校樣版本的工作流程截止日期已過去。

   當您使用快速校樣方法建立新校樣版本時，就會發生此情況。 **上傳檔案時自動產生校樣** 中所有規則的URL。 新的校樣版本會嘗試從先前產生的校樣中取得工作流程的截止日期。 如果過去是這些期限，則證明生成失敗。 若要補救此問題，您可以在未來將工作流程截止日期設定為舊版，或產生新的校樣版本。 如果您產生新版本，請使用 **更多>新版本>校樣** 選取 **未來的工作流截止時間**.

* 校樣PDF檔案時，校樣產生失敗的原因包括：

   * 字型和影像從外部源（例如從本地檔案系統）連結

      字型和影像必須嵌入PDF檔案，才能在其他電腦或Workfront Proof內顯示。

   * 您的PDF檔案包含空圖層或透明或重疊的欄位。

      如果無法確定導致此情況的層或對象，請將設計/文檔導出為優化PDF（這會刪除所有不需要的元素）。

