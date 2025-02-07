---
user-type: administrator
product-area: system-administration
keywords: kickstart，kick-start，kickstart，kick-start
navigation-topic: use-kick-starts
title: 使用Kick-Start範本將資料匯入Workfront
description: Kick-Start是特別格式化的Excel活頁簿，可填入您要匯入Workfront的資料。 Adobe Workfront提供了一個Kick-Start範本，您可以使用它來執行此操作，如Kick-Start資料匯入工具中所述。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '2754'
ht-degree: 6%

---

# 使用Kick-Start範本將資料匯入Workfront

<!--Audited: 12/2023-->

Kick-Start是特別格式化的Excel活頁簿，可填入您要匯入Workfront的資料。 Adobe Workfront提供您可用來執行此動作的Kick-Start範本，如[Kick-Start資料匯入工具](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md)中所述。

此程式分為3項主要工作：

* 首先，您將Kick-Start範本匯出為試算表檔案
* 接著，將您的資料填入試算表中
* 最後，將填入的試算表匯入Workfront

本文會以適當的順序概述其中的每個程式。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td>
   <p> 新增：標準</p>
   或
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 限制

您可以使用Kick-Start範本，將大量物件匯入Workfront。 但是，請考量下列限制：

* 以這種方式匯入資料不會更新Workfront中已存在之記錄的資訊。
* 您只能匯入新記錄及其資訊。
* 一次匯入不超過2,000筆記錄，以確保匯入不會逾時

## 將Kick-Start範本匯出為試算表檔案

匯出Kick-Start範本時，您會收到空白的Excel試算表活頁簿。 將試算表下載到您的電腦後，您可以使用試算表來填入您的資訊，然後將其匯入Workfront。

匯出Kick-Start範本：

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  -->

1. 按一下&#x200B;**系統** > **匯入資料(Kick-Starts)**。

