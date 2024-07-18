---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: 疑難排解校訂建立失敗
description: 校樣建立過程包括匯入和校樣產生。 有時候，當您建立校訂時，檔案可能無法匯入，或是在檔案匯入後無法產生校訂。
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# 疑難排解校訂建立失敗

校樣建立過程包括匯入和校樣產生。 有時候，當您建立校訂時，檔案可能無法匯入，或是在檔案匯入後無法產生校訂。

>[!NOTE]
>
> 如果您嘗試校訂的檔案不符合本節所列的任何條件，請聯絡Adobe Workfront支援以進一步調查。

## 匯入失敗的原因

* 您已建立包含50多個檔案的合併校訂。

## 校訂產生失敗的原因

* 不支援該檔案型別。\
  如需支援的檔案型別清單，請參閱[支援的校訂檔案型別和大小限制概觀](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md)。

* 檔案結構是檔案型別的非標準結構。
* 檔案受密碼保護，或已停用內容複製。

  與其他型別的檔案不同，如果PDF上內容複製的安全性設定設為「允許」，則PDF檔案可以產生為校樣。

* 頁面長度或頁數超過限制。

  點陣化後允許的頁面長度上限為195英吋；單一校訂的允許頁面計數上限為1,000頁。

* 檔案已損毀或損毀。
* 新校訂版本的工作流程截止日期是過去。

  當您使用快速校訂方法建立新的校訂版本，並選取&#x200B;**上傳檔案時自動產生校訂**&#x200B;時，就會發生這種情況。 新校訂版本會嘗試從先前產生的校訂中取得工作流程截止日期。 如果這些截止日期已過，則校訂產生失敗。 若要解決此問題，您可以在未來的舊版上設定工作流程截止日期，或產生新的校訂版本。 如果您產生新版本，請使用&#x200B;**更多>新版本>校訂**，並選取未來的&#x200B;**工作流程截止日期**。

* 校訂PDF檔案時，校訂產生失敗的原因包括：

   * 字型和影像是從外部來源連結（例如從您的本機檔案系統）

     字型和影像必須內嵌在PDF檔案中，才能顯示在其他電腦或Workfront Proof中。

   * 您的PDF檔案包含空白圖層或透明或重疊欄位。

     如果您無法判斷是哪個圖層或物件造成這種情況，請將設計/檔案匯出為最佳化PDF（這會移除所有不需要的元素）。

