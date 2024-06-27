---
title: 'Adobe Workfront Planning AI Assistant概觀'
description: 您可以使用AI輔助程式，根據目前頁面內容和記錄結構來產生、更新或移除記錄。 使用者的命令和AI對這些命令的執行會共同運作，以確保AI所做的變更正確地反映在您的環境中。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 64f187ed78b69db9b9ac0259e96ef0bf47abf4f4
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---


# Adobe Workfront Planning AI Assistant概觀

<!-- update TOC and miniTOC when making this live-->

>[!IMPORTANT]
>
>本文資訊請參考Adobe Workfront規劃和AI助理，這些都是Adobe Workfront的新產品。
>
>目前Workfront規劃和AI助理都處於搶先使用階段，只有少數客戶可以存取。
>
>您必須是Workfront客戶才能使用這些功能。
>
>如果您屬於此階段，您的客戶代表將會通知您。
>
>如需詳細資訊，請參閱 [Adobe Workfront規劃概觀](/help/quicksilver/planning/general/planning-overview.md).

您可以使用AI輔助程式，根據目前頁面內容和記錄結構來產生、更新或移除記錄。

使用者的命令和AI對這些命令的執行會共同運作，以確保AI所做的變更正確地反映在您的環境中。

## AI助理的考量事項

* 預設情況下，Workfront管理員可以使用AI助理。

* Workfront管理員必須為所有其他使用者啟用AI助理。 如需詳細資訊，請參閱 [啟用或停用AI助理](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* AI助理會在每個頁面的內容中運作。 您為AI助理提交的請求必須參考您開啟的頁面中可用的功能。

* AI助理所執行的動作會在您的Workfront Planning許可權和Workfront存取層級的內容中進行。 如需詳細資訊，請參閱下列文章：

   * [在Adobe Workfront Planning中共用許可權的概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)

* AI助理員代表使用者所做的變更會在紀錄的紀錄面板中進行追蹤。

* 您可以使用命令來復原動作。

## 目前可用於AI助理的功能

目前，AI助理可在Workfront的「規劃」區域中用於下列頁面：

* 記錄型別頁面
* 記錄頁面

此時您可以使用AI助理執行下列動作：

* 建立記錄。 含有新記錄連結的ID會在建立記錄後顯示。
* 根據您上傳的檔案建立記錄。 Workfront支援下列AI助理檔案格式：

  .pptx、.pdf、.docx、.xlsx、.ppt、.doc、.txt和大部分的影像格式
* 更新您在畫面上看到的記錄欄位
* 刪除記錄
* 還原您剛剛刪除的記錄

## 存取AI助理

1. 登入Workfront，然後前往 **規劃** 區域。

1. 按一下 **工作區卡片** > **記錄型別卡片**.

1. （選用）按一下 **記錄** 以開啟記錄的 **詳細資料** 頁面。

1. 按一下 **AI助理圖示** 全域導覽列中熒幕右上角的「 」。

   ![](assets/ai-assistant-icon-highlighted.png)

1. 在提供的空間中，開始輸入AI助理的命令，然後在完成時按一下Enter。

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   例如，您可以鍵入下列其中一項：

   * 建立記錄
   * 更新夏季行銷活動記錄的「說明」欄位，日期待定
   * 刪除最後一個記錄
   * 還原記錄

   AI助理處理命令時會顯示視覺指示器，設定回應時間的預期。

   收到成功回應後，請遵循提供的連結或注意左側的變更。
