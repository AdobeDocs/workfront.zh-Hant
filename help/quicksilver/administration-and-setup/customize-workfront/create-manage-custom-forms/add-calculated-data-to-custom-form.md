---
title: 使用舊版表單產生器將計算資料新增至自訂表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 在自訂表單中，您可以建立計算自訂欄位以產生計算。 為此，您需要建立使用資料運算式和現有欄位名稱的陳述式，這些欄位可以是自訂欄位、計算自訂資料欄位和內建Workfront欄位。 此陳述式會計算您輸入的資料，並在新的計算自訂欄位中顯示結果。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: fac70de35b3380105911f2958f477f65c9999e55
workflow-type: tm+mt
source-wordcount: '2898'
ht-degree: 0%

---

# 使用舊版表單產生器將計算資料新增至自訂表單

<!--Audited: 01/2024-->

在自訂表單中，您可以新增計算自訂欄位，以在自訂表單附加至物件時，使用現有資料產生新資料。

為此，您需要建立使用資料運算式和現有欄位名稱的陳述式，這些欄位可以是自訂欄位、計算自訂資料欄位和內建Adobe Workfront欄位。

此陳述式會計算您輸入的資料，並在新的計算自訂欄位中顯示結果。

計算自訂欄位可包含：

* 單一內建欄位的簡單參考。

  >[!INFO]
  >
  > **範例：** 若要計算專案與任務產生的收入，您可以建立包含內建欄位「實際收入」的計算自訂欄位。 當有人將自訂表單附加到專案或任務時，專案或任務的收入會顯示在欄位中。

* 參考一或多個欄位的運算式。 這些可以是自訂欄位、其他計算自訂欄位和內建欄位。

  >[!INFO]
  >
  >**範例：** 若要計算專案與任務產生的利潤，您可以建立名為「利潤」的計算自訂欄位，其中包含從收入中減去成本的數學運算式。
  >
  >若要這麼做，您可以使用數學運算式SUB （減）搭配內建的Workfront欄位「實際成本」和「實際收入」。
  >
  >在下列步驟中，您可以看到如何執行此範例。

