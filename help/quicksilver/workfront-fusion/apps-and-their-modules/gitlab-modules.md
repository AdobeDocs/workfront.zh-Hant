---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: GitLab模組
description: Adobe Workfront Fusion除了需要Adobe Workfront授權外，還需要Adobe Workfront Fusion授權。
author: Becky
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: d55ddd97a69f00a1f42d84dc55a12d2017855776
workflow-type: tm+mt
source-wordcount: '4370'
ht-degree: 0%

---


# [!UICONTROL GitLab] 模組

Adobe Workfront Fusion除了需要Adobe Workfront授權外，還需要Adobe Workfront Fusion授權。

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!UICONTROL GitLab]，並將其連接至多個協力廠商應用程式和服務。

>[!NOTE]
>
>本文期望您能熟悉API檔案和 [!DNL GitLab] 功能。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Connect [!DNL GitLab] to [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. 在任何 [!DNL Workfront Fusion] [!DNL Gitlab] 模組，按一下 **[!UICONTROL 新增]** 欄位旁邊。
1. 設定下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL連接名]</td> 
      <td> <p>輸入連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>輸入 [!DNL GitLab] 例項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL訪問令牌]</td> 
      <td><p>輸入您的[!UICONTROL專用令牌]或[!UICONTROL個人訪問令牌]。</p><p>如需在中找到或建立個人存取權杖的相關資訊，請參閱 [!DNL GitLab]，請參閱 <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">個人存取權杖</a> 在 [!DNL GitLab] 檔案。</p></td> 
     </tr> 
    </tbody> 
   </table>


1. 按一下 **[!UICONTROL 繼續]**.
1. 按一下 **[!UICONTROL 授權]** 以建立連線並返回模組。

## [!DNL GitLab] 模組及其欄位

設定時 [!DNL GitLab] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL GitLab] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 觸發器

+++**[!UICONTROL 監看組建狀態]**

此即時觸發模組會在組建狀態變更時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>您希望Webhook監看的項目，以查看建置狀態更改</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 觀看提交/MR/問題/片段評論]**

此即時觸發模組會在對提交、合併請求、問題或程式碼片段進行註解時，啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>您希望網頁連結監看的專案以取得意見</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 監看提交（推送）]**

此即時觸發模組會在提交至存放庫時啟動案例。 推送標籤時，此模組不會啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>希望Webhook監視提交項的項目</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch問題評論]**

此即時觸發模組會在對問題發表評論時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>希望Webhook監視問題評論的項目</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 監看問題]**

此 [!UICONTROL 即時觸發] 模組會在建立問題或更新、關閉或重新開啟現有問題時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>您希望網頁連結監看的問題專案</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 監看合併請求]**

此即時觸發模組會在發生下列任一情況時啟動：

* 已建立新的合併請求
* 現有的合併請求會更新、合併或關閉
* 在源分支中添加提交


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>您希望網頁連結監看以處理合併請求的專案</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 監看合併請求注釋]**

此即時觸發模組會在對合併請求進行註解時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>您希望Webhook監看的專案，以取得合併請求備注</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 監看管道狀態]**

此即時觸發模組會在管道狀態變更時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>希望Webhook監視管道狀態更改的項目</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 監看專案]**

此排程觸發模組會在新增已驗證使用者為其成員的新專案時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL GitLab] 帳戶 [!DNL Workfront] Fusion，請參見 <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] to [!DNL Workfront] 融合</a> 這篇文章。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">最大結果</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中監視的最大記錄數。</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch存放庫分支]**

此排程的觸發程式模組會在新分支新增至存放庫時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL GitLab] 帳戶 [!DNL Workfront] Fusion，請參見 <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] to [!DNL Workfront] 融合</a> 這篇文章。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">最大結果</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中監視的最大記錄數。</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch存放庫標籤]**

此即時觸發模組會在儲存庫中建立或刪除標籤時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>您要網頁連結監看標籤的專案</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 監看程式碼片段註解]**