1. 選取您要包含的資訊型別。

   您選取的每個選項代表匯出試算表中多個索引標籤的集合。 例如，如果您選取&#x200B;**報表**&#x200B;選項，則建立報表所需的所有物件都會包含在試算表中（檢視、篩選器、群組、報表）。

   您可以使用下列所有物件型別，將資料匯入Workfront。 (唯一的例外是「存取層級」選項。 匯出中的「存取層級」資料表僅供參考之用，可讓您依ID將存取層級指派給新的使用者帳戶。)

   每個物件型別的範本都可以以下列檔案格式匯出，並包含下列頁面：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>物件</strong> </p> </th> 
      <th> <p><strong>匯出為</strong> </p> </th> 
      <th> <p>匯出的試算表中有<strong>張工作表</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>儀表板</p> <p>系統中的所有儀表板都可以匯出。 您在一次匯出中最多可以選取100個特定儀表板。</p> </td> 
      <td scope="col">匯出為ZIP檔案</td> 
      <td scope="col"> <p>參數</p> <p>描述文字</p><p>參數選項</p> <p>參數群組</p> <p>類別參數</p> <p>類別</p> <p>報告</p> <p>入口網站頁籤區段</p> <p>儀表板</p> <p>偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>報告</p> <p>系統中的所有報表都可以匯出。 您在一次匯出中最多可以選取100個特定報告。</p> <p>Kick-Starts不支援文字模式篩選器或群組。 若要成功匯出，報表篩選器和群組必須切換至「標準模式」。</p> </td> 
      <td scope="col">匯出為ZIP檔案 </td> 
      <td scope="col"> <p scope="col">參數</p> <p scope="col">描述文字</p> <p scope="col">參數選項</p> <p scope="col">參數群組</p> <p scope="col">類別參數</p> <p scope="col">類別</p> <p scope="col">報告</p> <p scope="col">偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>核准</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td scope="col"> <p>階段核准者</p> <p>核准階段</p> <p>核准</p> <p>核准流程</p> <p>偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>自訂資料</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td scope="col"> <p>參數</p> <p>描述文字</p>  <p>參數選項</p> <p>參數群組</p> <p>類別參數</p> <p>類別</p> <p>偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>費用類型</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td> <p>費用類型</p> <p>偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td> <p>時數類型</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td> <p>時數類型</p> <p>偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td> <p>團隊</p> </td> 
      <td scope="col"> <p>匯出為Excel檔案</p> </td> 
      <td> <p> 小組成員</p> <p>團隊</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td> <p>使用者</p> </td> 
      <td> <p>匯出為Excel檔案。 若要檢視完整的選項清單，請按一下<strong>其他選項</strong>。</p> </td> 
      <td> <p>使用者</p> <p>偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td>存取層級</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p>存取層級</p> <p>偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td>指派</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p>指派</p> <p>偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td>公司</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 公司</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>電子郵件範本</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p>電子郵件範本</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>費用</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 費用'</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>外部頁面</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 外部頁面</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>篩選器</td> 
      <td>匯出為ZIP檔案</td> 
      <td> <p> 篩選器</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>群組</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 群組</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>分組</td> 
      <td>匯出為ZIP檔案</td> 
      <td> <p> 分組</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>小時</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 小時</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>問題</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 問題</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>職務角色</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 工作角色</p> <p>偏好設定 </p> </td> 
     </tr>

   <tr> 
      <td>里程碑路徑</td> 
      <td> 匯出為Excel檔案</td> 
      <td> <p> 里程碑</p> <p>里程碑路徑</p> <p>偏好設定 </p> </td> 
     </tr>

   <tr> 
      <td>備註</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 備註</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>專案組合</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 專案組合</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>專案</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 佇列</p> <p>專案</p> <p>路由規則</p> <p>佇列主題</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>資源估計</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 資源估計</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>風險</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 風險</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>風險類型</td> 
      <td> 匯出為Excel檔案</td> 
      <td> <p> 風險類型</p> <p>偏好設定</p> </td> 
     </tr> 
     <tr> 
      <td>計分卡</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p>計分卡問題</p> <p>計分卡選項</p> <p>計分卡</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>任務</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 任務</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>範本</td> 
      <td> 匯出為Excel檔案</td> 
      <td> <p> 佇列</p> <p>範本</p> <p>路由規則</p> <p>佇列主題</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>範本指派</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 範本指派</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>範本任務</td> 
      <td>匯出為Excel檔案</td> 
      <td> <p> 範本任務</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>時程表</td> 
      <td> 匯出為Excel檔案</td> 
      <td> <p> 時程表設定檔</p> <p>時程表</p> <p>偏好設定 </p> </td> 
     </tr> 
     <tr> 
      <td>檢視 </td> 
      <td> <p>匯出為ZIP檔案</p> </td> 
      <td> <p> 檢視</p> <p>偏好設定 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**下載**。
