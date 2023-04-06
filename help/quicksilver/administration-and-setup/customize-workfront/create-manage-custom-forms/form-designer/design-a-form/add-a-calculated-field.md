---
title: 使用表單設計器添加計算欄位
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 當自訂表單附加至物件時，您可以新增使用現有資料產生新資料的計算自訂欄位。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 使用表單設計器添加計算欄位

當自訂表單附加至物件時，您可以新增使用現有資料產生新資料的計算自訂欄位。

計算的自訂欄位可包含：

* 對單個內置欄位的簡單引用。

   >[!INFO]
   >
   > **範例：** 若要計算專案和任務產生的收入，您可以建立包含內建欄位「實際收入」的計算自訂欄位。 當某人將自訂表單附加至專案或任務時，專案或任務的收入會顯示在欄位中。

* 引用一個或多個欄位的表達式。 這些欄位可以是自訂欄位、其他計算的自訂欄位，以及內建欄位。

   >[!INFO]
   >
   >**範例：** 要計算由項目和任務生成的利潤，您可以建立一個名為「利潤」的計算自定義欄位，該欄位包含從收入中減去成本的數學表達式。
   >
   >要執行此操作，可以使用數學表達式SUB（減去）以及內置的Workfront欄位Actual Cost和Actual Revenue。
   >
   >在下列步驟中，您可以了解如何執行此範例。


## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 在自訂表單中重複使用現有的計算自訂欄位

您可以對屬於不同物件的自訂表單使用相同的計算自訂欄位。 例如，您可以使用為任務自定義表單上的項目自定義表單建立的「利潤」計算欄位。

使用現有的計算自訂欄位時，計算不會轉移至新表單。 您必須在相同欄位上，在新自訂表單上再次新增計算。

您也可以在新表單上對相同欄位進行不同的計算。 為計算的自訂欄位保留相同名稱，可確保命名慣例的緊密性和一致性。

>[!IMPORTANT]
>
>計算表達式中的更改可能會導致對象上的欄位值過期。 要確保始終查看這些欄位中的最新計算，請執行以下操作之一：
>
>* 在儲存您已以附加的自訂表單編輯資料的物件後，按一下「更多」圖示 ![](assets/more-icon.png) 在對象的首頁上，重新計算自定義表達式。
>* 在批量編輯對象時，選擇「重新計算自定義表達式」選項。
>* 在自訂表單上編輯「計算自訂欄位」時，選取「更新先前的計算」選項。


要重複使用現有計算的自定義欄位：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms** 中。

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. 按一下 **新自訂表單。**
1. 選取您要將自訂表單附加至哪些物件類型，然後按一下 **繼續**.

1. 在畫面左上方，按一下 **欄位程式庫**.

   ![](assets/field-library.png)

1. 使用搜尋方塊或展開 **計算** 區段來找出您需要的計算欄位，然後拖曳您要其顯示在自訂表單中的欄位。

1. （選用）重複上一步以新增任何其他欄位。

   >[!NOTE]
   >
   >在單一自訂表單中，最多可新增500個欄位和Widget。 但是，當表單上存在超過100個時，效能可能會降低，具體取決於表單的複雜性。
   >
   >
   >複雜表單的範例包括具有階層式參數的表單、計算的自訂資料欄位，以及單一欄位中的多個值選項。

1. 若要儲存變更，請按一下 **套用** 並移至其他區段，繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

## 新增計算欄位

>[!IMPORTANT]
>
>建立新的計算自訂欄位之前，請識別您要包含的現有欄位，以確定計算所需的資料存在於Workfront中。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms** 中。

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. 按一下 **新自訂表單。**
1. 選取您要將自訂表單附加至哪些物件類型，然後按一下 **繼續**.

1. 在畫面左側，尋找 **計算** 並拖曳至畫布上的區段。

   ![](assets/drag-field-to-section.png)

