---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 接收 [!DNL Adobe Workfront] 中的通知 [!DNL Slack]
description: 接收 [!DNL Adobe Workfront] 中的通知 [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 6%

---

# 接收 [!DNL Adobe Workfront] 中的通知 [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

安裝之後 [!DNL Adobe Workfront for Slack]，您可以 [!DNL Workfront] 中的通知 [!DNL Slack].\
如需關於安裝的資訊 [!DNL Workfront for Slack]，請參閱 [設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

您可以啟用所選數目 [!UICONTROL 通知] 出現在中通知泡泡圖示的 [!DNL Workfront] 介面，亦將於下列位置傳送： [!DNL Slack].

電子郵件通知獨立於下列專案運作： [!DNL Workfront] 介面通知。 您或您的 [!DNL Workfront] 管理員可以停用電子郵件通知，而介面通知則無法在中停用 [!DNL Workfront].\
不過，您可以停用 [!DNL Workfront] 您可能會在中收到的通知 [!DNL Slack]，如果您只想在 [!DNL Workfront] 介面。

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
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。\

## 必要條件

接收之前 [!DNL Workfront] 中的通知 [!DNL Slack]，您必須

* 設定 [!DNL Workfront for Slack]\
   有關設定的指示 [!DNL Workfront for Slack]，請參閱 [設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 設定 [!DNL Workfront] 以下專案的通知 [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. （視條件而定）晚於 [!DNL Workfront] 已新增至您的 [!DNL Slack] 執行個體，登入 [!DNL Workfront] 從 [!DNL Slack].\
   有關登入的資訊 [!DNL Workfront] 從 [!DNL Slack]，請參閱 [存取 [!DNL Adobe Workfront] 從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 從任何頻道，開始在訊息欄位中輸入以下命令之一：

   `/workfront settings`

   或

   `/wf settings`

1. 預設會啟用所有通知。\
   停用下列任何通知：

   * [!UICONTROL 我被指派到一個新任務或問題]
   * [!UICONTROL 我的團隊已指派至新任務或問題]
   * [!UICONTROL 我收到新的核准或存取要求]
   * [!UICONTROL 有人將我加入定向更新]
   * [!UICONTROL 有人在我參與的討論串中發表評論]
   * [!UICONTROL 我所訂閱的任務、問題或專案已有更新]
   * [!UICONTROL 有人對我其中一個工作項目發表評論]
   * [!UICONTROL 有人對我的說明請求發表評論]

   您對進行的變更 [!UICONTROL 通知] 選項會立即生效。\
   您啟用的通知會傳送至 [!DNL Workfront] [!DNL Slack] 頻道。 當您在此停用通知時，只會針對以下專案停用通知： [!DNL Slack]，而非 [!DNL Workfront] 介面。 您會繼續在 [!DNL Workfront] 通知泡泡在介面的右上角。

## 管理 [!DNL Workfront] 通知來源 [!DNL Slack]

您可以接收並回應 [!DNL Workfront] 通知來源 [!DNL Slack].

您可以針對在中啟用的通知停用電子郵件通知 [!DNL Slack]，以確保您不會收到重複的通知。\
如需有關設定電子郵件通知的資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

啟用或停用 [!DNL Workfront] 中的通知 [!DNL Slack] 不會影響您在內收到的通知 [!DNL Workfront] 介面。\
內的通知 [!DNL Workfront] 無法停用介面。

若要管理您的 [!DNL Workfront] 以下專案的通知 [!DNL Slack]：

1. 登入 [!UICONTROL Slack].
1. 登入 [!DNL Workfront] 從 [!DNL Slack].\
   有關登入的資訊 [!DNL Workfront] 從 [!DNL Slack]，請參閱 [!DNL Workfront] 從 [!DNL Slack]中的「 」區段 [存取 [!DNL Adobe Workfront] 從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 確保您的 [!DNL Workfront] 以下專案的通知 [!DNL Slack] 已啟用。\
   如需關於哪些專案的詳細資訊， [!DNL Workfront] 通知可設定為也傳送至 [!DNL Slack]，請參閱 [設定 [!DNL Workfront] 以下專案的通知 [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. 前往 **[!DNL Workfront]** 尋找您的頻道 [!DNL Workfront] 通知。
1. （條件式與選擇式）執行下列任一項作業：

   * 按一下 **[!UICONTROL 處理它]** 以接受處理任務。

   * （條件式與選擇式）按一下 **[!UICONTROL 回覆[!DNL Workfront]]** 若要回複評論，請輸入您的回覆，然後按一下 **[!UICONTROL 回覆]**.

   * （條件式與選擇式）按一下 **[!UICONTROL 核准]** 或 **[!UICONTROL 拒絕]** 核准或拒絕擱置核准的任務、問題或專案。

   * （條件式與選擇式）按一下 **[!UICONTROL 核准]**， **[!UICONTROL 變更]**，或 **[!UICONTROL 拒絕]**，以核准、核准變更，或拒絕檔案。

     您也可以將滑鼠移到檔案的縮圖上，然後按一下放大鏡圖示，在核准檔案之前檢視檔案的較大預覽。\
      僅限已核准的Slack [檔案型別](https://api.slack.com/types/file) 可預覽。

   * （條件式與選擇式）按一下 **[!UICONTROL 授予]** 或 **[!UICONTROL 忽略]** 以授與或忽略其他使用者對更多存取權的要求。\

     您會收到一則確認訊息，確認您的動作已完成，於 [!DNL Workfront]，適用於您在通知中作出的每個決定。
