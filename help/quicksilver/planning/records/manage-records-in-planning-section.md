---
title: 在Adobe Workfront物件的Planning區段中管理記錄
description: 您可以在左側面板的Workfront物件的Planning區段中，顯示連線至Adobe Workfront物件的Workfront Planning記錄。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1734'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# 管理來自Workfront物件的記錄連線

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

您可在Workfront中，於下列連結物件的區域顯示Workfront Planning記錄：

* Workfront物件的Planning區段：顯示連線到物件的所有記錄型別及其各自的連線記錄。
* Planning連線自訂欄位：顯示一個記錄型別、其個別連線記錄，以及連線記錄的最多7個查詢欄位。

## 存取需求

+++ 展開以檢視存取需求。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 產品</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront規劃<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td>
   <td>
<p>下列任一Workfront計畫：</p>
<ul><li>選取</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>舊版Workfront計畫不提供Workfront計畫</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td>
   <td>
<p>任何</p>
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p>
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權*</p></td>
   <td>
   <p>標準</p>
   <p>Workfront計畫不適用於舊版Workfront授權</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>檢視專案、方案和投資組合或取得更高的存取權</p>  
   <p>Workfront Planning沒有存取層級設定。 </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td>
   <p>在Workfront中，檢視專案、投資組合或方案的或更高許可權</a> </p> 
   <p>在Workfront規劃中：
   <ul><li>
   檢視工作區的許可權和記錄型別，以檢視任何連線的記錄 </li>
   或
   <li> 貢獻或更高的許可權至工作區和記錄型別，以連線或中斷記錄連線</a></li></ul> </p>  
   <p>系統管理員擁有所有Workfront Planning工作區的許可權，包括他們未建立的工作區</p> 
  </td>
  </tr>
 </tbody>
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 管理Planning區段中的記錄

您可以使用Workfront物件的Planning區段來檢視連線到Workfront物件的所有記錄型別及其各自的記錄。
「規劃」區段適用於下列Workfront物件：

* 專案
* 專案組合
* 方案
<!--* Group
* Company-->

### 關於Workfront物件Planning區段的考量事項

當您從Workfront物件的Planning區段檢視Workfront Planning記錄時，請考量下列事項：

* Workfront Planning記錄型別必須先連線至Workfront物件型別。

  如需詳細資訊，請參閱下列文章：

   * [連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [連接記錄](/help/quicksilver/planning/records/connect-records.md)
* 您可以從Workfront物件檢視Planning區段，即使沒有與Workfront物件相關聯的記錄亦然。

### 從Planning區段管理記錄連線

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下連線到Workfront專案、投資組合或方案的記錄型別的卡片。
1. 在表格檢視或記錄的詳細資訊頁面中，移至與Workfront物件有連線的已連線記錄欄位。 如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。
1. 在連線的記錄欄位中按一下Workfront物件的名稱。
物件的頁面會在Workfront中開啟。

   >[!NOTE]
   >
   >  如果您知道Workfront物件已連線至Planning記錄，則可以從Workfront物件導覽至Planning區段。

1. 按一下左側面板中的&#x200B;**規劃**。

   >[!NOTE]
   >
   >   您的Workfront或群組管理員必須先將Planning區段新增到您的版面配置範本中，才能為Workfront專案、投資組合或方案顯示該區段。

   Planning區段會顯示下列資訊：

   * 連線的記錄會顯示在包含以下資訊的個別卡片上：
      * 記錄名稱
      * 記錄縮圖
      * 在Workfront Planning中顯示的連線記錄欄位名稱。
   * 記錄會顯示在各自的工作區和記錄型別下。

   專案![上的](assets/planning-section-on-project.png)規劃區段

1. （選擇性）按一下[顯示所有連線]&#x200B;**&#x200B;**&#x200B;以顯示所有連線的記錄型別，包括沒有連線記錄的記錄型別。 依預設，不顯示沒有連線記錄的記錄型別。
1. 按一下記錄卡以顯示有關記錄的更多資訊。 記錄預覽方塊隨即顯示。
1. （選用）開始修改記錄預覽方塊中的欄位。 您的變更會自動儲存。
1. （選擇性）按一下預覽方塊右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤圖示中開啟詳細資料](assets/open-details-in-a-new-tab-icon.png)以開啟記錄的詳細資訊頁面。 記錄的詳細資訊頁面會在Workfront Planning中開啟。
1. （選擇性）將游標停留在記錄卡上，然後按一下中斷連線記錄圖示&#x200B;**-**，然後按一下&#x200B;**中斷連線**。
會發生下列情況：
   * 記錄不再連線至Workfront物件。
   * Workfront物件也會從Workfront Planning的記錄連線欄位中移除。
   * 連線至Planning記錄的Workfront查閱欄位值也會一併刪除。
1. 按一下&#x200B;**連線**，為連線的記錄型別連線更多記錄。

   如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。
1. （選擇性）如果您找不到要連線的記錄，而且您想要新增該記錄，請按一下[新增] **+ [新增]**&#x200B;以新增記錄。 如需詳細資訊，請參閱文章[建立記錄](/help/quicksilver/planning/records/create-records.md)中的「當您從其他記錄連線記錄時建立記錄」一節。

   會發生下列情況：

   * 記錄會立即連線至Workfront物件，並顯示在Planning區段中。
   * Workfront物件會新增至Workfront Planning記錄的已連線欄位。
   * 與Planning記錄連線之Workfront查詢欄位的值會填入Workfront Planning中。

