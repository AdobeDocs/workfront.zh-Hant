---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 更新之間的連結項目 [!DNL Jira] 和 [!DNL Adobe Workfront]
description: 連結時 [!DNL Jira] 問題 [!DNL Adobe Workfront] 任務或問題時，您的用戶可以更新一個應用程式中的項目，而該項目的對應項也會為第二個應用程式中工作的用戶更新。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 0%

---

# 更新之間的連結項目 [!DNL Jira] 和 [!DNL Adobe Workfront]

連結時 [!DNL Jira] 問題 [!DNL Adobe Workfront] 任務或問題時，您的用戶可以更新一個應用程式中的項目，而該項目的對應項也會為第二個應用程式中工作的用戶更新。

如需連結項目的詳細資訊，請參閱 [!DNL Workfront] 和 [!DNL Jira]，請參閱 [Adobe Workfront與Jira之間的連結項目](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

正如您設定 [!DNL Workfront] for [!DNL Jira]，作為 [!DNL Jira] 系統管理員，您可以配置一個應用程式中的某些欄位，以便與另一個應用程式中連結項目的欄位同步。

有關在連結之間同步欄位的詳細資訊 [!DNL Jira] 和 [!DNL Workfront] 項目，請參閱 [設定 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 計劃</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 授權概述</a>*</td> 
   <td> <p>[!UICONTROL計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 存取</td> 
   <td> <p>系統管理員存取</p> <p>重要：建議您在 [!DNL Jira] 和 [!DNL Workfront] 以專用於此整合，而非使用可能附加至使用者的現有整合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

在您可以連結項目之間之前 [!DNL Workfront] 和 [!DNL Jira]，您必須

* 安裝 [!DNL Workfront for Jira].

   安裝說明 [!DNL Workfront for Jira]，請參閱 [安裝 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* 設定 [!DNL Workfront for Jira].

   配置說明 [!DNL Workfront for Jira]，請參閱 [設定 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* 在 [!DNL Workfront] 和 [!DNL Jira].

   如需指示，請參閱 [在 [!DNL Adobe Workfront] 和 [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## 更新中的連結項目 [!DNL Workfront]

如果您主要在 [!DNL Workfront]，您可以在 [!DNL Workfront] 和同行 [!DNL Jira] 也會更新。 此更新會透過 [!DNL Workfront] for [!DNL Jira] 不要求您 [!DNL Jira] 授權。

只要 [!DNL Workfront] 管理員已配置 [!DNL Workfront for Jira] 要同步連結項目之間的欄位，請在中更新某些欄位 [!DNL Workfront] 也會更新連結的 [!DNL Jira] 問題。 如需更新中項目的詳細資訊，請參閱 [!DNL Workfront]，請參閱 [編輯問題](../../manage-work/issues/manage-issues/edit-issues.md) 和 [編輯任務](../../manage-work/tasks/manage-tasks/edit-tasks.md).

下列清單顯示 [!DNL Workfront] 與同步的欄位 [!DNL Jira] 連結項目上的欄位：

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
   <td>[!UICONTROL問題或任務名稱]</td> 
   <td> <p>[!UICONTROL問題名稱]</p> <p>「名稱」變更的註解會新增至 <strong>[!DNL Workfront]</strong> 的 [!DNL Jira] 問題。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL問題或任務說明]</td> 
   <td> <p> [!UICONTROL問題說明]</p> <p>會將有關更新說明的註解新增至 <strong>[!DNL Workfront]</strong> 的 [!DNL Jira] 問題。<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL已上載文檔]</p> <p>注意：連結到的文檔 [!DNL Workfront] 來自外部伺服器的項目不會傳輸至 [!DNL Jira] 問題。 僅直接上載到的文檔 [!DNL Workfront] 項目也會更新至連結的 [!DNL Jira] 問題。 </p> </td> 
   <td> <p>[!UICONTROL附件]</p> <p>已上傳附件的註解會新增至 <strong>[!DNL Workfront]</strong> 的 [!DNL Jira] 問題。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫完成日期]</td> 
   <td> <p>[!UICONTROL到期日]</p> <p>已變更的[!UICONTROL到期日]備注會新增至 [!DNL Workfront] 的 [!DNL Jira] 問題。 </p> <p>注意：您必須啟用 <strong>[!UICONTROL到期日]</strong> 為 [!DNL Jira] 無法在[!UICONTROL Jira]中查看此欄位更新的問題。 </p> </td> 
  </tr> 
  <tr> 
   <td>自訂Forms和自訂欄位</td> 
   <td> <p> 顯示於 [!DNL Workfront] 右面板 [!DNL Jira] 問題。 <br>面板中只會顯示具有實際值的自訂欄位。<br></p> <p>注意：「自訂表單」區段會以 [!DNL Workfront] 管理員。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL問題或任務優先順序]</td> 
   <td>顯示於 [!DNL Workfront] 右面板 [!DNL Jira] 問題。 <br>不會更新問題 <strong>[!UICONTROL優先順序]</strong> 欄位 [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日誌時間] </td> 
   <td> <p>會在 <strong>[!DNL Workfront]</strong> 的 [!DNL Jira] 問題。 這包括記錄時間的使用者名稱，以及記錄時間的使用者（若不同）。 沒有時間登入 <strong>[!UICONTROL工作日誌]</strong> 標籤 [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注釋]</td> 
   <td> <p>註解會新增至 <strong>[!DNL Workfront]</strong> 的 [!DNL Jira] 問題。 不會新增至 <strong>[!UICONTROL注釋]</strong> 的 [!DNL Jira] 問題</p> <p>注意：手動連結兩個現有項目時，會顯示已新增至 [!DNL Workfront] 項目，然後再將其連結至 [!DNL Jira] 不會同步到 [!DNL Jira] 問題。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 更新中的連結項目 [!DNL Jira]

如果您主要在 [!DNL Jira]，您可以在 [!DNL Jira] 和同行 [!DNL Workfront] 也會更新。 您不必擁有 [!DNL Workfront] 的授權 [!DNL Workfront] 連結至 [!DNL Jira] 接收您在 [!DNL Jira].

條件是 [!DNL Workfront] 管理員已配置 [!DNL Workfront] for [!DNL Jira] 要同步連結項目之間的欄位，請在 [!DNL Jira] 也會更新連結的 [!DNL Workfront] 項目。

下列清單顯示 [!DNL Jira] 與同步的欄位 [!DNL Workfront] 連結項目上的欄位：

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
   <td>[!UICONTROL問題狀態]</td> 
   <td> <p> [!UICONTROL問題或任務狀態]</p> <p>問題狀態(在 [!DNL Jira] 在Workfront中與下列狀態或等於下列狀態的狀態同步：</p> 
    <ul> 
     <li> <p>[!UICONTROL新建]（[!UICONTROL新建]）</p> </li> 
     <li> <p>[!UICONTROL正在進行]([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete]([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>注意：此 [!DNL Jira] 狀態會與第一個同步 [!DNL Workfront] 狀態等於適當狀態。</p> <p>如需中項目狀態的詳細資訊，請參閱 [!DNL Workfront]，請參閱 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL問題受託人]</td> 
   <td> <p> [!UICONTROL問題或任務受託人]</p> <p>重要：當您在 [!DNL Jira] 使用者 [!DNL Workfront] 帳戶時，整合會在 [!DNL Workfront] 僅當選項"[!UICONTROL自動建立用戶 [!DNL Workfront] 若 [!DNL Jira] 使用者沒有 [!DNL Workfront] account]」設為[!UICONTROL Always]。 此使用者未佔用 [!DNL Workfront] 授權。 可以為中的工作項目指派活躍的使用者 [!DNL Workfront]，但無法納入更新中。 如需設定自動建立的詳細資訊，請參閱 [!DNL Workfront] 使用者 [!DNL Jira]，請參閱 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">設定 [!DNL Workfront for Jira]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL問題附件]</td> 
   <td> [!UICONTROL問題或任務文檔]<br>關於在 [!DNL Jira] 會新增至的[!UICONTROL更新]標籤中 [!DNL Workfront] 問題或任務。  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL到期日]</td> 
   <td> <p> 關於變更 [!DNL Jira] 會新增至的[!UICONTROL更新]標籤中 [!DNL Workfront] 問題或任務。 </p> <p>注意：日期不變 [!DNL Workfront] 問題或任務。 </p> </td> 
  </tr> 
  <tr> 
   <td> 登入時間 [!DNL Workfront] 右面板或[!UICONTROL更多]菜單中的 [!DNL Jira] 問題<br></td> 
   <td> <p>小時<br>除了將Jira中記錄的小時數新增至連結的 [!DNL Workfront] 項目，則會在的[!UICONTROL更新]標籤中新增有關記錄時間的註解 [!DNL Workfront] 項目。</p> <p>如需連結之上記錄時間的詳細資訊 [!DNL Jira] 問題，包括更新 [!DNL Jira] 正在登錄時間的用戶 [!DNL Workfront]，請參閱 <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">連結的記錄時間 [!DNL Jira] 和 [!DNL Workfront] 項目</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> 註解 <br><br></td> 
   <td> <p>註解會新增至 [!DNL Workfront] 問題或任務(如果 <strong>[!UICONTROL注釋]</strong> 在[!UICONTROL設定]頁簽的[!UICONTROL從JIRA同步到WORKFRONT]部分中的設定 <strong>[!UICONTROL Always]</strong>.</p> <p>如需有關在中設定Workfront設定的資訊，請參閱 [!DNL Jira]，請參閱 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">設定 [!DNL Workfront for Jira]</a>.</p> <p>如需關於從連結項目加上註解的資訊 [!DNL Jira] 問題，請參閱 <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">來自連結的留言 [!DNL Jira] 問題</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 來自連結的記錄時間 [!DNL Jira] 問題

您為 [!DNL Jira] 項目 [!DNL Jira] 也會轉讓至連結的 [!DNL Workfront] 項目，無論位於 [!DNL Jira] 你記錄時間。\
當您在Jira登錄時 [!DNL Workfront] ，則時間僅記錄在 [!DNL Workfront].\
您記錄的時間 [!DNL Workfront] 不會影響 [!DNL Jira].

>[!NOTE]
>
>如果時間已新增至 [!DNL Jira] 連結到 [!DNL Workfront] 任務， [!UICONTROL 小時類型] 在 [!DNL Workfront] is [!UICONTROL 任務時間]. 如果時間已新增至 [!DNL Jira] 連結到 [!DNL Workfront] 問題， [!UICONTROL 小時類型] 在 [!DNL Workfront] is [!UICONTROL 問題時間].

註解會新增至 **[!DNL Workfront]** 標籤 [!DNL Jira] 和 **[!UICONTROL 更新]** 中項目的索引標籤 [!DNL Workfront] 記錄時間。\
時間也會顯示在 **[!UICONTROL 小時]** 的 [!DNL Workfront] 項目。

* [連結的記錄時間 [!DNL Jira] 和 [!DNL Workfront] 項目](#log-time-for-linked-jira-and-workfront-items)
* [從 [!DNL Jira] 到 [!DNL Workfront] 項目](#log-time-from-jira-to-a-workfront-item)

### 連結的記錄時間 [!DNL Jira] 和 [!DNL Workfront] 項目

您可以從 [!DNL Jira] 連結至 [!DNL Workfront] 項目，且時間會記錄在 [!DNL Jira] 問題和 [!DNL Workfront] 項目。

>[!IMPORTANT]
>
>如果使用者登入 [!DNL Jira] 中不存在 [!DNL Workfront]，整合會在Workfront中建立新的作用中使用者(若 **[!UICONTROL 在中自動建立使用者 [!DNL Workfront]&#x200B;如果 [!DNL Jira] 使用者沒有&#x200B;*[!DNL Workfront]&#x200B;帳戶]**設為**[!UICONTROL &#x200B;一律&#x200B;]**. 此使用者未佔用 [!DNL Workfront] 授權。 您可以指派作用中使用者至中的工作項目 [!DNL Workfront]，但您無法將其納入更新中。 有關配置自動建立的資訊 [!DNL Workfront] 使用者 [!DNL Jira]，請參閱 [設定 [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

登錄項的時間 [!DNL Jira] 並且記錄在 [!DNL Jira] 和 [!DNL Workfront]:

1. 登入 [!DNL Jira].
1. 前往 [!DNL Jira] 與 [!DNL Workfront] 項目。
1. 展開 **[!UICONTROL 更多]** 按一下 **[!UICONTROL 記錄工作]**.

1. 在 **[!UICONTROL 逗留時間]** 欄位中，指定處理此問題所花費的時間。 您必須使用下列時段來指定時間：

   * [!UICONTROL 周] (w)
   * [!UICONTROL 天] (d)
   * [!UICONTROL 小時] (h)

1. 繼續將資訊添加到時間條目，包括 **[!UICONTROL 工作說明]**，然後按一下 **[!UICONTROL 記錄檔]**.\
   時間會新增至 **[!UICONTROL 工作記錄]** 的 [!DNL Jira] 項目，以及 [!DNL Workfront] 連結到的項目。\
   時間條目的工作說明記錄為小時條目的附註，位於 [!DNL Workfront].

### 從 [!DNL Jira] 到 [!DNL Workfront] 項目

您可以只將時間記錄到連結的 [!DNL Workfront] 項目 [!DNL Jira] 此時未記錄的問題 [!DNL Jira] 問題。

1. 登入 [!DNL Jira].
1. 導覽至 [!DNL Jira] 連結至 [!DNL Workfront] 項目。

   此 [!DNL Workfront] 項目應顯示在 [!DNL Workfront] 問題的右面板。

1. 按一下 **[!UICONTROL 記錄時間]** 表徵圖。

1. 指定 **[!UICONTROL 小時]** 和 **[!UICONTROL 分鐘]** 您要記錄問題。

1. 按一下 **[!UICONTROL 記錄時間]**.

   時間會新增至 [!DNL Workfront] 項目。

   此次不會新增至 [!UICONTROL 工作記錄] 的 [!DNL Jira] 問題。

## 來自連結的留言 [!DNL Jira] 問題 {#comment-from-a-linked-jira-issue}

當您對 [!DNL Jira] 項目 [!DNL Workfront] 右側面板 [!DNL Jira]，註解也會新增至 [!UICONTROL 更新] 頁簽中的連結項目。

若要從 [!DNL Jira] 到 [!DNL Workfront] 項目：

1. 登入 [!DNL Jira].
1. 導覽至 [!DNL Jira] 連結至 [!DNL Workfront] 項目。

   此 [!DNL Workfront] 項目應顯示在 [!DNL Workfront] 問題的右面板。

1. 按一下 **[!UICONTROL 註解]** 圖示 [!DNL Workfront] 或 **[!UICONTROL 註解]** 標籤。

1. 開始鍵入注釋，然後按一下 **[!UICONTROL 傳送]**.

   註解會新增至下列項目：

   * 此 **[!DNL Workfront]** 的 [!DNL Jira] 問題。
   * 此 **[!UICONTROL 註解]** 的 [!DNL Jira] 問題。
   * 此 **[!UICONTROL 更新]** 頁簽中的連結項目。
