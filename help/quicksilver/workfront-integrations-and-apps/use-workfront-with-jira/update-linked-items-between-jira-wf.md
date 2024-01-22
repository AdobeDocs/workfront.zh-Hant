---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 更新連結專案介於 [!DNL Jira] 和 [!DNL Adobe Workfront]
description: 當您連結時 [!DNL Jira] 問題至 [!DNL Adobe Workfront] 任務或問題，您的使用者可以更新一個應用程式中的專案，而該專案的對應專案也會更新第二個應用程式中工作的使用者。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 0%

---

# 更新連結專案介於 [!DNL Jira] 和 [!DNL Adobe Workfront]

當您連結時 [!DNL Jira] 問題至 [!DNL Adobe Workfront] 任務或問題，您的使用者可以更新一個應用程式中的專案，而該專案的對應專案也會更新第二個應用程式中工作的使用者。

如需關於連結專案之間的詳細資訊 [!DNL Workfront] 和 [!DNL Jira]，請參閱 [Adobe Workfront和Jira之間的連結專案](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

當您設定時 [!DNL Workfront] 的 [!DNL Jira]， as a [!DNL Jira] 系統管理員可以設定一個應用程式中的特定欄位，以便與另一個應用程式中連結專案的欄位同步。

如需有關同步連結欄位之間的詳細資訊 [!DNL Jira] 和 [!DNL Workfront] 專案，請參閱 [設定 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td><p>新增：任何</p>
       <p>或</p>
       <p>目前： [！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新增：[！UICONTROL Standard]</p>
       <p>或</p>
       <p>目前： [！UICONTROL計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 存取</td> 
   <td> <p>系統管理員存取權</p> <p>重要：建議您在中建立個別的系統管理員帳戶 [!DNL Jira] 和 [!DNL Workfront] 以專門用於此整合，而不使用可能附加至使用者的現有整合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先決條件

連結專案之前，請先執行下列動作： [!DNL Workfront] 和 [!DNL Jira]，您必須：

* 安裝 [!DNL Workfront for Jira].

  有關安裝的指示 [!DNL Workfront for Jira]，請參閱 [安裝 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* 設定 [!DNL Workfront for Jira].

  有關設定的指示 [!DNL Workfront for Jira]，請參閱 [設定 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* 連結專案介於 [!DNL Workfront] 和 [!DNL Jira].

  如需指示，請參閱 [連結專案介於 [!DNL Adobe Workfront] 和 [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## 更新中的連結專案 [!DNL Workfront]

如果您主要在 [!DNL Workfront]，您可以更新中的工作專案 [!DNL Workfront] 及其中的同行 [!DNL Jira] 也會更新。 此更新會透過整合進行 [!DNL Workfront] 的 [!DNL Jira] 這不需要您擁有 [!DNL Jira] 授權。

只要您的 [!DNL Workfront] 管理員已設定 [!DNL Workfront for Jira] 若要同步化連結專案之間的欄位，請選取您更新於其中的某些欄位 [!DNL Workfront] 也會更新連結的 [!DNL Jira] 問題。 有關更新中專案的詳細資訊 [!DNL Workfront]，請參閱 [編輯問題](../../manage-work/issues/manage-issues/edit-issues.md) 和 [編輯任務](../../manage-work/tasks/manage-tasks/edit-tasks.md).

下列清單顯示哪些 [!DNL Workfront] 欄位同步與 [!DNL Jira] 連結專案上的欄位：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已更新 [!DNL Workfront] 欄位</strong> </th> 
   <th><strong>已同步 [!DNL Jira] 欄位/更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL問題或任務名稱]</td> 
   <td> <p>[！UICONTROL問題名稱]</p> <p>有關名稱變更的註解將新增至 <strong>[!DNL Workfront]</strong> 的標籤 [!DNL Jira] 問題。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL問題或任務說明]</td> 
   <td> <p> [！UICONTROL問題說明]</p> <p>有關更新說明的註解將新增到 <strong>[!DNL Workfront]</strong> 的標籤 [!DNL Jira] 問題。<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [！UICONTROL已上傳檔案]</p> <p>附註：連結到的檔案 [!DNL Workfront] 來自外部伺服器的專案未傳輸至 [!DNL Jira] 問題。 僅限直接上傳到的檔案 [!DNL Workfront] 專案也會更新至連結的 [!DNL Jira] 問題。 </p> </td> 
   <td> <p>[！UICONTROL附件]</p> <p>有關已上傳附件的註解已新增至 <strong>[!DNL Workfront]</strong> 的標籤 [!DNL Jira] 問題。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫完成日期]</td> 
   <td> <p>[！UICONTROL到期日期]</p> <p>有關已變更的[！UICONTROL到期日]的註解已新增至 [!DNL Workfront] 的標籤 [!DNL Jira] 問題。 </p> <p>附註：您必須啟用 <strong>[！UICONTROL到期日期]</strong> 針對您的 [!DNL Jira] 在[！UICONTROL Jira]中看到此欄位更新時出現問題。 </p> </td> 
  </tr> 
  <tr> 
   <td>自訂Forms和自訂欄位</td> 
   <td> <p> 顯示在 [!DNL Workfront] 的右側面板 [!DNL Jira] 問題。 <br>面板中只會顯示具有實際值的自訂欄位。<br></p> <p>注意：自訂表單區段會以的存取層級顯示 [!DNL Workfront] 管理員。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL問題或任務優先順序]</td> 
   <td>顯示在 [!DNL Workfront] 的右側面板 [!DNL Jira] 問題。 <br>它不會更新問題 <strong>[！UICONTROL優先順序]</strong> 中的欄位 [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄時間] </td> 
   <td> <p>有關記錄時間的註解會新增至 <strong>[!DNL Workfront]</strong> 的標籤 [!DNL Jira] 問題。 這包括記錄時間的使用者名稱，以及記錄時間的使用者名稱（如果不同）。 沒有任何時間登入 <strong>[！UICONTROL工作記錄檔]</strong> 定位於 [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL註解]</td> 
   <td> <p>註解將新增至 <strong>[!DNL Workfront]</strong> 的標籤 [!DNL Jira] 問題。 它不會新增至 <strong>[！UICONTROL註解]</strong> 的標籤 [!DNL Jira] 問題</p> <p>附註：當您手動連結兩個現有專案時，新增至的註解會 [!DNL Workfront] 專案之前，先將它連結至 [!DNL Jira] 不要同步至 [!DNL Jira] 問題。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 更新中的連結專案 [!DNL Jira]

如果您主要在 [!DNL Jira]，您可以更新中的工作專案 [!DNL Jira] 及其中的同行 [!DNL Workfront] 也會更新。 您不一定要擁有 [!DNL Workfront] 的授權 [!DNL Workfront] 連結至您的 [!DNL Jira] 接收您在中進行更新的問題 [!DNL Jira].

條件為 [!DNL Workfront] 管理員已設定 [!DNL Workfront] 的 [!DNL Jira] 若要同步化連結專案之間的欄位，您更新其中的某些欄位 [!DNL Jira] 也會更新連結的 [!DNL Workfront] 個專案。

下列清單顯示哪些 [!DNL Jira] 欄位同步與 [!DNL Workfront] 連結專案上的欄位：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已更新 [!DNL Jira] 欄位</strong> </th> 
   <th><strong>已同步 [!DNL Workfront] 欄位/更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL問題狀態]</td> 
   <td> <p> [！UICONTROL問題或任務狀態]</p> <p>中的問題狀態 [!DNL Jira] 在Workfront中同步下列狀態或等同於下列狀態的狀態：</p> 
    <ul> 
     <li> <p>[！UICONTROL NEW] ([！UICONTROL NEW])</p> </li> 
     <li> <p>[！UICONTROL進行中] ([！UICONTROL INP])</p> </li> 
     <li> <p>[！UICONTROL已關閉]/[！UICONTROL完成] ([！UICONTROL CLS]/[！UICONTROL CPL])</p> </li> 
    </ul> <p>注意： [!DNL Jira] 狀態會與第一個同步 [!DNL Workfront] 相等於適當狀態的狀態。</p> <p>有關中專案狀態的詳細資訊 [!DNL Workfront]，請參閱 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[！UICONTROL問題附件]</td> 
   <td> [！UICONTROL問題或任務檔案]<br>關於上傳新檔案的註解 [!DNL Jira] 已新增至[！UICONTROL更新]索引標籤 [!DNL Workfront] 問題或任務。  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL到期日期]</td> 
   <td> <p> 有關[！UICONTROL到期日]變更的註解 [!DNL Jira] 已新增至[！UICONTROL更新]索引標籤 [!DNL Workfront] 問題或任務。 </p> <p>注意：此日期沒有變更 [!DNL Workfront] 問題或任務。 </p> </td> 
  </tr> 
  <tr> 
   <td> 將時間記錄在 [!DNL Workfront] 右面板或從[！UICONTROL更多]功能表的 [!DNL Jira] 問題<br></td> 
   <td> <p>小時<br>除了將登入Jira的時數新增至連結之外 [!DNL Workfront] 專案，有關記錄時間的註解會新增至的[！UICONTROL更新]索引標籤 [!DNL Workfront] 個專案。</p> <p>如需有關連結的記錄時間的詳細資訊 [!DNL Jira] 問題，包括更新 [!DNL Jira] 正在記錄時間的使用者 [!DNL Workfront]，請參閱 <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">連結的記錄時間 [!DNL Jira] 和 [!DNL Workfront] 個專案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> 註解 <br><br></td> 
   <td> <p>註解會新增至的[！UICONTROL Updates]索引標籤 [!DNL Workfront] 問題或任務，如果 <strong>[！UICONTROL註解]</strong> 在[！UICONTROL Setup]標籤的[！UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT]區段中設定為 <strong>[！UICONTROL Always]</strong>.</p> <p>如需有關在中配置Workfront設定的資訊 [!DNL Jira]，請參閱 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">設定 [!DNL Workfront for Jira]</a>.</p> <p>如需如何評論連結專案的相關資訊 [!DNL Jira] 問題，請參閱 <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">來自連結的註解 [!DNL Jira] 問題</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 從連結記錄時間 [!DNL Jira] 問題

您記錄的時間 [!DNL Jira] 中的專案 [!DNL Jira] 也會轉移至連結的 [!DNL Workfront] 個專案，無論位於何處 [!DNL Jira] 您記錄時間。\
當您在Jira中登入時間 [!DNL Workfront] 時，時間僅記錄在 [!DNL Workfront].\
您錄製的時間 [!DNL Workfront] 不會影響中連結問題的時間 [!DNL Jira].

>[!NOTE]
>
>如果將時間新增到 [!DNL Jira] 連結至的專案 [!DNL Workfront] 任務， [!UICONTROL 小時型別] 時間單位： [!DNL Workfront] 是 [!UICONTROL 任務時間]. 如果將時間新增到 [!DNL Jira] 連結至的專案 [!DNL Workfront] 問題， [!UICONTROL 小時型別] 時間單位： [!DNL Workfront] 是 [!UICONTROL 問題時間].

註解已新增至 **[!DNL Workfront]** 定位於 [!DNL Jira] 和 **[!UICONTROL 更新]** 中的專案索引標籤 [!DNL Workfront] 以記錄記錄時間。\
時間也會顯示在 **[!UICONTROL 小時]** 的標籤 [!DNL Workfront] 個專案。

* [連結的記錄時間 [!DNL Jira] 和 [!DNL Workfront] 個專案](#log-time-for-linked-jira-and-workfront-items)
* [記錄時間從 [!DNL Jira] 至 [!DNL Workfront] 專案](#log-time-from-jira-to-a-workfront-item)

### 連結的記錄時間 [!DNL Jira] 和 [!DNL Workfront] 個專案

您可以記錄來自以下專案的時間： [!DNL Jira] 連結至的問題 [!DNL Workfront] 專案，並且時間會同時記錄在 [!DNL Jira] 問題以及 [!DNL Workfront] 個專案。

>[!IMPORTANT]
>
>如果使用者登入時間 [!DNL Jira] 不存在於 [!DNL Workfront]，整合會在Workfront中建立新的作用中使用者，如果 **[!UICONTROL 自動在中建立使用者 [!DNL Workfront]如&#x200B;果 [!DNL Jira] 使用者沒有&#x200B;*[!DNL Workfront]帳&#x200B;戶]**已設為**[!UICONTROL &#x200B;一直&#x200B;]**. 此使用者未佔用 [!DNL Workfront] 授權。 您可以將作用中的使用者指派給中的工作專案 [!DNL Workfront]，但您不能將其納入更新中。 有關設定自動建立的 [!DNL Workfront] 使用者來源 [!DNL Jira]，請參閱 [設定 [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

若要在中記錄專案的時間 [!DNL Jira] 並將它錄製在 [!DNL Jira] 和 [!DNL Workfront]：

1. 登入 [!DNL Jira].
1. 前往 [!DNL Jira] 連結至的問題 [!DNL Workfront] 個專案。
1. 展開 **[!UICONTROL 更多]** 功能表並按一下 **[!UICONTROL 記錄工作]**.

1. 在 **[!UICONTROL 逗留時間]** 欄位中，指定處理此問題所花費的時間。 您必須使用下列期間來指定時間：

   * [!UICONTROL 周] (w)
   * [!UICONTROL 天] (d)
   * [!UICONTROL 小時] (h)

1. 繼續將資訊新增至您的時間專案，包括 **[!UICONTROL 工作說明]**，然後按一下 **[!UICONTROL 記錄]**.\
   時間會新增至 **[!UICONTROL 工作記錄檔]** 的標籤 [!DNL Jira] 專案，以及 [!DNL Workfront] 連結至它的專案。\
   時間專案的工作說明會記錄為中時數專案的備註 [!DNL Workfront].

### 記錄時間從 [!DNL Jira] 至 [!DNL Workfront] 專案

您可以只將時間記錄到連結的 [!DNL Workfront] 專案來自 [!DNL Jira] 未將此次錄製到的問題 [!DNL Jira] 問題。

1. 登入 [!DNL Jira].
1. 導覽至 [!DNL Jira] 連結至的問題 [!DNL Workfront] 個專案。

   「 」的詳細資料 [!DNL Workfront] 專案應顯示在 [!DNL Workfront] 問題的右側面板。

1. 按一下 **[!UICONTROL 記錄時間]** 圖示。

1. 指定數量 **[!UICONTROL 小時]** 和 **[!UICONTROL 分鐘]** 您要登入問題。

1. 按一下 **[!UICONTROL 記錄時間]**.

   時間會新增至 [!DNL Workfront] 個專案。

   此時間未新增至 [!UICONTROL 工作記錄檔] 的標籤 [!DNL Jira] 問題。

## 來自連結的註解 [!DNL Jira] 問題 {#comment-from-a-linked-jira-issue}

當您註解 [!DNL Jira] 專案來自 [!DNL Workfront] 右側面板於 [!DNL Jira]，則註解也會新增至 [!UICONTROL 更新] Workfront中連結專案的索引標籤。

註解來源 [!DNL Jira] 至 [!DNL Workfront] 專案：

1. 登入 [!DNL Jira].
1. 導覽至 [!DNL Jira] 連結至的問題 [!DNL Workfront] 個專案。

   「 」的詳細資料 [!DNL Workfront] 專案應顯示在 [!DNL Workfront] 問題的右側面板。

1. 按一下 **[!UICONTROL 註解]** 圖示於 [!DNL Workfront] 面板或 **[!UICONTROL 註解]** 標籤。

1. 開始輸入評論，然後按一下 **[!UICONTROL 傳送]**.

   註解會新增至下列專案：

   * 此 **[!DNL Workfront]** 的標籤 [!DNL Jira] 問題。
   * 此 **[!UICONTROL 註解]** 的標籤 [!DNL Jira] 問題。
   * 此 **[!UICONTROL 更新]** Workfront中連結專案的索引標籤。