1. 在畫面右側，設定您所新增之自訂欄位類型可用的選項：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td>輸入欄位的標籤。 這是使用者在使用自訂表單時會看到的內容。 欄位 <b>名稱</b>，會自動填入，而Workfront會在報表中參照。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">指示</td> 
      <td> 依預設，您為欄位建立的公式會儲存在此處。 您可以新增文字，以提供關於欄位及其中公式的其他資訊。 這有兩種用處： 
       <ul> 
      <li><p>這提醒了我們，公式是什麼，它如何運作。 如果您打算在多個表單上使用此計算的自訂欄位，這個功能會特別實用。</p> </li> 
      <li> <p>使用者將游標暫留在欄位上時，可檢視工具提示。 您可以在此處新增任何文字，讓這些文字在工具提示中查看。</p> <p>如果您不希望他們在工具提示中看到公式（這可能會令他們困惑），可以隱藏它。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td> 
      <td> <p>要儲存和顯示欄位結果的格式。</p> <p>如果欄位將用於數學計算，請一律使用 <strong>數字</strong> 或 <strong>貨幣</strong> 格式。 選擇「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</p> 
      <p><b>重要</b>:在選擇格式之前，請考慮新欄位的正確格式。 自訂表單儲存後，無法編輯格式欄位。 而選擇錯誤的格式可能會影響報表和清單群組中的未來計算和匯總值。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **計算** 框中，開始構建計算：
   1. 按一下 **最大化** 開啟計算編輯器並建立計算。</p>
計算通常以表達式開頭，後跟括弧，其中包含自定義表單附加到對象時要引用的欄位。

      每個欄位都必須以大括弧包住。 當您開始輸入欄位名稱時，系統會提出建議，您可以選取一個欄位，以將其插入計算中。

