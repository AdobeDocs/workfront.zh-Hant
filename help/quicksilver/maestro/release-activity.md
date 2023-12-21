---
title: Adobe大師發行活動
description: Adobe Maestro目前可供特定Workfront客戶使用。 請經常閱讀本文章，瞭解最近為Adobe Maestro發行的功能。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 5d8e189f01a52b2d1b605b497ed17737fb0a0924
workflow-type: tm+mt
source-wordcount: '2890'
ht-degree: 0%

---

# Adobe大師發行活動

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能使用Maestro功能。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro/maestro-overview.md).

本文列出2023年5月22日Maestro封閉Beta版計畫推出後所發行的功能。

已發行的功能會依其發行順序列出，最新的排在前。 參與Maestro封閉測試版計畫的客戶可以存取其預覽和生產環境中的所有功能。

>[!IMPORTANT]
>
>在功能發行至生產環境後的某個時間，將可使用以下各節中參考的檔案。

本節列出2023年5月22日Maestro封閉Beta版計畫推出後所發行的功能和修補程式。

功能每週都會發行，並依發行順序列出，最新的則排在前。 參與Maestro封閉測試版計畫的客戶可以存取其預覽和生產環境中的所有功能。

<!--
## Week of November 27, 2023

### Maestro permissions for users and groups

Production: November 28, 2023

>[!IMPORTANT]
>
>This functionality is not yet available in Preview.

You can now share a workspace with users and groups. You can set their permissions to different levels, depending on what information they need to view or edit in a Maestro workspace. After you share permissions to a workspace, users have permissions to the record types, records, and fields in that space.

The following are the permissions levels for Maestro workspaces:  

* None: Users cannot access any workspaces in Maestro, even if the Maestro area is shared with them through a layout template. 

* View: Users can view workspaces that are shared with them. They can also view record types, and records from the shared workspace. 

* Contribute: Users can create, edit, or delete records in the workspace that is shared with them.  They cannot create or edit record types or workspaces ones shared with them.  

* Manage: Users can create, edit, and delete record types, records, and fields in workspaces that are shared with them. They cannot create workspaces.  

Only Workfront administrators can create, edit, or delete workspaces and all information associated with them.  

For more information, see [Grant access to Adobe Maestro](../maestro/access/grant-access.md) and [Overview of sharing permissions in Adobe Maestro](../maestro/access/sharing-permissions-overview.md). -->

## 2024年12月18日當週

### 從詳細資訊頁面新增記錄註解

所有客戶的預覽和生產： 2023年12月18日

