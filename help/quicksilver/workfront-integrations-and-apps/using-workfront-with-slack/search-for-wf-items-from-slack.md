---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 搜尋 [!DNL Adobe Workfront] 項目自 [!DNL Slack]
description: 您可以搜尋 [!DNL Adobe Workfront] 項目自 [!DNL Slack], if your instance of Slack has had the [!DNL Workfront] 已安裝應用程式。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 6%

---

# 搜尋 [!DNL Adobe Workfront] 項目自 [!DNL Slack]

您可以搜尋 [!DNL Adobe Workfront] 項目自 [!DNL Slack]，若您的例項 [!DNL Slack] 有 [!DNL Workfront] 已安裝應用程式。

如需有關設定的詳細資訊 [!DNL Workfront] with [!DNL Slack]，請參閱 [設定 [!DNL Adobe Workfront] for [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 計劃]</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

搜索之前 [!DNL Workfront] 項目自 [!DNL Slack]，您必須

* 設定 [!DNL Workfront] for [!DNL Slack]\
   配置說明 [!DNL Workfront for Slack]，請參閱 [設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 搜尋 [!DNL Workfront] 項目自 [!DNL Slack]:

1. 登入 [!DNL Slack] 執行個體和登入 [!DNL Workfront] 從 [!DNL Slack].\
   如需登入的詳細資訊，請參閱 [!DNL Workfront] 從 [!DNL Slack]，請參閱「登入」 [!DNL Workfront] 從 [!DNL Slack]「 」部分 [存取 [!DNL Adobe Workfront] 從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 從任何通道，開始在消息欄位中鍵入以下任一命令：

   `/workfront search <keyword>`

   或

   `/wf search <keyword>`

   >[!NOTE]
   >
   >命令區分大小寫。 關鍵字不區分大小寫，並且必須輸入時不帶括弧或雙引號。\
   >![slack_search_result_select_object_box.png](assets/slack-search-result-select-object-box-350x30.png)   >

1. 在顯示的欄位中，從以下欄位中選取物件類型：

   * 專案
   * 任務
   * 問題
   * 報告
   * 人員
   * 範本
   * 文件
   * 專案組合
   * 方案
   * 儀表板
   * 公司
   * 備註

      一次只能選擇一個對象類型。\
      隨即顯示符合搜尋條件的項目清單。

1. 按一下項目名稱以在中開啟 [!DNL Workfront] 中的任何值。