此即時觸發模組會在對程式碼片段進行新註解時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>您希望網頁連結監看的專案以取得意見</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 觀看托多]**

此計畫觸發模組在添加新操作時啟動一個方案。 未應用任何篩選器時，當添加新的待執行操作時，將運行觸發器。

如需欄位的相關資訊，請參閱 [獲取待辦事項清單](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 觀看Wiki頁面]**

此即時觸發模組會在建立或編輯Wiki頁面時啟動案例。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>選取您要用於此觸發器的網頁連結，或新增新的網頁連結。 </p><p>要添加新的網頁鈎， <ol><li>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</li><li>輸入下列內容： <ul><li>網頁鈎點的名稱</li><li>要用於此Webhook的連接</li><li>希望Wiki頁面的WebHook監視的項目</li></ul></li><li>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。 </td> 
   </tr> 
   </tbody> 
</table>

+++

### 動作

+++**[!UICONTROL 接受合併請求]**

此動作模組會將提交的變更與指定的合併請求合併。

如需欄位的相關資訊，請參閱 [接受合併請求](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取消組建]**

此動作模組會取消專案的單一組建。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL GitLab] 帳戶 [!DNL Workfront] Fusion，請參見 <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] to [!DNL Workfront] 融合</a> 這篇文章。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL項目ID]</td> 
   <td> <p>選取或對應包含您要取消之組建的專案。</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td>選取或對應您要取消的組建。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL合併提交消息]</td> 
   <td> 輸入或映射合併的提交消息。
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL應刪除源分支]</td> 
   <td>選擇是否在合併完成時刪除源分支。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">生成成功時合併[!UICONTROL]</td> 
   <td>選取建置完成後是否立即合併請求。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>如果存在，則此SHA必須與源分支的HEAD匹配。 如果不符合，合併會失敗。</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 取消管道的組建]**

此動作模組會取消單一管道的組建。

如需欄位的相關資訊，請參閱 [取消管道的作業](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 管線成功時取消合併]**

如果管道成功時合併請求被設定為合併，則此動作模組會取消該動作。