>[!NOTE]
>
>下列功能將於2024年1月版本中用於生產環境：
>
>* 搜尋註解
>
>* 複製並貼上影像
>
>* 拖放影像
>
>如需詳細資訊，請參閱 [2024年第一季版本總覽](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

您現在可以在詳細資訊頁面中檢視記錄時，新增評論或回覆其他人，以在個別記錄上與其他人共同作業。

Maestro記錄的註解體驗符合Workfront物件的新註解體驗。

如需詳細資訊，請參閱 [管理記錄註解](/help/quicksilver/maestro/records/manage-record-comments.md).

### Adobe Workfront Fusion的Maestro聯結器(Beta)

生產： 2023年12月21日

>[!IMPORTANT]
>
>貴組織必須購買Adobe Workfront Fusion，才能與Maestro建立連線。
>
>如需詳細資訊，請參閱 [Adobe Workfront Fusion概觀](/help/quicksilver/workfront-fusion/get-started/workfront-fusion-overview.md).

現在，您可以使用Adobe Workfront Fusion來連線到Maestro。 使用新的AdobeMaestro Fusion連線，您可以：

* 建立、讀取、更新和刪除記錄

* 依記錄型別取得記錄清單

* 刪除或取得記錄型別清單

* 搜尋記錄

* 進行API呼叫

* 在Maestro中進行變更時觸發案例

如需詳細資訊，請參閱 [Adobe大師模組](/help/quicksilver/workfront-fusion/apps-and-their-modules/maestro-modules.md).

## 2023年12月11日當週

### 更新記錄型別表格檢視中的主要欄位

預覽和生產： 2023年12月14日

您現在可以選擇要顯示在Maestro表格檢視的第一欄中的欄位。 此欄位現在稱為主要欄位。

在此增強功能之前，記錄的「名稱」欄位一律顯示在表格檢視的第一欄，且無法放置於其他位置。

改良後，請注意下列事項：

* 依預設，「名稱」欄或欄位仍然是表格的第一欄。

* 您可以選擇以下任何型別的欄位作為主要欄位，並取代第一欄中的「名稱」欄位：

   * 單行文字

   * 數字

   * 公式

     >[!NOTE]
     >
     >公式型別的欄位將在稍後日期發佈。

* 表格檢視的主要欄位一律凍結且無法移動，除非您將其他欄位設定為主要欄位。

* 您可以從非主要欄標題變更主要欄位。

* 記錄型別的所有表格檢視都具有您選取的相同主要欄位。

如需詳細資訊，請參閱 [管理表格檢視](/help/quicksilver/maestro/views/manage-the-table-view.md).


### 連結Maestro記錄與Adobe Experience Manager Assets

預覽版本： 2023年12月14日

生產版本： 2023年12月21日

>[!IMPORTANT]
>
>貴組織的Workfront執行個體必須上線至Adobe業務平台或Adobe Admin Console，才能將Maestro記錄連線至Adobe Experience Manager Assets。
>
>如果您對上線Adobe Admin Console有任何疑問，請參閱 [Adobe Unified Experience常見問題集](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).


您現在可以在Maestro記錄型別與Adobe Experience Manager Assets之間建立連線。

建立連線後，此更新便可使用下列功能：

* 您可以將Experience Manager資產和資料夾從Experience Manager Assets中他們有權存取的特定存放庫連結到Maestro記錄。 您可以在此程式中連線資產欄位至Maestro欄位。

* Maestro使用者可以檢視連線資產的名稱，以及Maestro中連線欄位的值

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Maestro after you establish the connection. Connected assets are visible in the Maestro table and timeline views of this new record type.  
-->

* 您可以從連線的記錄欄位按一下Maestro記錄表格檢視中的資產名稱，並檢視包含資產縮圖和數個關鍵欄位的快顯視窗。 從快顯視窗中，您可以導覽至Experience Manager中的資產檢視器，並檢視有關該檢視器的所有詳細資訊。

如需詳細資訊，請參閱 [連線記錄型別](/help/quicksilver/maestro/architecture/connect-record-types.md).

## 2023年12月4日當週

### 在Maestro表格檢視中，針對People-type和連結的記錄欄位，將資訊從一個欄位複製並貼到另一個欄位

預覽和生產： 2023年12月5日

您現在可以在Maestro記錄型別表格檢視中，將資訊從一個欄位複製並貼到另一個相同型別的欄位。 下列欄位型別現在支援此功能：

* 人員
* 連結的記錄欄位

請考量下列事項：

* 顯示多個值的欄位支援將欄位值從一個欄位複製和貼上到另一個欄位。

* 您無法從其他來源複製資訊，除了與貼上資訊的欄位型別相同的Maestro欄位之外。

* 您無法複製和貼上顯示在記錄之詳細資訊區域中的欄位值。

如需詳細資訊，請參閱 [編輯記錄](../maestro/records/edit-records.md).

如需連結欄位的詳細資訊，請參閱 [連線記錄型別](../maestro/architecture/connect-record-types.md).

## 2023年11月27日當週

### 在Maestro表格檢視中，將資訊從一個欄位複製並貼上到另一個欄位

預覽和生產： 2023年11月28日

您現在可以在Maestro記錄型別表格檢視中，將資訊從一個欄位複製並貼到另一個相同型別的欄位。

請考量下列事項：

* 您無法從其他來源複製資訊，除了與貼上資訊的欄位型別相同的Maestro欄位之外。

* 您無法複製和貼上顯示在記錄之詳細資訊區域中的欄位值。

* 您無法複製和貼上下列欄位型別的欄位值：

   * 人員

   * 系統欄位

   * 在連線記錄之後建立的連結欄位

如需詳細資訊，請參閱 [編輯記錄](../maestro/records/edit-records.md).

## 2023年11月6日當週

### 表格檢視的分組

預覽和生產： 2023年11月7日

您現在可以在記錄型別頁面的表格檢視中將記錄分組。 您可以在Maestro介面中依三個不重複欄位分組 <!--checking into this for now: and by four fields when using the API-->.

如需詳細資訊，請參閱 [管理表格檢視](../maestro/views/manage-the-table-view.md).

## 2023年10月30日當週

### 新的欄位型別和日期欄位，以擷取建立或上次修改記錄的人員或日期

預覽和生產： 2023年10月30日

我們為Maestro記錄引進了以下欄位型別：

* 建立者

* 建立日期

* 上次修改者

* 上次修改日期

從這些欄位型別建立的欄位值是唯讀的，並擷取建立或上次修改記錄的使用者名稱，或記錄建立或上次修改的日期。

如需詳細資訊，請參閱 [建立欄位](../maestro/fields/create-fields.md).

### 從Maestro記錄導覽至Workfront物件

預覽和生產： 2023年10月31日

您現在可以從Maestro的下列區域開啟Workfront物件頁面：

* 唯讀連結Workfront物件記錄表格檢視

* 唯讀Workfront物件記錄詳細資訊頁面

如需詳細資訊，請參閱 [連線記錄](../maestro/records/connect-records.md).

### 改善表格檢視中的導覽

預覽和生產： 2023年11月2日

我們已改善記錄型別頁面之表格檢視中的導覽。

以下是一些改善專案：

* 使用鍵盤上的Tab鍵來導覽表格的欄和列

* 從任何欄位置新增記錄。 在此改進之前，您只能從第一欄新增記錄。

* 使用Shift + Enter鍵盤組合在表格中新增記錄（或列）。

如需詳細資訊，請參閱 [建立記錄](../maestro/records/connect-records.md).

## 2023年10月16日起一週

### 新增人員欄位型別

預覽和生產： 2023年10月16日

您現在可以新增People-type欄位至Maestro記錄型別。 您可以使用「人員」型別欄位，將現有使用者與記錄建立關聯。 如需詳細資訊，請參閱 [建立欄位](../maestro/fields/create-fields.md).

### RTF格式 — 段落欄位格式

預覽和生產： 2023年10月16日

我們已為段落型別欄位新增RTF格式控制項。 您可以在記錄型別的表格檢視或記錄的詳細資訊頁面中使用RTF格式化段落欄位。 如需詳細資訊，請參閱 [編輯記錄](../maestro/records/edit-records.md).


### 時間軸檢視的記錄與群組色彩編碼

預覽和生產： 2023年10月19日

您現在可以對「時間軸」檢視中的記錄列和群組進行色彩編碼。

以下是「時間軸」檢視中，您可以選擇為記錄列和群組顯示的顏色選項：

* 群組可符合下列顏色：

   * 灰色（預設）

   * 您分組依據的欄位色彩

* 長條圖可以符合下列顏色：

   * 記錄型別的顏色

   * 您選取的欄位顏色

   * 群組的顏色

   * 無顏色（預設）

將顏色與特定欄位比對時，您只能選取具有顏色編碼選項的欄位。

如需詳細資訊，請參閱 [管理時間表檢視](../maestro/views/manage-the-timeline-view.md).

## 2023年10月9日當週

### 在表格檢視中搜尋

預覽和生產： 2023年10月9日

您現在可以搜尋關鍵字，以便在表格檢視中快速尋找記錄。 您可以在熒幕上顯示的任何欄位中使用關鍵字和特殊字元來尋找記錄。 如需詳細資訊，請參閱 [管理表格檢視](../maestro/views/manage-the-table-view.md).

## 2023年9月18日當週

### 重新排序列

預覽和生產： 2023年9月20日

您現在可以在記錄型別頁面的「表格」檢視中，重新排序一或多個列（或記錄）。 如需詳細資訊，請參閱 [管理表格檢視](../maestro/views/manage-the-table-view.md).

## 2023年9月4日當週

### 連結Maestro記錄與Workfront公司和群組

預覽和生產： 2023年9月5日

您現在可以連結Maestro記錄與Workfront公司和群組。 您必須先在Maestro記錄型別與Workfront公司和群組物件型別之間建立連線。 然後，您可以將所選記錄型別的單一Maestro記錄連線到個別Workfront公司和群組。

請考量下列事項：

* 您必須為每個Workspace在Maestro記錄型別與Workfront公司和群組物件型別之間建立連線。

* 您無法將分類記錄型別與Workfront物件型別連線。

* 您可以將多個Maestro記錄連線到同一個Workfront公司或群組，並將多個公司或群組連線到同一個Maestro記錄。

* 您無法在Maestro中編輯公司或群組。 檢閱Maestro連結的記錄時，在Workfront中執行的所有公司或群組變更都會顯示在Maestro中。

  如需詳細資訊，請參閱下列文章：

   * [連線記錄型別](../maestro/architecture/connect-record-types.md)
   * [連線記錄](../maestro/records/connect-records.md)

### 單行文字欄位的URL支援

預覽和生產： 2023年9月7日

為了在表格檢視中使用連結時提高可見度，我們在單行文字欄位中新增了對URL的支援。 更新單行文字欄位時，若使用其他網站或外部磁碟機的URL，現在可將這些URL識別為連結，並可讓您從表格中按一下這些URL。 在此增強功能之前，連結會顯示為文字。

## 2023年8月28日當週

### 「表格檢視」工具列的「欄位可見性」選單

預覽和生產： 2023年8月31日

若要顯示特定記錄集的正確資訊，尤其是如果您想要與必須看到某記錄型別之部分而非全部欄位的其他人共用檢視時，您現在可以選取要顯示哪些欄位（或欄），以及要隱藏哪些欄位在「表格」檢視中。

您可以從欄位欄的每個標題隱藏或顯示個別欄位，也可以從表格檢視工具列的設定管理記錄型別的所有欄位。

如需詳細資訊，請參閱 [管理表格檢視](../maestro/views/manage-the-table-view.md).

## 2023年8月21日起一週

### 將Maestro記錄連線到計畫和投資組合

預覽和生產： 2023年8月24日

您現在可以將Maestro記錄與Workfront計畫和產品組合連線。 您必須在Maestro記錄型別與建立連線欄位的方案或投資組合之間建立連線。 然後，您可以將來自相同工作區中所有其他記錄型別的任何Maestro記錄連線到特定計畫和產品組合，這些計畫和產品組合會在相同工作區中建立唯讀Workfront計畫或WorkfrontPortfolio記錄型別。 請考量下列事項：

* Workfront聯結器記錄型別對於每個工作區都是唯一的。
* 您可以將多個Maestro記錄連線到同一個Workfront計畫或產品組合，並將多個計畫和產品組合連線到同一個Maestro記錄。
* 您無法在Maestro中編輯計畫和投資組合。 檢閱連結的記錄時，在Workfront中執行的所有計畫和產品組合變更在Maestro中可見。

### 表格檢視的新排序功能

預覽和生產： 2023年8月24日

您現在可以在記錄型別頁面的表格檢視中排序記錄。
下列功能現已可用：

* 在表格層級排序，您可以同時依多個欄位排序。
* 在欄或欄位層級排序，您可以一次依個別欄位排序。

### 改進時間軸檢視：新的分組外觀和緊湊標準檢視切換器

預覽和生產： 2023年8月24日

我們已對時間表檢視進行下列改進：

* 您現在可以下列模式顯示時間軸檢視：

   * 標準：以個別的明細行顯示記錄。
   * 緊密：顯示日期在同一行上不相交的記錄。

* 我們已變更時間軸檢視中群組行的外觀，以顯示在其包含記錄的時間軸上方。 在此改善之前，群組線會跨時間軸的整個長度顯示。

## 2023年8月14日起一週

### 重新排序表格檢視中的欄

您現在可以在Maestro表格檢視中重新排序欄。 重新排序欄時，請考量下列事項：

* [名稱]欄位永遠是記錄型別頁面表格檢視中的第一個欄位

* 您無法將「名稱」欄位移至其他位置

* 「名稱」欄位已凍結，且不是水準捲動的一部分。

### 時間軸檢視的水準捲動

您現在可以在記錄型別的時間軸檢視中水準捲動。

## 2023年8月7日當週

### 從Excel檔案匯入記錄型別

預覽和生產： 2023年8月10日

您現在可以匯入Excel檔案，以在工作區中建立記錄型別。 檔案的頁面會成為記錄型別，而檔案的欄會成為各自的欄位。

### 改善連線記錄型別和專案的體驗

預覽和生產： 2023年8月10日

我們已改善您連線記錄型別的方式，包括連線至Workfront專案。 作為此改進的一部分，我們在從表格檢視中為記錄型別新增欄位時進行了以下變更：

* 已從「新欄位」索引標籤中移除「關係型別」欄位。

* 新增「新連線」索引標籤，您可以在此直接選取要連線的記錄或物件型別，而不需要「關係型別」欄位。

## 2023年7月10日起一週

### 更新記錄型別的外觀

預覽和生產： 2023年7月13日

您現在可以為記錄型別選取自訂圖示，並為記錄型別圖示選取自訂顏色。

### 新增核取方塊欄位型別

預覽和生產： 2023年7月13日

您現在可以將「核取方塊」欄位型別新增至Maestro記錄型別。 您可以使用Checkbox-type欄位，將單一核取方塊選項新增到記錄。 您可以使用此欄位來指示該特定記錄的特定屬性或狀態。 例如，您可以將其用作追蹤完成、核准或每個記錄的任何其他二進位屬性的標幟。

## 2023年6月26日起一週

### 快速啟用表格中的內容功能表

預覽和生產： 2023年6月28日

我們啟用了在表格檢視或記錄型別中檢視記錄時，以滑鼠右鍵按一下記錄列中的任何位置來啟動內容功能表的能力。 現在，當您從記錄型別的表格檢視中的任何位置存取內容功能表時，可以快速檢視、刪除或複製記錄之「詳細資訊」頁面的連結。 在此增強功能之前，內容功能表只能從記錄的「名稱」欄的「更多」功能表存取。

## 2023年6月19日起一週

### 記錄欄位名稱是唯一的

我們現在引入了一項要求，要求Maestro記錄型別的欄位名稱應具有唯一名稱。 屬於不同記錄型別的欄位不必有唯一名稱。

## 2023年6月5日起一週

### 將Maestro記錄連線至Workfront專案

預覽和生產： 2023年6月5日

您現在可以將Maestro記錄與Workfront專案連線。 您必須建立聯結器Maestro記錄型別，以建立Maestro記錄與Workfront專案之間的連線。 然後，您可以使用「關係」欄位，將所有其他記錄型別的任何Maestro記錄連線到聯結器記錄。 請考量下列事項：

* 您必須擁有每個工作區的Workfront聯結器記錄型別。
* 您可以將多個Maestro記錄連線到同一個Workfront專案，並將多個專案連線到同一個Maestro記錄。
* 您無法在Maestro編輯專案。 檢閱連結的記錄時，在Workfront中執行的所有專案變更都會顯示在Maestro中。

## 2023年5月29日起一週

### 建立時間表檢視的二日期需求

預覽和生產： 2023年5月31日

您必須至少有兩個與記錄型別相關聯的日期欄位，才能建立時間表檢視。