+++ **展開以查看計算自訂欄位中所需的語法**

      每個欄位都必須使用下方說明的語法，每個欄位名稱周圍都帶有大括弧。 當您開始輸入欄位名稱時，系統會提出建議，您可以選取一個欄位，以將其插入計算中。 如果您在計算中輸入的資料不正確，會出現警告訊息提醒您。 除非編輯計算以包含有效欄位和有效的計算表達式，否則無法保存表單。

      >[!NOTE]
      >
      >目前，系統僅在您開始鍵入要在將附加自訂表單的對象上引用的欄位名稱時，才會提出建議。 不建議使用父對象中的欄位。

      **用大括弧括住欄位名稱**

      * 如果要讓計算參照內建欄位，欄位名稱必須由大括弧包住。

         例如： `{actualRevenue}`

         欄位名稱區分大小寫，且必須以在計算中確切顯示的方式顯示在Workfront系統中。

         導覽至 [Workfront API Explorer](https://developer.adobe.com/workfront/api-explorer/) 以標識可用於計算的欄位名稱。

      * 如果要讓計算參照自訂欄位，欄位名稱必須由大括弧包住，前面必須有 `DE:` 括弧內。

         例如： `{DE:Profit}`

         系統會列出您在輸入 `DE:`.

         * 如果您希望計算參考將從 *上層* 將自定義表單附加到對象時，必須在欄位名稱前面加上父對象的對象類型，也要以大括弧表示。

         例如，如果將自定義表單配置為處理任務，並且您希望欄位在表單附加到任務時計算父對象的實際收入，則您需要指明 `Project` 作為欄位的物件類型：

         `{project}.{actualRevenue}`

         或者，如果是自訂欄位：

         `{project}.{DE:profit}`

         **使用句點分隔項目**

         在計算的自定義欄位中引用相關對象時，必須將對象名稱和屬性與句點分開。

         例如，在任務類型自定義表單中，要在計算的自定義欄位中顯示Portfolio所有者的名稱，可鍵入以下內容：

         `{project}.{porfolio}.{owner}`

         這會決定下列項目：從自定義表單（任務）的對象，可以訪問與任務（項目）相關的下一個對象。 從那裡，您可以訪問項目（產品組合）的下一個相關對象，然後參考為產品組合對象（所有者）定義的欄位

         **參考自訂欄位的名稱語法**

         當您在計算的自訂欄位中參考其他自訂欄位時，需要輸入欄位名稱，如Workfront使用者介面中所顯示。

         例如，要在標有「執行贊助商」的自定義欄位中參考所選選項，可鍵入以下內容：

         `{DE:Executive sponsor}`

         >[!NOTE]
         >
         >typeahead欄位的語法與其他類型欄位的語法稍有不同，因為您需要新增 `:name` 最後。
         >
         >例如，要參考名為「執行贊助商」的自定義類型欄位中的選定選項，可鍵入：
         >
         >`{DE:Executive sponsor:name}`


         **多物件自訂表單中的計算自訂欄位**

         在多對象自定義表單中，所選對象類型至少必須與表單的計算自定義欄位中引用的一個欄位相容。 無法與物件相容的欄位在表單上會顯示「不適用」。

         為確保計算欄位為所有對象類型顯示正確結果，必須使用 `$$OBJCODE` 來定義每個對象類型的計算。

         >[!INFO]
         >
         >**範例:**
         >
         >在配置為處理項目、任務和問題的自定義表單中，可以使用以下公式來顯示對象類型：
         >
         >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
         >
         >在專案中，欄位將顯示「這是專案」、任務會顯示「這是任務」，而在問題中，欄位會顯示「這是問題」。


         >[!INFO]
         >
         >**範例：** 儘管沒有指派給：項目中的「名稱」欄位有內置的「所有者」欄位（該欄位會自動填入建立項目的人員的名稱，除非有人手動更改此名稱）。
         >
         >因此，在自定義的「負責」欄位中，您可以使用 `$$OBJCODE` 如下所示，在將自定義表單附加到項目時參考「所有者」欄位，並指派給：表單附加至任務時的「名稱」欄位：
         >
         >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

         如需變數的詳細資訊，例如 `$$OBJCODE,` 請參閱 [萬用字元篩選變數](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

         **自動更新計算的自訂欄位**

         發生下列情況時，對象上計算的自定義欄位會自動重新計算：

         * 物件上的某些項目會變更，例如每日時間軸計算。
         * 某人編輯另一個由對象上計算的自定義欄位引用的欄位。
         * 計算表達式為空，且欄位包含一個值 — 這會將值設為null。

            >[!NOTE]
            >
            ><div>在附加至物件的自訂表單中，計算自訂欄位中的日期和時間陳述式是由協調通用時間(UTC)計算並儲存，而非由組織例項和使用者設定檔所設定的時區設定。 根據每個使用者的個別時區，以自訂表單產生計算。</div>

+++
   1. 在大型文字方塊中按一下，然後按一下 **運算式** 和 **欄位** 可將其新增至您的計算。

      您也可以開始在大型文字方塊中輸入運算式或欄位，然後在顯示時加以選取。 每個項目在欄位中顯示「F」，在運算式中顯示「E」。

      如果鍵入左括弧，則會自動添加右括弧。

+++ **展開以查看實用提示**
      >[!TIP]
      >
      >您可以執行下列任一操作來取得計算方面的協助：
      > 
      >* 將滑鼠指標暫留在計算中的運算式上，可查看說明、可如何使用的範例，以及可在文章中取得詳細資訊的「了解詳情」連結 [計算資料運算式](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
         >  ![](assets/hover-expression-help-text.jpg)
      >* 使用顏色編碼識別您新增的元件。 運算式會以藍色顯示，欄位則以綠色顯示。
         >  ![](assets/colors-fields-expressions.jpg)
      >* 查找計算錯誤，隨時以粉紅色突出顯示。 您可以將滑鼠移至醒目提示的錯誤上，以顯示其原因的簡短說明。
         >  ![](assets/error-help.png)
      >* 在計算下方的區域中，在現有的Workfront物件上預覽結果。
         ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->

         >  ![](assets/preview-calc.jpg)
      >* 使用左側顯示的行號在長計算中引用表達式。


+++
   1. 按一下 **最小化** 完成為計算的自定義欄位建立計算時。

   1. （選用）使用下列任一選項進一步設定您計算的自訂欄位：

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新增邏輯</td> 
      <td>您可以新增「顯示邏輯」 ，以根據使用者在填寫表單時在先前的多選取欄位（下拉式清單、核取方塊或選項按鈕）中進行的至少一個選取，判斷計算的欄位是否顯示。 <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>只有在表單上計算的自訂欄位前面至少有一個核取方塊、選項按鈕或下拉式欄位時，才能使用此功能。 </p> <p>「跳過邏輯」對計算的自定義欄位不可用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新先前的計算</td> 
      <td>編輯現有的計算自定義欄位時，可以選擇此選項以在保存自定義表單時觸發計算中的更新。 只有在您儲存自訂表單時，才會發生此情況。 在執行此操作後，選項會恢復為其停用狀態。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在指示中顯示公式</td> 
      <td>如果您希望填寫自訂表單的使用者將游標移至欄位上時，查看欄位的公式，請保留此選項為啟用。 如需詳細資訊，請參閱 <a href="#instructions" class="MCXref xref">說明</a> 表格的前面。</td> 
     </tr> 
    </tbody> 
   </table>

1. 若要儲存變更，請按一下 **套用** 並移至其他區段，繼續建立您的表單。

   或

   按一下 **儲存並關閉**.


