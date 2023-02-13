---
user-type: administrator
product-area: system-administration
keywords: kickstart,kickstart,kickstarts,kickstarts
navigation-topic: use-kick-starts
title: 使用Kick-Start範本將資料匯入Adobe Workfront
description: 「開始」是特別格式的Excel活頁簿，可填入您要匯入至Workfront的資料。 Adobe Workfront提供您可用來執行此作業的Kick-Start範本，如Kick-Starts資料匯入工具中所述。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 4912349cbbc74a6f7587312e83297169ecd52f51
workflow-type: tm+mt
source-wordcount: '2412'
ht-degree: 8%

---

# 使用Kick-Start範本將資料匯入Adobe Workfront

「開始」是特別格式的Excel活頁簿，可填入您要匯入至Workfront的資料。 Adobe Workfront提供您可用來執行此動作的「啟動」範本，如 [Kick-Starts資料匯入工具](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

此程式分為3個主要工作：

* 首先，您將「啟動」範本匯出為試算表檔案
* 接著，您會將資料填入試算表
* 最後，將填入的試算表匯入Workfront

本條按適當順序列出了上述各程式。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 限制

您可以使用Kick-Start範本，將大量物件匯入Workfront。 但請考量下列限制：

* 以此方式匯入資料不會更新Workfront中已存在之記錄的資訊
* 您只能導入新記錄及其資訊
* 一次匯入不超過2,000筆記錄，以確保匯入不會逾時

## 將「啟動」範本匯出為試算表檔案

匯出「啟動」範本時，您會收到空白的Excel試算表活頁簿。 在本文後續的程式中，您會將您的資訊填入活頁簿，然後將其匯回Workfront。

要導出「啟動」模板：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **匯出資料（啟動）**.

1. 按一下 **更多選項**，然後選取您要包含的資訊類型。

   您選取的每個選項代表匯出試算表中多個索引標籤的集合。 例如，若您選取「報表」選項，則建立報表的所有必要物件都會包含在試算表中（檢視、篩選、群組、報表）。

   您可以使用下列所有物件類型，將資料匯入Workfront。 (唯一的例外是「存取層級」選項。 導出中的「訪問級別」資料表供參考，它允許您按ID將訪問級別分配給新用戶帳戶。)

   每種對象類型的模板均可以以下列檔案格式導出，並包含以下工作表：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>物件</strong> </p> </th> 
      <th> <p><strong>匯出為</strong> </p> </th> 
      <th> <p><strong>匯出試算表中的工作表</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>儀表板</p> <p>系統中的所有控制面板都可匯出。 在單次匯出中，最多可選取100個特定控制面板。</p> </td> 
      <td scope="col">匯出為ZIP檔案</td> 
      <td scope="col"> <p>參數</p> <p>參數選項</p> <p>參數群組</p> <p>類別參數</p> <p>類別</p> <p>報告</p> <p>入口網站頁籤區段</p> <p>儀表板</p> <p>喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>報告</p> <p>系統中的所有報表都可匯出。 在單一匯出中，最多可選取100個特定報表。</p> </td> 
      <td scope="col">匯出為ZIP檔案 </td> 
      <td scope="col"> <p scope="col">參數</p> <p scope="col">參數選項</p> <p scope="col">參數群組</p> <p scope="col">類別參數</p> <p scope="col">類別</p> <p scope="col">報告</p> <p scope="col">喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>核准</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td scope="col"> <p>步驟核准者</p> <p>核准步驟</p> <p>核准</p> <p>核准流程</p> <p>喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>自訂資料</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td scope="col"> <p>參數</p> <p>參數選項</p> <p>參數群組</p> <p>類別參數</p> <p>類別</p> <p>喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>費用類型</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td> <p>費用類型</p> <p>喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td> <p>時數類型</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td> <p>時數類型</p> <p>喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td> <p>團隊</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td> <p> 小組成員</p> <p>團隊</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td> <p>使用者</p> </td> 
      <td> <p>匯出為Excel檔案。 若要查看選項的完整清單，請按一下 <strong>更多選項</strong>.</p> </td> 
      <td> <p>使用者</p> <p>喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td>存取層級</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p>存取層級</p> <p>喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td>指派</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p>指派</p> <p>喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td>公司</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 公司</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>電子郵件範本</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p>電子郵件範本</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>費用</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 費用'</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>外部頁面</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 外部頁面</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>篩選器</td> 
      <td>匯出為ZIP檔案</td> 
      <td> <p> 篩選器</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>群組</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 群組</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>分組</td> 
      <td>匯出為ZIP檔案</td> 
      <td> <p> 分組</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>時數</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 時數</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>問題</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 問題</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>職務角色</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 工作角色</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>里程碑路徑</td> 
      <td> 匯出為Excel檔案</td> 
      <td> <p> 里程碑</p> <p>里程碑路徑</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>備註</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 備註</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>專案組合</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 專案組合</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>專案</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 佇列</p> <p>專案</p> <p>路由規則</p> <p>佇列主題</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>資源估計</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 資源估計</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>資源集區</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 資源集區</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>風險</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 風險</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>風險類型</td> 
      <td> 匯出為Excel檔案</td> 
      <td> <p> 風險類型</p> <p>喜好設定</p> </td> 
     </tr> 
     <tr> 
      <td>計分卡</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p>計分卡問題</p> <p>計分卡選項</p> <p>計分卡</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>任務</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 任務</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>範本</td> 
      <td> 匯出為Excel檔案</td> 
      <td> <p> 佇列</p> <p>範本</p> <p>路由規則</p> <p>佇列主題</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>範本指派</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 範本指派</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>範本任務</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 範本任務</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>時程表</td> 
      <td> 匯出為Excel檔案</td> 
      <td> <p> 時間表設定檔</p> <p>時程表</p> <p>喜好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>檢視 </td> 
      <td> <p>匯出為ZIP檔案</p> </td> 
      <td> <p> 檢視</p> <p>喜好設定 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **下載**.
1. 繼續 [將您的資料填入試算表範本中](#populate-the-spreadsheet-template-with-your-data) 填入範本中的資訊。

## 將您的資料填入試算表範本中 {#populate-the-spreadsheet-template-with-your-data}

* [關於試算表中包含的標籤（資料表）](#about-the-tabs-data-sheets-included-in-the-spreadsheet)
* [導入記錄](#import-a-record)
* [包含日期](#include-dates)
* [使用萬用字元](#use-wildcards)
* [ID的屬性名稱替代](#attribute-name-substitution-for-ids)

### 關於試算表中包含的標籤（資料表） {#about-the-tabs-data-sheets-included-in-the-spreadsheet}

>[!TIP]
>
>若要更清楚了解填入Kick-Start範本時，您需要如何設定每欄資訊的格式，請考慮在您嘗試匯入的物件上，以現有的Workfront資料匯出Kick-Start，以執行實務。 如需指示，請參閱 [透過Kick-Starts從Adobe Workfront匯出資料](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

當您開啟空白的「啟動」範本時，會有許多標籤（資料表）可供使用。 它們取決於您選取要下載的物件。 每個代表應用程式中的一個對象，如項目、任務、小時、儀表板和用戶：

開啟其中一個標籤時，第2行會顯示每個對象的欄位，這些欄位可在導入過程中設定。 在欄標題中，字詞&quot;set&quot;後，欄位名稱會如資料庫中所示顯示。 這些欄位可作為欄標題。

>[!IMPORTANT]
>
>若要避免錯誤，請確定下列事項：
>
>* 請勿以任何方式刪除或修改這些欄位。 例如，請勿變更其順序或名稱。
>* 以粗體顯示的欄標題填入每個欄位。 這些代表必填欄位。
>
>  但是，如果必填欄位包含系統首選項中設定的預設值，則無需填入該值。
>
>  例如，在 **PROJ項目** 標籤 **setCondition** 和 **setConditionType** 欄位可以留空，但 **setGroupID** 和 **setName** 欄不能。

### 導入記錄  {#import-a-record}

工作表的每一行都對應於一個唯一對象。

1. 填入 **isNew** 欄：

   * 如果要導入的對象是新的，請輸入 **TRUE** 匯入列中的資料。
   * 如果物件已在Workfront中，請輸入 **FALSE** 來忽略列。

1. 填入 **ID** 欄，其方法如下：

   * 如果您要匯入的物件為新物件(且您已輸入&#x200B;**TRUE** 在 **isNew** 欄)，指定ID的任何數字。 試算表中的此編號必須是唯一的。

   * 如果您要匯入的物件已存在於Workfront系統中(且您已輸入&#x200B;**FALSE** 在 **isNew** 欄)，則ID必須是Workfront中該物件的英數字元GUID。

      **範例：** 若為專案， **setGroupID** 欄必須是下列其中一項：

      * Workfront實例中現有組的GUID
      * ID欄中的值（數字） **群組** 表（如果要在導入期間建立新組）

         ![](assets/verysimplekickstartprojectimport-350x31.png)

1. 輸入要在匯入期間填入的必填欄位和任何其他欄位的值。
1. （選用）若要新增自訂資料：

   * 為要包含在匯入程式中的每個自訂欄位建立新欄。
   * 為其對應的自訂欄位命名每個新欄，如下所示： **DE:[顯示在Workfront中的自訂欄位名稱]**.
   * 在欄中 **setCategoryID**，鍵入此自定義欄位所在的現有自定義表單的GUID。 匯入自訂資料時，此欄位為必填欄位。
   * 如果您需要在自訂欄位中新增多個資料值（例如選項按鈕、核取方塊或清單），請使用「偏好設定」標籤中所列的垂直條自訂資料分隔字元「|」來分隔值。

      **範例：** 在「DE:Departments」(DE:Departments)列下鍵入A|D，以自定義表單填入部門A和部門D。

### 包含日期  {#include-dates}

Workfront可以處理大部分的日期格式。 不過，您必須確定試算表中的日期欄已格式化為日期。 如果欄的格式為一般、數字或文字，匯入將會失敗。

>[!TIP]
>
>大多數人認為最容易使用MM/DD/YYYY格式(例如：07/10/2022)。

Workfront也接受時間值作為日期的一部分(例如：07/10/2022 01:30或07/10/2022下午1:00)。

如果您忽略日期中的時間，Workfront會執行下列其中一項作業：

* 假設為凌晨12:00。 若要查看您預期的日期結果，系統時區必須符合您的時區。
* 如果它位於與計畫關聯的對象上，則時間將預定到計畫允許的最早時間。

>[!NOTE]
>
>使用UNIX時間戳時，您必須在值的結尾處加上三個附加零。
>
>例如，如果時間戳記為7336899000，您會在儲存格中輸入7336899000000。

### 使用萬用字元 {#use-wildcards}

在填入Kick-Start範本試算表時，您可以使用下列萬用字元：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>萬用字元</strong> </p> </th> 
   <th> <p><strong>行為</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>今天$</p> </td> 
   <td> <p>當用於 <strong>setDate</strong> 欄位中，此萬用字元會將日期設為匯入「啟動」當天的午夜。</p> <p>您可以使用篩選器上包含萬用字元的標準語法來修改萬用字元。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果您希望某個專案在匯入的當周的星期一開始，而無論您實際執行匯入的日期為何，您可以使用 <strong>$$TODAYbw</strong>. 這會將您專案的計劃開始日期設定為星期日凌晨12:00。 由於該項目的時間表當時可能不允許工作，因此它將在星期一上午9:00開始。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$NOW</p> </td> 
   <td> <p>當用於 <strong>setDate</strong> 欄位中，此通配符會根據您在「啟動」導入期間建立記錄的時間設定日期。</p> <p>您可以使用篩選器上包含萬用字元的標準語法來修改萬用字元。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果您希望專案在匯入後3小時開始，可以使用 <strong>$$NOW+3小時</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>當用於 <strong>setAssignedToID</strong> 或其他基於userID的欄位，此通配符將分配工作，或者將記錄與執行導入的個人關聯。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$客戶</p> </td> 
   <td> <p>此萬用字元是專為Kick-Start使用者匯入而新增。 建立Workfront帳戶時，會建立具有系統管理員存取層級的使用者。 在帳戶中建立其他使用者時，指派給預設管理員的使用者名稱可作為前置詞。</p> <p>因為使用者名稱在所有客戶中必須是唯一的，因此當您有幾個人使用非常常見的使用者名稱（例如John Smith），而他們可能使用「jsmith」使用者名稱時，這個用法就很有用。 使用預設的管理員用戶名預先指定用戶名，可保證每個用戶名都是唯一的(例如： <strong>$$CUSTOMER.jsmith</strong>)。</p> <p>提示：若要確保使用者名稱在系統範圍內是唯一的，更優雅的方式是在 <strong>setUsername</strong> 欄位。</p> </td> 
  </tr> 
 </tbody> 
</table>

### ID的屬性名稱替代  {#attribute-name-substitution-for-ids}

儘管盡可能使用ID是最佳作法，但有時在設定 **setAttributeID** 值。 只需變更欄標題，即可依名稱參考值。

**範例:**

* **（項目導入）**

   匯入專案時，請設定 **setGroupID** 來執行 **群組** 表格，記下個別群組ID，並貼到正確的儲存格(**setGroupID** 欄) **PROJ項目** 頁簽。

   這在只處理幾個群組和專案時是可行的，但若您處理其中的數個群組和專案，則不實用。

   要執行上述示例的「屬性名稱替代」，請更改 **setGroupID** 欄標題 **#setGroupID組****名**. 然後，您可以依名稱參考每個專案的群組。

   >[!NOTE]
   >
   >使用「屬性名稱替代」的選項僅限於現有記錄的引用。 不能對在同一導入中建立的對象使用名稱替代。

* **（使用者匯入）**

   匯入使用者時，請填入 **setRoleID** 從 **角色角色** 標籤。

   有些角色ID是用於帳戶中已存在的記錄，有些則是在匯入期間建立。

   對於分配給現有角色的新用戶記錄，可以使用名稱替代。 對於分配給新導入角色的新用戶記錄，不能。

   以下說明如何在相同的匯入檔案上使用兩種方法：

   * 在試算表的左側新增欄 **setRoleID** 欄。
   * 為新列命名 **#setRoleID角色名稱**.
   * 對於分配給現有記錄的角色，請在 **#setRoleID角色名稱** 欄。

      對於新角色記錄的角色分配，請在setRoleID的「角色」工作表中輸入您在ID。

      ![](assets/setroleid-350x66.png)

## 將試算表資料匯入Workfront

將資料填入Excel範本後，可將其資料上傳至Workfront。

「啟動」匯入支援下列檔案類型：

* 基於XML的Excel(&#42;.xlsx)
* 舊版Excel(&#42;.xls)
* 壓縮(&#42;ZIP)xlsx或xls檔案

   >[!NOTE]
   >
   >當匯入的 Excel 試算表參考了報告、文件、顯示圖片；或檢視、篩選或分組屬性檔案時，您必須使用 ZIP 檔案。使用壓縮的匯入檔案時， &#42;ZIP檔案的名稱必須與 &#42;.xlsx或 &#42;.xls檔案，且所有內容必須位於相同的檔案結構層級（無資料夾）。


若要將範本試算表資料匯入Workfront:

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** >**匯入資料（啟動）**.

1. 在 **使用Kick-Start試算表上傳資料** ，按一下 **選擇檔案**，然後瀏覽並選取填入的試算表。

1. 按一下 **上傳。**

   如果Excel檔案上傳至Workfront的時間超過5分鐘，應用程式會逾時，且無法上傳檔案。

   嘗試以較小的對象批次導入資料。

1. （條件性）如果您使用Workfront Fusion，現在可以開啟FLO或案例。