如需欄位的相關資訊，請參閱 [管線成功時取消合併](https://docs.gitlab.com/ee/api/merge_requests.html) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 選擇提交]**

此動作模組會挑選指定分支的提交。

如需欄位的相關資訊，請參閱 [選擇提交](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立新標籤]**

此動作模組會為指定存放庫建立新標籤。

如需欄位的相關資訊，請參閱 [建立新標籤](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立新管線]**

此動作模組會為指定專案建立新管道。

如需欄位的相關資訊，請參閱 [建立新管線](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立新版本]**

此動作模組會將發行說明新增至現有的git標籤。

如需欄位的相關資訊，請參閱 [建立發行](https://docs.gitlab.com/ee/api/releases/#create-a-release) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立新標籤]**

此動作模組會在存放庫中建立新標籤，指向提供的參考。

如需欄位的相關資訊，請參閱 [建立新標籤](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立操作]**

此操作模組為當前用戶在選定問題上建立操作。 當前用戶是由用於此模組的連接上的憑據標識的用戶。

如需欄位的相關資訊，請參閱 [建立要執行的](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 在合併請求上建立待辦事項]**

此操作模組為所選合併請求上的當前用戶建立一個操作。 當前用戶是由用於此模組的連接上的憑據標識的用戶。

如需欄位的相關資訊，請參閱 [建立待辦事項](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立合併請求]**

此動作模組會在專案上建立新的合併請求。

如需欄位的相關資訊，請參閱 [建立合併請求](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 在儲存庫中建立新檔案]**

此操作模組將在選定的儲存庫中建立新檔案。

如需欄位的相關資訊，請參閱 [在儲存庫中建立新檔案](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立新的問題說明]**

此動作模組會為單一專案問題建立問題說明。

如需欄位的相關資訊，請參閱 [建立新的問題說明](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立新的合併請求附註]**

此動作模組會為單一合併請求建立附註。

如需欄位的相關資訊，請參閱 [建立新的合併請求附註](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立新里程碑]**

此動作模組會為專案建立新的里程碑。

如需欄位的相關資訊，請參閱 [建立新里程碑](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立新的程式碼片段備注]**

此動作模組會為單一程式碼片段建立新備注。 程式碼片段附註是使用者可張貼至程式碼片段的註解。

如需欄位的相關資訊，請參閱 [建立新的程式碼片段備注](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立存放庫分支]**

此動作模組會建立單一存放庫分支。

如需欄位的相關資訊，請參閱 [建立存放庫分支](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 建立建置變數]**

此動作模組會建立新的組建變數。

如需欄位的相關資訊，請參閱 [建立變數](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 刪除合併請求]**

此動作模組僅適用於管理員和專案擁有者。 它會刪除相關的合併請求

如需欄位的相關資訊，請參閱 [刪除合併請求](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 刪除儲存庫中的現有檔案]**

此動作模組會從存放庫中刪除現有檔案。

如需欄位的相關資訊，請參閱 [刪除儲存庫中的現有檔案](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 刪除儲存庫分支]**

此動作模組會從存放庫中刪除分支。

如需欄位的相關資訊，請參閱 [刪除儲存庫分支](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 編輯問題]**

此動作模組會更新現有的專案問題。 此呼叫也可將問題標示為已關閉。

如需欄位的相關資訊，請參閱 [編輯問題](https://docs.gitlab.com/ee/api/issues.html#edit-issue) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 編輯里程碑]**
此動作模組會更新現有的專案里程碑。

如需欄位的相關資訊，請參閱 [編輯里程碑](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 清除組建]**

此動作模組會清除專案的組建（移除作業成品和作業記錄）。

如需欄位的相關資訊，請參閱 [清除作業](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得todo的清單]**

此搜尋模組會擷取待辦項目清單。

如需欄位的相關資訊，請參閱 [獲取待辦事項清單](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得單一組建]**

此動作模組會擷取專案的單一工作。

如需欄位的相關資訊，請參閱 [獲得一份工作](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得單一存放庫標籤]**

此動作模組會擷取由其名稱決定的特定存放庫標籤。

如需欄位的相關資訊，請參閱 [取得單一存放庫標籤](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得特定部署]**

此動作模組會擷取特定部署。

如需欄位的相關資訊，請參閱 [取得特定部署](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得指派給單一里程碑的所有問題]**

此搜尋模組會擷取指派給單一專案里程碑的所有問題。

如需欄位的相關資訊，請參閱 [取得指派給單一里程碑的所有問題](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 從存放庫取得檔案]**

此動作模組會擷取儲存庫中檔案的相關資訊，例如名稱、大小或內容。

如需欄位的相關資訊，請參閱 [從存放庫取得檔案](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得專案使用者]**

此搜尋模組會擷取專案的使用者。

如需欄位的相關資訊，請參閱 [取得專案使用者](https://docs.gitlab.com/ee/api/projects.html#get-project-users) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得單一問題]**

此動作模組會擷取問題詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>若要建立新連線，請參閱 <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL連接 [!DNL GitLab] 到Workfront聚變]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目]</td> 
   <td> <p>選取包含您要擷取其詳細資訊之問題的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL問題ID]</td> 
   <td> <p>輸入或映射要檢索有關的詳細資訊的問題的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL 獲取單一問題說明]**

此動作模組會針對特定專案問題擷取單一附註。

如需欄位的相關資訊，請參閱 [獲取單一問題說明](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得單一合併請求]**

此動作模組會擷取有關單一合併請求的資訊。

如需欄位的相關資訊，請參閱 [取得單一合併請求](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得單一合併請求變更]**

此搜尋模組會擷取關於合併請求的資訊，包括其檔案和變更。