## 管理Planning連線欄位型別中的記錄

您可以使用Workfront物件上的Planning連線自訂欄位，檢視連線至Workfront物件的記錄型別及其個別記錄。

當您建立Planning連線自訂欄位時，可以控制為Workfront物件顯示哪些Planning記錄型別。

* Planning連線欄位會在建立連線之後，以及將該欄位附加到下列Workfront物件的表單時，顯示Planning記錄：

   * 專案
   * 專案組合
   * 方案
   * 群組
   * 公司

如需詳細資訊，請參閱[建立表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

### 有關Planning連線欄位型別的考量事項

當您從Workfront物件的Planning連線欄位檢視Workfront Planning記錄時，請考量下列事項：

* Planning記錄連線至Workfront物件後，Workfront物件的自訂表單上會以下列方式顯示Planning連線欄位：

   * 如果只選取所連線記錄的主要欄位，則如果連線允許連結多個記錄，則Planning連線欄位會顯示為具有多個值的欄位。 如需詳細資訊，請參閱[連線記錄型別概觀](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。
   * 如果您的Workfront或群組管理員從自訂表單上的連線記錄中新增了其他查閱欄位，則Planning連線欄位會顯示為表格。 最多可以為Planning連線欄位選取7個欄位。 表格檢視是唯讀的。

* 您只能將一個記錄型別與一個Planning連線欄位建立關聯。 您在表單中的Planning連線欄位數量沒有限制。
* 您必須擁有物件、記錄和Workfront Planning的正確存取權和許可權，才能將具有Planning連線自訂欄位的自訂表單附加至Workfront物件。
* 您必須擁有Workfront Planning中工作區的Contribute許可權，才能從Workfront物件的Planning連線欄位連線或中斷連線記錄。
* Workfront Planning記錄型別必須先連線至Workfront物件型別。 如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。這可讓Workfront Planning記錄從Workfront存取。
* 您只能針對可具有Workfront Planning連線的物件，從Workfront物件的Planning連線欄位連線或中斷連線記錄。

  例如，您也許可以將具有Planning連線欄位的自訂表單附加到任務，但無法將Workfront Planning物件連線到任務。
* 大量編輯Workfront物件時，您無法編輯Planning連線欄位。

### 管理來自Planning連線欄位型別的記錄連線

1. 移至下列其中一個已連線至Workfront Planning記錄型別的物件型別：

   * 專案
   * 專案組合
   * 方案
   * 公司
   * 群組

1. 按一下左側面板中的&#x200B;**&lt; Object > Details**。
1. （視條件而定）為您選取的物件新增自訂表單，其中至少有一個Planning連線欄位（如果沒有）。

   >[!NOTE]
   >
   >您的Workfront或群組管理員必須先建立表單並在其上新增Planning連線欄位，才能將其新增至物件。


1. 按一下欄位內部以新增連線的記錄，然後按一下欄位內部的向下箭頭，以從清單中選取記錄。

   ![在記錄清單開啟的專案上規劃連線欄位](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >您無法將記錄新增至與Workfront物件（設定該欄位時所選取的物件除外）關聯的Planning連線欄位。
   >
   >例如，您無法從專案的自訂表單將記錄新增至為Portfolio連線所建立的Planning連線欄位。
   >
   >有指示表示欄位的物件與您選取的物件不相符。
   >
   >![警告表單](assets/warning-unsupported-object-planning-connection-field-on-form.png)上不支援的物件Planning連線欄位

1. 按一下清單外部以將其關閉。

   會發生下列情況：

   * 記錄會立即連線至Workfront物件，並顯示在Planning連線欄位以及Workfront物件的Planning區段中。
   * Workfront物件會新增至Workfront Planning記錄的已連線欄位。
   * 與Planning記錄連線之Workfront查詢欄位的值會填入Workfront Planning中。
   * 如果您的Workfront或群組管理員在建立自訂表單時新增記錄查詢欄位，記錄的查詢欄位會自動填入表格檢視中。 Planning連線欄位中的表格檢視是唯讀的。

     ![專案詳細資料自訂表單上具有資料表的Planning連線欄位](assets/planning-connection-field-with-table-on-project-details-custom-form.png)

     >[!NOTE]
     >
     >只有在自訂表單的Planning連線欄位中新增查閱欄位時，才會顯示表格檢視。


1. （選擇性）在Planning連線欄位中，按一下記錄名稱或暫留在表格中的記錄名稱，然後按一下Planning連線自訂表單上的&#x200B;**開啟記錄**&#x200B;圖示![開啟記錄圖示](assets/open-record-icon-on-planning-connection-custom-form.png)，以在Workfront Planning中開啟記錄。
Workfront Planning記錄詳細資料預覽方塊開啟。
1. 檢閱或編輯紀錄的相關資訊，或按一下&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤中開啟記錄](assets/open-details-in-a-new-tab-icon.png)以開啟紀錄詳細資訊頁面。

1. （選擇性）從Workfront中的自訂表單中，按一下記錄上的&#x200B;**移除**&#x200B;圖示![移除圖示](assets/remove-icon.png)，將其從Planning連線欄位中移除，並將其與Workfront物件中斷連線。
Workfront物件與Planning記錄中斷連線，且任何來自Workfront的查閱資訊都會從記錄中移除。

1. 按一下&#x200B;**儲存變更**&#x200B;以儲存自訂表格以及您對Workfront物件所做的任何其他變更。
