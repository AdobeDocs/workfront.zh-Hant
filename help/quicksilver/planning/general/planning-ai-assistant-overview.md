---
title: Adobe Workfront Planning AI助理概觀
description: 您可以使用AI輔助程式，根據目前頁面內容和記錄結構來產生、更新或移除記錄。 使用者的命令和AI對這些命令的執行會共同運作，以確保AI所做的變更正確地反映在您的環境中。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 0%

---


# Adobe Workfront Planning AI Assistant概觀

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

您可以使用「AI輔助程式」，根據目前頁面內容和記錄結構來產生、更新或移除記錄。

使用者的命令和AI對這些命令的執行會共同運作，以確保AI所做的變更正確地反映在您的環境中。

## AI助理的考量事項

* AI助理必須先為貴組織啟用，才能供貴公司的使用者使用。 如需詳細資訊，請參閱[AI助理概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。
* Workfront為貴組織啟用AI助理後，即可供Workfront主要管理員使用。 如需詳細資訊，請參閱[設定您系統的基本資訊](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

* Workfront管理員必須為所有其他使用者啟用AI助理。 如需詳細資訊，請參閱[啟用或停用AI助理](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

* AI助理會在每個頁面的內容中運作。 您為AI助理提交的請求必須參考您開啟的頁面中可用的功能。

* AI助理在「計畫」區域中執行的動作會根據您的Workfront Planning許可權和Workfront存取層級來設定。 如需詳細資訊，請參閱下列文章：

   * [在Adobe Workfront Planning中共用許可權的概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)

* AI助理員代表使用者所做的變更會在紀錄的紀錄面板中進行追蹤。

* 您可以使用命令來復原動作。 例如，您可以輸入「復原上次變更」來回覆變更。

* <span class="preview">透過AI助理建立、更新或刪除物件時，AI助理會顯示預期的動作並要求確認。 之後，您可以確認或取消動作。</span>

## 目前可用於AI助理的功能

目前，AI助理可在Workfront的「規劃」區域中用於下列頁面：

* Workspace頁面
* 記錄型別頁面
* 記錄頁面

此時您可以使用AI助理執行下列動作：

* 搜尋記錄。 您可以依據任何記錄欄位中包含的資訊進行搜尋。
* 建立記錄。 含有新記錄連結的ID會在建立記錄後顯示。 您可以指定要在建立過程中更新的欄位，例如日期或說明。
* 根據您上傳的檔案建立記錄。 Workfront支援下列AI助理檔案格式：

  PPTX、PDF、DOCX、XLSX、PPT、DOC、TXT和大部分影像格式
* 更新您在畫面上看到的記錄欄位
* 刪除記錄
* 還原您剛剛刪除的記錄


## 在Workfront Planning中找到AI助理

您可以在Workfront Planning的下列區域中找到AI助理：

* 熒幕右上角的主要導覽列。
* 在記錄的詳細資訊區域中，在預覽中開啟記錄之後或開啟記錄的頁面之後。

## 存取「規劃」區域的AI助理

1. 登入Workfront，然後按一下熒幕右上角的&#x200B;**主功能表**&#x200B;圖示![點主功能表](assets/dots-main-menu.png)，或左上角的&#x200B;**主功能表**&#x200B;圖示![行主功能表](assets/lines-main-menu.png) （若有）。

。按一下&#x200B;**計畫**。 「規劃」區域隨即開啟。

1. 按一下&#x200B;**工作區卡片**。

1. （選擇性）按一下&#x200B;**記錄型別卡片**。

1. （選擇性）按一下&#x200B;**記錄**&#x200B;以開啟記錄的&#x200B;**詳細資料**&#x200B;頁面。

1. 按一下全域導覽列中熒幕右上角或記錄預覽或頁面右上角的&#x200B;**AI助理圖示**。

   ![AI助理圖示](assets/ai-assistant-icon-highlighted.png)

1. 在提供的空間中，開始輸入AI助理的命令，然後在完成時按一下Enter。

   ![具有空白命令方塊的AI助理面板](assets/ai-assistant-panel-with-empty-command-box.png)

   例如，您可以鍵入下列其中一項：

   * 建立開始日期為7月4日、結束日期為7月30日的行銷活動
   * 更新夏季行銷活動記錄的「說明」欄位，日期待定
   * 刪除最後一個記錄
   * 還原記錄

   AI助理處理命令時會顯示視覺指示器，設定回應時間的預期。

   收到成功回應後，請遵循提供的連結或注意左側的變更。