如需欄位的相關資訊，請參閱 [取得單一合併請求變更](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 獲取單個合併請求提交]**

此動作模組會擷取合併請求提交項目清單。

如需欄位的相關資訊，請參閱 [獲取單個合併請求提交](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得單一合併請求附註]**

此動作模組會針對指定的合併請求傳回單一附註。

如需欄位的相關資訊，請參閱 [取得單一合併請求附註](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得里程碑]**

此動作模組會擷取里程碑詳細資訊。

如需欄位的相關資訊，請參閱 [取得單一里程碑](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得單一專案]**

此動作模組會擷取專案詳細資訊。

如需欄位的相關資訊，請參閱 [取得單一專案](https://docs.gitlab.com/ee/api/projects.html#get-single-project) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 獲取單個儲存庫分支]**

此動作模組會擷取存放庫分支詳細資訊。

如需欄位的相關資訊，請參閱 [獲取單個儲存庫分支](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得程式碼片段附註]**

此模組會擷取指定程式碼片段的單一附註。

如需欄位的相關資訊，請參閱 [取得單一程式碼片段附註](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 獲取提交的注釋]**

此搜索模組檢索項目中提交的注釋。

如需欄位的相關資訊，請參閱 [獲取提交的注釋](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 獲取提交的差異]**

此操作模組獲取項目中提交的差異。

如需欄位的相關資訊，請參閱 [獲取提交的差異](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 保留成品]**

設定到期時，防止刪除對象。

如需欄位的相關資訊，請參閱 [保留成品](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出所有合併請求附註]**

此搜尋模組會擷取單一合併請求的所有附註清單。

如需欄位的相關資訊，請參閱 [列出所有合併請求附註](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出所有程式碼片段附註]**

此模組會取得單一程式碼片段的所有附註清單。 程式碼片段附註是使用者可張貼至程式碼片段的註解。

如需欄位的相關資訊，請參閱 [??](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出提交組建]**

此搜尋模組會傳回專案中特定提交的組建清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>若要建立新連線，請參閱 <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL連接 [!DNL GitLab] 到Workfront聚變]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID]</td> 
   <td> <p>選取包含要列出組建的提交的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL範圍]</td> 
   <td> 若要將搜尋限制為以特定狀態建置，請選取狀態。 將此欄位留空會傳回提交的所有組建。  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL 清單問題]**

此搜尋模組會依指定的篩選設定傳回所有問題。

