---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 從 [!DNL Adobe Workfront] 存取 [!DNL Slack]
description: 整合 [!DNL Adobe Workfront] 與 [!DNL Slack] 可讓您從Slack存取 [!DNL Workfront] ，或在 [!DNL Workfront] 中使用斜線命令執行某些動作。 整合可從任何 [!DNL Slack] 環境使用，包括 [!DNL Slack] 行動應用程式。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 1%

---

# 從[!DNL Adobe Workfront]存取[!DNL Slack]

將[!DNL Adobe Workfront]與[!DNL Slack]整合可讓您從[!DNL Workfront]存取[!DNL Slack]，或使用斜線命令在[!DNL Workfront]中執行某些動作。 整合可從任何[!DNL Slack]環境使用，包括[!DNL Slack]行動應用程式。

您或您的[!DNL Slack]管理員必須在您的[!DNL Workfront]執行個體中安裝[!DNL Slack]應用程式，才能使用[!DNL Workfront]的[!DNL Slack]。 如需詳細資訊，請參閱[為Slack設定Adobe Workfront](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>任何</p>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 關於斜線指令 {#about-slash-commands}

使用[!DNL Slack]時，您會在訊息欄位中輸入訊息。 當您以斜線啟動訊息時，它會變成命令，而且其行為與簡單訊息不同。 命令會通知[!DNL Slack]執行動作。

您可以在任何[!DNL Workfront]頻道中輸入斜線命令，以從[!DNL Slack]存取您的[!DNL Slack]執行個體。

在[!DNL Slack]中使用斜線命令存取[!DNL Workfront]時，請記住下列事項：

* 斜線指令區分大小寫。
* [!DNL Workfront]的命令只對您可見，無論您在哪個管道輸入它們。
* 命令應該一律以`/workfront`或`/wf`開頭，後面接著空格和您要在[!DNL Workfront]中執行的動作名稱。

  這表示您的命令適用於[!DNL Workfront]應用程式。 [!DNL Workfront]的命令只有在您已使用您的[!DNL Workfront]執行個體設定[!DNL Slack]應用程式時才有效。

如需可從Slack為[!DNL Workfront]執行的所有命令清單，請參閱[中的 [!DNL Workfront] Access [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack)slash命令。

## 從[!DNL Workfront]登入[!DNL Slack] {#log-in-to-workfront-from-slack}

當您在Slack的訊息欄位中輸入任何命令時，系統會要求您先登入[!DNL Workfront]。\
如需來自[!DNL Workfront]的[!DNL Slack]命令的完整清單，請參閱本文章節[中的 [!DNL Workfront] Access [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack)from a slash命令。

若要從[!DNL Workfront]登入[!DNL Slack]：

1. 登入您的[!DNL Slack]執行個體。
1. 從任何色版中，鍵入下列指令之一：\
   `/workfront log in`

   或

   `/wf log in`

1. 按一下回應中顯示的[!DNL Workfront] **[!UICONTROL 登入]**&#x200B;連結。\
   新標籤隨即開啟，其中包含[!DNL Workfront]認證的欄位。

1. 依照提示使用Enhanced Authentication、OAuth 2.0或您的安全性宣告標籤語言(SAML) URL登入[!DNL Workfront]。

   >[!NOTE]
   >
   >* 當系統提示您輸入[!DNL Workfront]帳戶的主機時，請使用下列格式輸入該主機： *yourCompany&#39;sDomain.my.workfront.com*。 您公司的網域通常是您公司的名稱。
   >* 增強式驗證必須由[!DNL Workfront]系統管理員針對這項整合啟用才能使用。


   [!DNL Workfront]中[!DNL Slack]個通知的設定頁面隨即開啟。

1. （選用）停用您不想在[!DNL Workfront]中接收的任何[!DNL Slack]通知。

   如需有關為[!DNL Workfront]設定[!DNL Slack]設定的資訊，請參閱本文章的[設定設定](#configure-settings-configure-settings)一節

1. 導覽回您的[!DNL Slack]頻道。

   您已從您的[!DNL Workfront]執行個體登入[!DNL Slack]。

## 從[!DNL Workfront]存取[!DNL Slack]

* [關於斜線指令](#about-slash-commands-about-slash-commands)
* [從 [!DNL Workfront] 中的共用連結存取 [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## 從[!DNL Workfront]中的斜線命令存取[!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. 登入您的[!DNL Slack]執行個體並從[!DNL Workfront]登入[!DNL Slack]。\
   如需有關從[!DNL Workfront]登入[!DNL Slack]的詳細資訊，請參閱[從 [!DNL Workfront] 登入 [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. 從任何通道中，開始在訊息欄位中輸入以下命令：

   `/workfront help`

   或

   `/wf help`

1. 從下列命令中選取：

   * `/wf home`

     顯示您可以存取任務、問題和核准清單的按鈕。 按一下其中一個按鈕會顯示[!DNL Slack]中每個清單的前20個專案。

     如需有關從[!DNL Workfront]管理[!DNL Slack]個工作專案的詳細資訊，請參閱[從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)管理您的工作和核准。

   * `/wf add task <TaskName>`

     包含將顯示在[!DNL Workfront]介面中的工作名稱。

     將工作新增至[!DNL Workfront]。

     如需有關從Slack新增任務到[!DNL Workfront]的詳細資訊，請參閱[!DNL Slack]從[建立任務和問題中的「從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md)建立任務」一節。

   * `/wf add issue <Issue Name>`

     包含將顯示在[!DNL Workfront]介面中的問題名稱。

     新增問題至[!DNL Workfront]

     如需有關從[!DNL Workfront]新增問題到[!DNL Slack]的詳細資訊，請參閱[!DNL Slack]從[建立任務和問題中的「從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md)建立問題」一節。

   * `/wf favorites`

     顯示[!DNL Workfront]我的最愛清單。

     如需有關從[!DNL Slack]存取您的最愛的相關資訊，請參閱[存取您的最愛和最近專案[!UICONTROL 文章中的]從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites)存取您的[我的最愛 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md)清單區段。

   * `/wf recent`

     顯示[!DNL Workfront]中最近存取專案的清單。

     如需有關從[!DNL Slack]存取您最近專案的詳細資訊，請參閱[從[!UICONTROL 存取您的]最近專案 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] 清單和從[!UICONTROL 存取最近專案 [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md)。

   * `wf tasks`

     顯示工作清單。

     如需有關從[!DNL Slack]管理您的任務的詳細資訊，請參閱[!DNL Slack]從[管理您的工作和核准 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)中的「管理您的任務」一節。

   * `/wf issues`

     顯示問題清單。

     如需有關從[!DNL Slack]管理您的問題的詳細資訊，請參閱[!DNL Slack]從[管理您的工作和核准中的「從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)管理您的問題」一節。

   * `/wf approvals`顯示您的[!DNL Workfront]核准。\

     如需有關從[!DNL Slack]管理您的核准的詳細資訊，請參閱[!DNL Slack]從[管理您的工作和核准中的「從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md)管理您的核准」一節。

   * `/wf search <keyword>`

     包含關鍵字。

     搜尋特定關鍵字。 您可以搜尋下列型別物件：

      * 專案
      * 任務
      * 問題
      * 報表
      * 人員
      * 範本
      * 文件
      * 產品組合
      * 方案
      * 控制面板
      * 公司
      * 注意\

        如需在[!DNL Slack]中搜尋的詳細資訊，請參閱[從Slack [!DNL Adobe Workfront] 搜尋](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md)專案。
   * `/wf log in`

     從[!DNL Workfront]將您登入[!DNL Slack]。

   * `/wf log out`

     從[!DNL Workfront]將您登出[!DNL Slack]。 如果您在另一個應用程式的另一個瀏覽器標籤中開啟了單獨的[!DNL Workfront]執行個體，則您仍會登入[!DNL Workfront]。
   * `/wf settings`

     可讓您在[!DNL Workfront]中設定[!DNL Slack]設定。

     如需有關在Slack中設定[!DNL Workfront]設定的資訊，請參閱[設定設定](#configure-settings-configure-settings)。

   * `/wf help`
顯示[!DNL Workfront]的完整命令清單。


   * `Visit Workfront Help`：在新的瀏覽器分頁中開啟[!UICONTROL 說明網站上的]Slack[!DNL Workfront]區段。


1. （選擇性）若要刪除任何命令的訊息，請將滑鼠移至包含該命令的Slack訊息的右上角，然後按一下&#x200B;**[!UICONTROL 顯示訊息動作]**，然後按一下&#x200B;**[!UICONTROL 刪除訊息]**。

1. （選擇性和條件性）按一下&#x200B;**[!UICONTROL 刪除]**&#x200B;以確認您要刪除此訊息。

### 從[!DNL Workfront]中的共用連結存取[!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

您可以透過連結存取[!DNL Workfront]物件，這些連結會連結到[!DNL Slack]中與您共用的物件。

如需從共用連結存取[!DNL Workfront]的詳細資訊，請參閱[中的 [!DNL Adobe Workfront] 從共用連結存取 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md)物件。

## 進行設定 {#configure-settings}

1. 在[!DNL Slack]訊息欄位內，輸入下列命令：

   `/workfront settings`

   或

   `/wf settings`

   預設會啟用所有設定。

1. 取消選取下列選項，即可停用Workfront的設定：

   * 在&#x200B;**[!UICONTROL 一般設定]**&#x200B;區域中，停用&#x200B;**[!UICONTROL 在[!DNL Workfront]頻道中貼上[!DNL Slack] URL時，如果不想讓]**&#x200B;在您共用[!DNL Slack]Slack[!DNL Workfront]中物件的URL時新增關於您的[!UICONTROL 物件的其他資訊，請顯示額外的說明、到期日或要求者名稱]&#x200B;設定。

   * 在&#x200B;**[!UICONTROL 通知設定]**&#x200B;區域中，停用您要停止從Workfront接收的通知。\

     如需有關在[!DNL Workfront]接收[!DNL Slack]通知的資訊，請參閱[中的 [!DNL Adobe Workfront] 接收 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md)通知。

## 從[!DNL Workfront]登出[!DNL Slack]

1. 在[!DNL Slack]訊息欄位內，輸入下列命令：\
   `/workfront log out`或\
   `/wf log out`\
   您會收到一則訊息，確認您已登出[!DNL Workfront]。\
   如果您在另一個應用程式的另一個瀏覽器標籤中開啟了單獨的[!DNL Workfront]執行個體，則您仍會登入[!DNL Workfront]。