如需為貴組織建立自訂表單的相關資訊，以及瞭解可與其建立關聯的欄位型別，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td><p>目前：計畫</p>
   或
   <p>新增：標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>管理自訂表單的存取權</p> </p> </td> 
  </tr>  
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取層級設定，請聯絡Workfront管理員。 如需存取需求的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 新增計算欄位至自訂表單 {#add-a-calculated-field-to-a-custom-form}

您既可以使用內建的Workfront欄位，也可以使用已在計算自訂欄位的運算式中建立的自訂欄位。

>[!IMPORTANT]
>
>在建立計算自訂欄位之前，請先識別要納入的現有欄位，以確定Workfront中存在計算所需的資料。

1. 開始建立或編輯自訂表單，如所述 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 在 **新增欄位** 標籤，按一下 **已計算**.

   在右側的顯示區域中，欄位顯示填入值12345。 這是一個指示器，提醒您在建立或編輯自訂表單時，該欄位是一個計算的自訂欄位。 當表單附加至物件且使用者填寫時，他們會在欄位中看到計算結果，而不是12345值。

1. 為計算欄位指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td>輸入欄位的標籤。 這是使用者使用自訂表單時看到的內容。 欄位 <b>名稱</b>，會自動填入並符合標籤，因此Workfront在報表中會參照。 這是必填欄位。</td> 
     </tr>

   <tr> 
   <td role="rowheader">姓名</td> 
   <td>依預設，欄位的「名稱」與「標籤」相同。 不過，您可以修改欄位的「名稱」，使其與欄位的「標籤」不同。 欄位 <b>名稱</b> 在報表中由Workfront參照。 這是必填欄位。</td> 
   </tr>

   <tr> 
     <td role="rowheader" id="instructions">指示</td> 
      <td> <p>新增文字以提供有關欄位及其公式的其他資訊。</p>
      <p>您也可以在此處貼上用於計算自訂欄位的公式。 在這種情況下，我們建議您先更新自訂欄位的「計算」，然後從「計算」欄位複製最終運算式，並將其貼到「指示」欄位中。 </p>


   此功能可用於下列用途：
   <ul> 
      <li> <p>提醒您公式是什麼及其運作方式。 如果您打算在多個表單上使用此計算自訂欄位，這會特別實用。</p> </li> 
       <li> <p>當使用者將游標停留在欄位上時，即可看到工具提示。 您可以在此處新增任何您希望他們在工具提示中看到的文字。</p> </li> 
       </ul>
       <p>如果您不希望使用者在工具提示中看到公式，這會讓他們感到困惑，請勿將其新增到指示欄位。 請改用「在指示中顯示公式」設定來顯示或隱藏公式，如本文進一步所述 <a href="#build-the-calculation-for-your-calculated-custom-field">為您的計算自訂欄位建立計算</a> 本文章內容。</p>

   <p>如需有關在新表單上使用相同計算自訂欄位的資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">在自訂表單中重複使用現有的計算自訂欄位</a>.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td> 
      <td> <p>您希望儲存並顯示欄位結果的格式。</p> <p>如果您打算在數學計算中使用欄位，請一律使用 <strong>數字</strong> 或 <strong>貨幣</strong> 格式。 當您選取「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</p> 
      <p><b>重要</b>： <p>在選擇格式之前，請考慮新欄位的正確格式。 儲存自訂表單後無法編輯格式欄位。 選擇錯誤的格式可能會影響未來的計算，以及報告和清單分組中的彙總值。</p>
      <p><strong>注意：</strong> 使用貨幣格式的計算欄位不應包含引號。 （例如，使用800.00而非「800.00」。） 使用引號可能會由於貨幣型別的語言格式細微差別而造成非預期的後果。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 如區段所述，繼續更新自訂欄位資訊 [為您的計算自訂欄位建立計算](#build-the-calculation-for-your-calculated-custom-field) 本文章內容。

## 為您的計算自訂欄位建立計算 {#build-the-calculation-for-your-calculated-custom-field}

1. 開始建立計算自訂欄位，如區段中所述 [新增計算欄位至自訂表單](#add-a-calculated-field-to-a-custom-form) 本文章內容。

1. 按一下 **最大化** 以開啟 **計算編輯器** 並建置您的計算。

   >[!INFO]
   >
   >**範例：** 使用本文簡介中的範例，您可以為專案和任務在自訂表單中建立名為「利潤」的計算自訂欄位。 此欄位可能包含顯示「實際收入」與「實際成本」之間差異的計算：
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >在此範例中， `SUB` 是運算式，而參考欄位為 `actualRevenue` 和 `actualCost`.

   計算通常以運算式開始，後面接著括弧，其中包含當自訂表單附加至物件時要參考的欄位。 如需可用運算式的詳細資訊，請參閱 [計算資料運算式的概觀](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   每個欄位都必須以大括弧括住，如區段中所述 [計算自訂欄位中所需的語法](#syntax-required-in-calculated-custom-fields) 本文章內容。 當您開始輸入欄位名稱時，系統會提供建議，您可以選取一個來將其插入計算。

   >[!NOTE]
   >
   >   您不能在計算中參考下列型別的欄位： 
   >   
   >   * 含格式的文字欄位
   >   * 說明文字。
   >   
   >   如需自訂欄位型別的相關資訊，請參閱 [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

1. 按一下「計算編輯器」方塊中的大型文字方塊，然後按一下「搜尋」或「展開」，再按一下 **運算式** 和 **欄位** 文字方塊右側的區段。 這會將它們新增至計算中。

   您也可以開始在大型文字方塊中輸入運算式或欄位，然後在顯示時選取該運算式或欄位。 每個專案在欄位中顯示為「F」，在運算式中顯示為「E」。

   如果您鍵入左括弧，則會自動新增右括弧。

   >[!TIP]
   >
   >您可以執行下列任一項作業，以取得計算的協助：
   > 
   >* 將滑鼠指標暫留在計算中的運算式上可檢視說明、示範其使用方式的範例，以及文章中其他資訊的「瞭解更多」連結 [計算資料運算式的概觀](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
   >  ![](assets/hover-expression-help-text.jpg)
   >* 使用顏色編碼來識別您新增的元件。 運算式會以藍色顯示，而欄位則會以綠色顯示。
   >  ![](assets/colors-fields-expressions.jpg)
   >* 立即尋找以粉紅色反白顯示的計算錯誤。 您可以將滑鼠停留在醒目提示的錯誤上，以顯示其原因的簡短說明。
   >  ![](assets/error-help.png)
   >* 在 **在現有物件上預覽** ，開始輸入Workfront物件的名稱，然後在其顯示在清單中時選取它。 這可讓您預覽將表單附加至物件時欄位的外觀。
   ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
   >  ![](assets/preview-calc.jpg)
   >* 使用左邊顯示的行號在長計算中參考運算式。

1. 按一下 **最小化** 當您完成計算自訂欄位的計算時。

   >[!NOTE]
   >
   >在右側的顯示區域中，欄位顯示填入值12345。 這是一個指示器，提醒您在建立或編輯自訂表單時，該欄位是一個計算的自訂欄位。 當表單附加至物件且使用者填寫時，他們會在欄位中看到計算結果，而不是12345值。

1. （可選）使用下列任一選項來進一步設定您的計算自訂欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新增邏輯</td> 
      <td>您可以新增顯示邏輯，以根據使用者在填寫表單時於前置的多重選擇欄位（下拉式清單、核取方塊或選項按鈕）中進行的至少一個選擇，決定是否要顯示計算欄位。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">新增顯示邏輯和略過邏輯至自訂表單</a>. <p>唯有在表單的計算自訂欄位前面至少有一個核取方塊、選項按鈕或下拉欄位時，才能使用此選項。 </p> <p>略過邏輯不適用於已計算的自訂欄位。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新先前的計算</td> 
      <td>當您編輯現有的計算自訂欄位時，可以選取此選項，以在儲存自訂表單時觸發計算中的更新。 當您儲存自訂表單時，只會發生一次。 執行此操作後，選項會回到其停用狀態。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在指示中顯示公式</td> 
      <td>如果您希望填寫自訂表單的使用者將游標停留在欄位上時檢視欄位公式，請將此選項保持啟用。 如需詳細資訊，請參閱以下資訊 <a href="#instructions" class="MCXref xref">指示</a> 此表格的舊版。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **完成** 在計算自訂欄位上完成所有變更時。

   或者，按一下 **套用** 如果您想要繼續將自訂欄位新增至表單，請到目前為止將變更套用至表單。

   或者，按一下 **儲存+關閉** 完成自訂表單上的所有變更時。
1. 若要驗證您的計算自訂欄位是否正常運作，請將自訂表單附加至物件，然後在計算自訂欄位中檢閱結果。

   有關附加自訂表單的說明，請參閱 [新增自訂表單至物件](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   如果您想以其他方式繼續建置自訂表單，您可以繼續檢視下列其中一篇文章：

   * [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [在自訂表單中定位自訂欄位和Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [新增顯示邏輯和略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [預覽並完成自訂表格](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 計算自訂欄位中所需的語法

自訂計算欄位中使用的每個欄位都必須使用以下說明的語法，並在每個欄位名稱兩側加上大括弧。 當您開始輸入欄位名稱時，系統會提供建議，您可以選取一個來將其插入計算。 如果您在計算中輸入的資料不正確，警告訊息會警告您。 除非編輯計算以包含有效欄位和有效的計算運算式，否則無法儲存表單。

>[!NOTE]
>
>目前，只有在您開始輸入要在自訂表單將附加到的物件上參考的欄位名稱時，系統才會提出建議，而不是在物件的父項上。

### 以大括弧括住欄位名稱

* 如果您希望計算參照內建欄位，欄位名稱必須用大括弧括住，並且必須格式化為顯示在Workfront資料庫中的格式。 您不能使用欄位在Workfront介面中顯示的名稱。

例如： `{actualRevenue}`

欄位名稱會區分大小寫，且必須以駝峰式大小寫格式顯示，如同它們在Workfront系統中顯示一樣。

* 如果您希望計算參照自訂欄位，欄位名稱必須用大括弧括住，並在前面加上 `DE:` 括弧內。 自訂欄位區分大小寫，且必須如Workfront介面中所顯示的那樣格式化。

例如： `{DE:Profit}`

系統列出您在輸入時可以選擇的所有自訂欄位 `DE:`.

* 如果您希望計算參照在自訂表單附加至物件時，會從父物件提取資料的欄位，則必須在欄位名稱前面加上父物件的物件型別，同樣位於大括弧中。

  例如，如果自訂表單設定為與任務搭配使用，而您希望欄位在表單附加到任務時計算父級物件的實際收入，則您需要指示 `project` 做為欄位的物件型別：

  `{project}.{actualRevenue}`

  或者，如果是自訂欄位：

  `{project}.{DE:profit}`

  如果您不確定由於自訂表單是針對多個物件型別而設定了父物件的物件型別，則可以使用萬用字元篩選變數 `$$OBJCODE` 讓計算適用於每種可能的型別。 如需詳細資訊，請參閱 [多物件自訂表單中的已計算自訂欄位](#calculated-custom-fields-in-multi-object-custom-forms) 本文章內容。

### 使用句點分隔專案

當您在計算的自訂欄位中參考相關物件時，必須使用句點分隔物件名稱和屬性。

例如，在任務型別自訂表單中，若要在計算的自訂欄位中顯示Portfolio擁有者的名稱，您可以輸入下列內容：

`{project}.{porfolio}.{owner}`

此系統會依照下列步驟（依此順序）擷取資訊：

1. 從自訂表單的物件（任務），然後
1. 存取任務的父系或其他相關物件（專案），然後
1. 存取專案的父系或其他相關物件（專案組合），然後
1. 存取投資組合（投資組合的擁有者）的下一個相關物件。

### 參照自訂欄位的名稱語法

當您在計算的自訂欄位中參考另一個自訂欄位時，您需要輸入顯示在Workfront介面中的欄位名稱。

例如，若要參照在標示為Executive supporter的自訂欄位中選取的選項，您可以輸入以下內容：

`{DE:Executive sponsor}`

>[!NOTE]
>
>自動提示欄位的語法與其他型別的欄位不同，因為您需要新增 `:name` 在結尾處。
>
>例如，若要參照在名為「高階主管支援人」的自訂預先輸入欄位中選取的選項，您可以輸入：
>
>`{DE:Executive sponsor:name}`

## 多物件自訂表單中的已計算自訂欄位 {#calculated-custom-fields-in-multi-object-custom-forms}

在多物件自訂表單中，選取的物件型別必須與表單的計算自訂欄位中參考的所有欄位相容。 如果發生不相容的情況，訊息會警告您進行調整。

>[!INFO]
>
>**範例：**
>
>在設定為與Task物件型別搭配使用的自訂表單中，您會建立名為「負責」的計算自訂欄位。 您可將其設定為參考內建欄位，以便在表單附加至任務時，顯示負責的主要受指派人名稱：
>
>`{assignedTo}.{name}`
>
>您稍後會將Project物件型別新增至自訂表單。 警告訊息會告訴您Project物件型別與計算的自訂欄位不相容。

發生此情況時，您可以執行下列任一項作業：

* 從自訂表單中移除兩個不相容的專案之一：物件型別或參照的計算自訂欄位。
* 保留這兩個專案並使用萬用字元篩選器變數 `$$OBJCODE` 作為IF運算式中的條件，以建立兩個不同版本的In Charge欄位。 這允許欄位成功運作，無論表單附加到的物件型別為何。

>[!INFO]
>
>**範例：** 雖然專案中沒有「指派至：名稱」欄位，但有一個內建的「擁有者」欄位（除非有人手動變更此欄位，否則會自動填入建立專案者的名稱）。
>
>因此，在您的自訂負責欄位中，您可以使用 `$$OBJCODE` 如下所示，當自訂表單附加到專案時，這是參考「所有者」欄位，而當表單附加到任務時，這是參考「指派給：名稱」欄位：
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

如需變數的詳細資訊，例如 `$$OBJCODE,` 另請參閱 [萬用字元篩選器變數概觀](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 自動更新計算的自訂欄位

當發生下列情況時，會自動重新計算物件上的已計算自訂欄位：

* 物件上的某些專案會變更，例如每日時間表計算。
* 有人編輯物件上計算自訂欄位參考的另一個欄位。
* 計算的運算式是空的，而欄位包含一個值 — 這會將值設定為null。

  >[!NOTE]
  >
  ><div>在附加到物件的自訂表單中，已計算自訂欄位中的日期和時間陳述式會根據世界協調時間(UTC)進行計算和儲存，而不是根據為組織執行個體和使用者設定檔設定的時區設定。 自訂表單中的計算是根據每位使用者的個別時區產生。</div>