如需欄位的相關資訊，請參閱 [清單問題](https://docs.gitlab.com/ee/api/issues.html#list-issues) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出合併時關閉的問題]**

此搜尋模組會合併提供的合併請求，以擷取要結束的所有問題。

如需欄位的相關資訊，請參閱 [列出合併時關閉的問題](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 清單標籤]**

此搜尋模組會擷取專案中的所有標籤。

如需欄位的相關資訊，請參閱 [清單標籤](https://docs.gitlab.com/ee/api/labels.html#list-labels) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出合併請求]**

此搜尋模組會依篩選器設定擷取所有合併請求。

如需欄位的相關資訊，請參閱 [列出合併請求](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出擁有的專案]**

此搜尋模組會擷取已驗證使用者設為擁有者的專案。

如需欄位的相關資訊，請參閱 [列出使用者專案](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出專案組建]**

此搜尋模組會擷取專案中的組建清單。

如需欄位的相關資訊，請參閱 [列出專案作業](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出專案部署]**

此搜尋模組會擷取專案中的部署清單。

如需欄位的相關資訊，請參閱 [列出專案部署](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出項目問題說明]**

此搜尋模組會擷取單一問題的所有附註清單。

如需欄位的相關資訊，請參閱 [列出項目問題說明](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出專案問題]**

此搜尋模組會傳回指定專案中的所有問題。

如需欄位的相關資訊，請參閱 [列出專案問題](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出專案里程碑]**

此搜尋模組會擷取專案中的所有里程碑。

如需欄位的相關資訊，請參閱 [列出專案里程碑](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出項目管道]**

此搜尋模組會擷取專案的所有管道。

如需欄位的相關資訊，請參閱 [列出項目管道](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出項目儲存庫標籤]**

此搜尋模組會從專案中擷取存放庫標籤清單，並以反向字母順序依名稱排序。

如需欄位的相關資訊，請參閱 [列出項目儲存庫標籤](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出專案變數]**

此搜尋模組會擷取專案變數的清單。

如需欄位的相關資訊，請參閱 [列出專案變數](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出專案]**

此搜尋模組會擷取已驗證使用者所屬的所有專案。

如需欄位的相關資訊，請參閱 [列出所有專案](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出存放庫分支]**

此模組會依搜尋詞搜尋存放庫分支。

如需欄位的相關資訊，請參閱 [列出存放庫分支](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 清單儲存庫提交]**

此搜索模組檢索項目中的儲存庫提交項清單。

如需欄位的相關資訊，請參閱 [清單儲存庫提交](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 列出儲存庫貢獻者]**

此搜尋模組會擷取存放庫貢獻者清單。

如需欄位的相關資訊，請參閱 [貢獻者](https://docs.gitlab.com/ee/api/repositories.html#contributors) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 清單儲存庫樹]**

此搜索模組檢索項目中的儲存庫檔案和目錄清單。

如需欄位的相關資訊，請參閱 [清單儲存庫樹](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 將操作標籤為完成]**

此動作模組會標籤由目前使用者的ID所提供的單一待辦項目，如已完成。

如需欄位的相關資訊，請參閱 [將標籤為完成項](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 修改現有問題說明]**

修改問題的現有備注。

如需欄位的相關資訊，請參閱 [修改現有問題說明](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 修改現有合併請求說明]**

修改合併請求的現有附註。

如需欄位的相關資訊，請參閱 [修改現有合併請求說明](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 修改現有程式碼片段附註]**

此動作模組會修改程式碼片段的現有備注。

如需欄位的相關資訊，請參閱 [修改現有程式碼片段附註](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 新問題]**

此動作模組會建立新專案問題。

如需欄位的相關資訊，請參閱 [新問題](https://www.integromat.com/en/help/app/gitlab) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 播放組建]**

此動作模組會觸發手動動作以啟動工作。

如需欄位的相關資訊，請參閱 [做工作](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 要提交的貼文評論]**

此操作模組將注釋添加到提交。

如需欄位的相關資訊，請參閱 [要提交的貼文評論](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 移除變數]**

此動作模組會移除專案的變數。

如需欄位的相關資訊，請參閱 [移除變數](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 重試生成]**

此動作模組會在提交中重試單一組建。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>若要建立新連線，請參閱 <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL連接 [!DNL GitLab] 到Workfront聚變]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID]</td> 
   <td> <p>選取包含您要重試之組建的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td> 選取您要重試的組建。 </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL 重試管道中的失敗作業]**

此動作模組重試管道中的組建失敗。

如需欄位的相關資訊，請參閱 [重試管道中的作業](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 取得變數]**

此模組會擷取專案特定變數的詳細資訊。

如需欄位的相關資訊，請參閱 [顯示變數詳細資訊](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 更新發行]**

此動作模組會更新版本。

如需欄位的相關資訊，請參閱 [更新發行](https://docs.gitlab.com/ee/api/releases/#update-a-release) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 更新合併請求]**

此動作模組會更新現有的合併請求。 您可以變更目標分支、標題，甚至關閉MR。

如需欄位的相關資訊，請參閱 [更新合併請求](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) 在 [!DNL GitLab] 檔案。

+++

+++**[!UICONTROL 更新變數]**

此動作模組會更新專案的變數。

如需欄位的相關資訊，請參閱 [更新變數](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) 在 [!DNL GitLab] 檔案。

+++
