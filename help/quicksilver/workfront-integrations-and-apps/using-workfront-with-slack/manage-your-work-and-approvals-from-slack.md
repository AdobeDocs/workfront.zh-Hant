---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: 從Slack管理您的工作和核准
description: 您可以存取首頁工作清單、檢閱並同意處理任務和問題，以及直接從Slack檢閱或決定核准。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 1%

---

# 從[!DNL Slack]管理您的工作和核准

安裝[!DNL Adobe Workfront for Slack]之後，您可以執行下列動作：

* 從[!DNL Slack]存取您的[!UICONTROL 首頁]專案清單
* 檢閱並接受來自[!DNL Slack]的任務和問題工作
* 檢閱並決定來自[!DNL Slack]的核准

如需使用[!DNL Slack]設定[!DNL Workfront]的詳細資訊，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront]計畫</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 先決條件

在您可以從[!DNL Slack]管理您的工作和核准之前，您必須

* 設定[!DNL Workfront for Slack]\
  如需設定[!DNL Workfront for Slack]的說明，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 從[!DNL Slack]管理您的工作

1. 登入您的[!DNL Slack]執行個體並從[!DNL Slack]登入[!DNL Workfront]。\
   如需有關從[!DNL Slack]登入[!DNL Workfront]的詳細資訊，請參閱[Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的「從[!DNL Slack]登入[!DNL Workfront]」區段。

1. 從任何通道中，開始在訊息欄位中輸入以下命令：

   `/workfront home`

   >[!NOTE]
   >
   >* 命令區分大小寫。
   >* 您可以使用`/wf`來啟動命令，而非`/workfront`。

   您可從其中存取任務、問題和核准清單的按鈕隨即顯示。 按一下其中一個按鈕會顯示[!DNL Slack]中每個清單的前20個專案。

1. （選擇性）按一下&#x200B;**[!UICONTROL 工作]**&#x200B;以顯示您的所有工作。

   如需有關在[!DNL Slack]中管理工作的詳細資訊，請參閱[從 [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack)管理您的工作。

1. （選擇性）按一下「**[!UICONTROL 問題]**」以顯示您的所有問題。

   如需[!DNL Slack]中管理問題的詳細資訊，請參閱[從 [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack)管理您的問題。

1. （選擇性）按一下&#x200B;**[!UICONTROL 核准]**&#x200B;以顯示等待您決定的所有核准。\
   如需在[!DNL Slack]中管理核准的詳細資訊，請參閱[從 [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack)管理您的核准。

## 從[!DNL Slack]管理您的工作 {#manage-your-tasks-from-slack}

1. 登入您的[!DNL Slack]執行個體並從[!DNL Slack]登入[!DNL Workfront]。\
   如需有關從[!DNL Slack]登入[!DNL Workfront]的資訊，請參閱[Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的「從[!DNL Slack]登入[!DNL Workfront]」區段。

1. 從任何頻道，開始在訊息欄位中輸入以下任一命令：

   `/workfront home`，然後按一下&#x200B;**[!UICONTROL 工作]**

   或

   `/workfront tasks`

   >[!NOTE]
   >
   >* 命令區分大小寫。
   >* 您可以使用`/wf`來啟動命令，而非`/workfront`。

   清單上的前20個任務隨即顯示。

1. 按一下&#x200B;**[!UICONTROL +`<remaining number>`其他]**&#x200B;以顯示其他工作。
1. 請考慮檢閱下列有關您工作專案的資訊：

   * **[!UICONTROL 名稱]**
   * **[!UICONTROL 專案名稱]**&#x200B;或&#x200B;**[!DNL Parent Object Name]**

   * 工作專案的&#x200B;**[!DNL Planned Completion Date]**。
   * **[!DNL Assigned By Name]**：這是指派任務給您的使用者名稱。
   * **[!UICONTROL 狀態]**

1. （選用）按一下專案名稱，即可在個別瀏覽器分頁中於Workfront開啟該專案。
1. （選擇性）在&#x200B;**[!UICONTROL 狀態]**&#x200B;欄位中，選取新的狀態。
1. （選擇性）按一下&#x200B;**[!UICONTROL 記錄時間]**，然後選取&#x200B;**[!UICONTROL 小時型別]**&#x200B;和小時量，以記錄專案上的時間。

   >[!NOTE]
   >
   >* 您最多只能以1小時或2小時（12小時30分鐘）為增量來記錄小時。
   >* 您記錄的時數其「輸入日期」為今天。 您無法記錄來自[!DNL Slack]之過去或未來日期的時間。

   您會收到時間已記錄的確認。

1. （選擇性）按一下&#x200B;**[!UICONTROL 處理它]**&#x200B;以接受處理任務。 [!UICONTROL 處理它]按鈕消失。

## 從[!DNL Slack]管理您的問題 {#manage-your-issues-from-slack}

1. 登入您的[!DNL Slack]執行個體並從[!DNL Slack]登入[!DNL Workfront]。\
   如需有關從[!DNL Slack]登入[!DNL Workfront]的詳細資訊，請參閱[從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] 登入 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)。 [!DNL Workfront] 

1. 從任何頻道，開始在訊息欄位中輸入以下任一命令：

   `/workfront home`，然後按一下&#x200B;**[!UICONTROL 問題]**

   或

   `/workfront issues`

   >[!NOTE]
   >
   >* 命令區分大小寫。
   >* 您可以使用`/wf`來啟動命令，而非`/workfront`。

   清單中的前20個問題隨即顯示。

1. 按一下&#x200B;**[!UICONTROL +其他`<number>`個]**&#x200B;以顯示其他專案。
1. 請考慮檢閱下列有關您工作專案的資訊：

   * **[!UICONTROL 名稱]**
   * **[!UICONTROL 專案]**&#x200B;名稱或父系物件名稱
   * **[!UICONTROL 到期日為]**&#x200B;日期：這是工作專案的計畫完成日期。
   * **[!DNL Requested by]**&#x200B;名稱：這是主要連絡人（針對問題）或進行指派的使用者（針對任務）。

1. （選用）按一下問題名稱，以在Workfront的個別瀏覽器標籤中開啟。
1. （選擇性）按一下&#x200B;**[!DNL Work on it]**&#x200B;以開始處理您尚未接受的問題。

   [!UICONTROL 處理它]按鈕消失。

## 從[!DNL Slack]管理您的核准 {#manage-your-approvals-from-slack}

1. 登入您的[!DNL Slack]執行個體並從[!DNL Slack]登入[!DNL Workfront]。\
   如需有關從[!DNL Slack]登入[!DNL Workfront]的詳細資訊，請參閱[Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的「從[!DNL Slack]登入[!DNL Workfront]」區段。

1. 從任何頻道，開始在訊息欄位中輸入以下任一命令：

   `/workfront home`，然後按一下&#x200B;**[!UICONTROL 核准]**

   或

   `/workfront approvals`

   >[!NOTE]
   >
   >* 命令區分大小寫。
   >* 您可以使用`/wf`來啟動命令，而非`/workfront`。

   **[!UICONTROL 核准]**&#x200B;清單上的前20個專案會顯示。 也會顯示有關專案的其他資訊，例如要求專案的使用者名稱或專案所屬的專案名稱。

1. 按一下&#x200B;**[!UICONTROL +其他`<number>`個]**&#x200B;以顯示其他專案。

1. 請考慮管理下列物件的核准：

   * **專案**

     按一下&#x200B;**[!UICONTROL 核准]**&#x200B;或&#x200B;**[!UICONTROL 拒絕]**&#x200B;以接受或拒絕專案狀態變更。

   * **任務**

     按一下&#x200B;**[!UICONTROL 核准]**&#x200B;或&#x200B;**[!UICONTROL 拒絕]**&#x200B;以接受或拒絕工作的狀態變更。

   * **問題**

     按一下&#x200B;**[!UICONTROL 核准]**&#x200B;或&#x200B;**[!DNL Reject]**&#x200B;以接受或拒絕問題的狀態變更。

   * **文件**

     按一下[核准]&#x200B;**核准檔案，**&#x200B;[!UICONTROL &#x200B;拒絕&#x200B;]&#x200B;**拒絕檔案，或**&#x200B;[!UICONTROL &#x200B;變更&#x200B;]&#x200B;**指示您核准檔案，但檔案需要其他變更。**\
     （選擇性）將滑鼠移到檔案縮圖上，按一下放大鏡並預覽檔案。

   * **校訂**&#x200B;按一下校訂名稱，在個別索引標籤的[!DNL Workfront]中開啟並管理核准。
   * **存取要求**

     按一下&#x200B;**[!UICONTROL 授與存取權]**，為要求的物件賦予增強的許可權，或按一下&#x200B;**[!UICONTROL 忽略]**，忽略要求以取得更多存取權。

1. （選擇性）按一下提交核准的物件名稱，在新的瀏覽器分頁中於[!DNL Workfront]開啟它。