1. 繼續進行[將您的資料填入試算表範本中](#populate-the-spreadsheet-template-with-your-data)，將您的資訊填入空白的範本試算表中。

## 將您的資料填入試算表範本中 {#populate-the-spreadsheet-template-with-your-data}

* [試算表中索引標籤（資料表）的概觀](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [匯入記錄](#import-a-record)
* [包含日期](#include-dates)
* [使用萬用字元](#use-wildcards)
* [ID的屬性名稱替代](#attribute-name-substitution-for-ids)

### 試算表中索引標籤（資料表）的概觀

>[!TIP]
>
>若要更清楚瞭解當您填入Kick-Start範本時如何需要格式化每個欄中的資訊，請考慮執行一個練習，使用您嘗試匯入物件上的現有Workfront資料匯出Kick-Start。 如需指示，請參閱[透過Kick-Starts從Adobe Workfront匯出資料](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)。

當您開啟空白的Kick-Start範本時，會有許多標籤（資料表）可供使用。 它們取決於您選取要下載的物件。 每一個都代表應用程式中的物件，例如專案、任務、小時、控制面板和使用者：

當您開啟其中一個標籤時，第2列會顯示每個物件在匯入期間可設定的欄位。 在欄標題中，在「set」一詞之後，欄位名稱會依其在資料庫中的顯示方式顯示。 這些欄位可作為欄標題。

>[!IMPORTANT]
>
>若要避免錯誤，請確定下列事項：
>
>* 請勿刪除Kick-Start試算表的空白第一列。
>* 請勿以任何方式刪除、修改或重新排列這些欄位（欄標題）。 例如，請勿變更其順序或名稱。
>* 將值新增至欄標題中以粗體顯示的每個欄位。 這些代表必填欄位。
>
>     但是，如果必要欄位包含系統偏好設定中設定的預設值，則不需要填入該欄位。
>
>     例如，在&#x200B;**PROJ專案**&#x200B;索引標籤上，**setCondition**&#x200B;和&#x200B;**setConditionType**&#x200B;欄位可以保留空白，但&#x200B;**setGroupID**&#x200B;和&#x200B;**setName**&#x200B;欄不能保留空白。
>
>* 系統會自動產生某些欄位，包括&#x200B;**setResourceRevenue**&#x200B;和&#x200B;**setEnteredByID**。 如果您在試算表中輸入這些欄位的資料，當您上傳試算表時，kick-start程式會覆寫資料。

### 匯入記錄  {#import-a-record}

工作表的每一列都對應一個唯一物件。

1. 在&#x200B;**isNew**&#x200B;欄中新增資訊：

   * 如果您要匯入的物件是新的，請輸入&#x200B;**TRUE**&#x200B;以匯入資料列中的資料。 此值區分大小寫，且必須一律使用大寫字母
   * 如果物件已在Workfront中，請在&#x200B;**isNew**&#x200B;欄中輸入&#x200B;**FALSE**&#x200B;以忽略該列。 此值區分大小寫，且必須一律使用大寫字母

      * Workfront中已存在的記錄不會更新。
      * 如果您從Workfront下載含有資料的範本，則現有物件已標示&#x200B;**FALSE**。
      * 如果您下載了空白範本，則不需要為現有物件新增列。

1. 以下列其中一種方式在&#x200B;**ID**&#x200B;欄中新增資訊：

   * 如果您要匯入的物件是新的（而且您在&#x200B;**isNew**&#x200B;資料行中輸入&#x200B;**TRUE**），請為ID輸入任何數字。 此數字在試算表中必須是唯一的。 例如，如果您匯入三個物件，您可以分別賦予它們ID 1、2、3。

   * 如果物件已存在於Workfront中（且&#x200B;**FALSE**&#x200B;位於&#x200B;**isNew**&#x200B;欄），而您正在匯入現有物件的相關新資訊，則ID必須是Workfront中該物件的英數字元GUID。

   >[!TIP]
   >
   > 若要在Workfront中找出物件的唯一GUID，您可以為該物件建立報表，並將ID欄新增至報表。 該欄中每個物件的值是物件的GUID。

   * Workfront中已存在的記錄不會更新。
   * 如果您下載含有資料的範本，則現有物件已包含GUID作為ID。
   * 您可以在&#x200B;**isNew**&#x200B;資料行中將&#x200B;**FALSE**&#x200B;變更為&#x200B;**TRUE**、變更ID，並在匯入前進行必要的資料調整，以根據現有物件匯入新的物件。

   ![群組的範例ID](assets/kick-start-group-example.png)

   * 匯入專案時，您必須指定群組ID。

      * 如果群組已存在於Workfront中，您必須將其唯一識別碼新增至專案的&#x200B;**setGroupID**&#x200B;欄位。
      * 如果Workfront中不存在群組，您可以將&#x200B;**群組群組**&#x200B;工作表新增至匯入檔案，將「群組」工作表上的&#x200B;**isNew**&#x200B;欄位設定為&#x200B;**TRUE**，並在&#x200B;**ID**&#x200B;欄位中指出新群組的數值ID。 新專案的&#x200B;**setGroupID**&#x200B;欄位必須與新群組的數值&#x200B;**ID**&#x200B;相符。

     **範例：**&#x200B;針對專案，**setGroupID**&#x200B;資料行中顯示的值必須是下列其中一項：

      * Workfront例項中現有群組的GUID
      * **群組群組**&#x200B;工作表上ID資料欄中的值（數字） （如果您在匯入期間建立新群組）

1. 必要欄位的輸入值，以及您要在匯入期間填入的任何其他欄位。
1. （選用）若要新增自訂資料：

   * 為您要納入匯入程式的每個自訂欄位建立新欄。
   * 為對應自訂欄位命名每個新欄位，如下所示： **DE：[自訂欄位在Workfront中出現的名稱]**。 例如，您可以建立下列自訂欄位：&quot;DE： Departments&quot;。
   * 在&#x200B;**setCategoryID**&#x200B;欄中，輸入此自訂欄位所在的現有自訂表單的GUID。 匯入自訂資料時，此欄位是必填欄位。
   * 如果您需要在自訂欄位中新增多個資料值（例如單選按鈕、核取方塊或清單），請使用「偏好設定」標籤中列出的垂直列自訂資料分隔符號「|」來分隔值。

     **範例：**&#x200B;在DE：Departments欄下輸入A|D以填入自訂表單中的部門A和部門D。

### 包含日期  {#include-dates}

Workfront可以處理大部分的日期格式。 不過，您必須確保試算表中的日期欄會格式化為日期。 如果欄的格式是一般、數字或文字，匯入將會失敗。

>[!TIP]
>
>最受歡迎的格式為YYYY/MM/DD格式。
>
>例如：07/10/2023。

Workfront也接受時間值做為日期的一部分。

例如：07/10/2022 01:30或07/10/2022 1:00 PM。

如果您在日期中省略時間，Workfront會執行下列任一項作業：

* 假設時間是凌晨12:00。 為了檢視您預期的日期結果，系統時區必須與您的時區相符。
* 如果它位在與排程相關聯的物件上，則時間會遞延至排程允許的最早時間。

>[!NOTE]
>
>使用UNIX時間戳記時，必須在值的末尾加上三個額外的零。
>
>例如，如果您的時間戳記是7336899000的，您會在儲存格中輸入7336899000000。

### 使用萬用字元 {#use-wildcards}

填入Kick-Start範本試算表時，您可以使用下列萬用字元：

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
   <td> <p>$$今天</p> </td> 
   <td> <p>在<strong>setDate</strong>欄位上使用時，此萬用字元會將日期設定為您匯入Kick-Start當天的午夜。</p> <p>您可以使用篩選器上允許搭配萬用字元的標準語法，來修改萬用字元。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>若您想要專案在匯入當週的星期一開始，無論您實際執行匯入的日期為何，都可以使用<strong>$$TODAYbw</strong>。 這會將您的專案計劃開始日期設定為星期日凌晨12:00。 由於專案排程此時可能不允許工作，因此將於星期一上午9:00開始。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>在<strong>setDate</strong>欄位上使用時，此萬用字元會根據您在Kick-Start匯入期間建立記錄的時刻設定日期。</p> <p>您可以使用篩選器上允許搭配萬用字元的標準語法，來修改萬用字元。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果您希望專案在匯入後3小時開始，可以使用<strong>$$NOW+3h</strong>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>在<strong>setAssignedToID</strong>或其他以使用者ID為基礎的欄位上使用時，此萬用字元會指派工作或以其他方式將記錄與執行匯入的個人建立關聯。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$客戶</p> </td> 
   <td> <p>這是特別為Kick-Start使用者匯入新增的萬用字元。 建立Workfront帳戶時，會建立具有系統管理員存取層級的使用者。 在帳戶中建立其他使用者時，指派給預設管理員的使用者名稱可以當做前置詞。</p> <p>由於使用者名稱在所有客戶中必須是唯一的，因此如果您有多個個人使用非常常見的使用者名稱，例如John Smith，他可能會有一個使用者名稱「jsmith」，這個選項會很有用。 在使用者名稱指派前面加上預設的管理員使用者名稱，即可保證每個使用者名稱都是唯一的（例如： <strong>$$CUSTOMER.jsmith</strong>）。</p> <p>提示：若要確保使用者名稱在整個系統內是唯一的，更輕鬆的方式是在<strong>setUsername</strong>欄位中輸入個人的電子郵件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

### ID的屬性名稱替代  {#attribute-name-substitution-for-ids}

雖然最佳做法是儘可能使用ID，但有時在設定&#x200B;**setAttributeID**&#x200B;值時，不方便將ID從一個工作表交叉參照到另一個工作表。 只要變更欄標題，您就可以依名稱參考值。

**範例：**

* **專案匯入**

  匯入專案時，請移至&#x200B;**群組群組**&#x200B;工作表，記下個別群組識別碼，並將它們貼到&#x200B;**專案專案**&#x200B;工作表的正確儲存格（**setGroupID**&#x200B;欄）中，以設定專案的&#x200B;**setGroupID**。

  這在僅處理幾個群組和專案時是可行的，但如果您處理每個群組和專案，則不太現實。

  若要對上述範例進行屬性名稱替代，請將&#x200B;**setGroupID**&#x200B;欄標題變更為&#x200B;**#setGroupID群組名稱**。 然後，您可以依名稱參照每個專案的群組。

  >[!NOTE]
  >
  >使用「屬性名稱替代」的選項僅限於現有記錄的參照。 您無法在相同匯入中建立的物件使用名稱替代。

* **使用者匯入**

  匯入使用者時，從&#x200B;**ROLE Role**&#x200B;索引標籤上的角色清單中填入&#x200B;**setRoleID**。

  有些角色ID是用於帳戶中已存在的記錄，而其他角色ID則在匯入期間建立。

  對於指派給現有角色的新使用者記錄，您可以使用名稱替代。 對於指派給新匯入角色的新使用者記錄，您無法。

  以下說明如何在相同的匯入檔案中使用這兩種方法：

   * 在試算表中新增一欄至&#x200B;**setRoleID**&#x200B;欄的左側。
   * 為新資料行&#x200B;**命名#setRoleID角色名稱**。
   * 若要將角色指派給現有記錄，請在&#x200B;**#setRoleID ROLE name**&#x200B;欄位中輸入角色名稱。

     對於新角色記錄的角色指派，請在setRoleID中輸入您在ROLE Role工作表中指派的ID。

     ![使用者的角色ID](assets/set-role-id.png)

## 將試算表資料匯入Workfront

將資料填入Excel範本中後，您就可以將其資料上傳至Workfront。

Kick-Start匯入支援下列檔案型別：

* Excel (.xls或.xlsx)
* 壓縮的(.ZIP)檔案（僅包含.xlsx或.xls檔案）

  >[!NOTE]
  >
  >匯入參照下列物件的Excel試算表時，您必須使用.ZIP檔案：
  >
  >* 報告
  >* 文件
  >* 頭像
  >* 檢視、篩選或分組屬性檔案
  >
  >使用壓縮的匯入檔案時，.ZIP檔案的名稱必須與.xlsx或.xls檔案相同，而且所有檔案都必須處於相同的結構層級（沒有資料夾）。

若要將範本試算表資料匯入Workfront：

<!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. 按一下&#x200B;**系統** > **匯入資料(Kick-Starts)**。

1. 在&#x200B;**使用Kick-Start試算表上傳資料**&#x200B;區段中，按一下&#x200B;**選擇檔案**，然後瀏覽並選取填入的試算表。

1. 按一下&#x200B;**上傳。**

   如果Excel檔案上傳至Workfront需要5分鐘以上的時間，應用程式會逾時，且Workfront無法上傳檔案。

   嘗試以較小的物件批次匯入資料。

1. （視條件而定）如果您正在使用Workfront Fusion，現在可以開啟FLO或情境。
