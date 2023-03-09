---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用舊版表單產生器將自訂欄位新增至自訂表單
description: 使用自訂表單時，您可以建立新的自訂欄位，並將其新增至自訂表單。 您也可以新增已新增至其他自訂表單的自訂欄位。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '2208'
ht-degree: 2%

---

# 使用舊版表單產生器將自訂欄位新增至自訂表單

使用自訂表單時，您可以建立新的自訂欄位，並將其新增至自訂表單。

您也可以新增已新增至其他自訂表單的自訂欄位。 如需指示，請參閱 [在自訂表單中重複使用自訂欄位或介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

如需將資產介面工具集新增至自訂表單（這是類似新增自訂欄位的程式）的資訊，請參閱 [在自訂表單中新增或編輯資產介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>在包含許多自訂欄位或自訂欄位中許多多選選項的自訂表單中，使用者在這些欄位中新增或變更值時，可能會遇到效能變慢的問題。 例如，包含100個自訂欄位的表單，或包含200個以上選項的多選自訂欄位，當使用者與其互動時可能會變慢。

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
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 新增自訂欄位至自訂表單

1. 開始建立或編輯自訂表單，如 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 開啟 **新增欄位** 標籤。

   ![](assets/add-a-field.jpg)

1. 使用 **新欄位** ![](assets/new-field.jpg) 選取，選取下列其中一個欄位類型：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">單行文字欄位</td> 
      <td>可讓使用者在欄位中輸入單行文字。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">段落文字欄位</td> 
      <td>可讓使用者在欄位中輸入多行文字。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">含格式的文字欄位</td> 
      <td>允許用戶在欄位中鍵入多行文本，並使用粗體、斜體、下划線、項目符號、編號、超連結和塊引號來格式化文本。 可在首頁、更新區域、清單和Workfront物件的詳細資訊區域中使用。 字元限制為15,000，可容納大量文字和格式。</p> <p>如需透過API存取此欄位的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">API中的RTF欄位儲存</a>.</p> <p><b>注意</b>:Workfront行動應用程式無法使用格式化的文字欄位（未來版本提供）。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">下拉</td> 
      <td>提供下拉式選項清單。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自動提示 </td> 
      <td>可讓使用者輸入Workfront中存在之物件的名稱。 當使用者開始輸入時，會顯示建議清單。
      此欄位類型支援下列物件：
      <ul><li>使用者</li>
      <li>群組</li>
      <li>職務角色</li>
      <li>專案組合</li>
      <li>方案</li>
      <li>專案</li>
      <li>團隊</li>
      <li>範本</li>
      <li>公司</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已計算</td> 
      <td>可讓您定義運算式，並在自訂表單上顯示結果。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">將計算資料新增至自訂表單</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">日期</td> 
      <td>顯示日曆，使用者可在其中選取日期和時間。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">核取方塊</td> 
      <td>允許用戶選擇多個選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">單選按鈕</td> 
      <td>僅要求使用者選取一個選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述文字</td> 
      <td>可讓您加入指示並連結至Workfront以外的頁面。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">分節符號</td> 
      <td>區段插播實際上不是欄位。 您可以使用分區符號將自訂欄位和小工具組織到分區，並視需要為每個區段設定不同的檢視和編輯權限。 有關添加和配置節斷點的資訊，請參見 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">為自訂表單新增區段分頁</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **欄位設定** 標籤中，設定您要新增的自訂欄位類型可用的選項：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要在自訂欄位上方顯示的描述性標籤。 您隨時都可以變更標籤。</p> <p><b>重要</b>:請避免在此標籤中使用特殊字元。 報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td> <p>（必要）此名稱是當您將自訂欄位新增至Workfront中的各種區域時，系統識別自訂欄位的方式，例如報表、首頁和API互動。</p> <p>當您第一次設定自訂欄位並輸入標籤時，「名稱」欄位會自動填入以符合。 但「標籤」和「名稱」欄位未同步，因此您可以自由地更改用戶看到的標籤，而不必更改系統看到的名稱。</p> 
      <p><b>重要</b>:   
      <ul> 
      <li>雖然可以這麼做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果您這麼做，系統將不再識別自訂欄位，現在可能會在Workfront的其他區域參照該欄位。 <p>例如，如果您將自訂欄位新增至報表，之後又變更其名稱，Workfront在報表中將無法辨識該欄位，除非您使用新名稱將其重新新增至報表，否則該欄位將停止正常運作。</p> </li>
      <li> <p>建議您不要輸入已用於內建Workfront欄位的名稱。</p> </li>
      <li><p>建議您不要在自訂欄位名稱中使用句點/點字元，以防止在Workfront不同區域使用欄位時發生錯誤。</p></li>
      </ul> <p>每個自訂欄位名稱在貴組織的Workfront例項中必須是唯一的。 這樣，您就可以重複使用已針對其他自訂表單建立的表單。 如需詳細資訊，請參閱 <a href="#Add" class="MCXref xref">新增自訂欄位至自訂表單</a> 這篇文章。</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關自訂欄位的任何其他資訊。 當使用者填寫自訂表單時，可將滑鼠移至問號圖示上方，檢視包含您在此輸入之資訊的工具提示。</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td> 
      <td> <p>選取要在自訂欄位中擷取的資料類型。</p> <p><b>附註</b>:   
        <ul> 
         <li>表單儲存後無法編輯此欄位。 如果要在數學計算中使用欄位，請確保選擇數字或貨幣格式。<br></li> 
         <li>選擇「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">顯示類型</td> 
      <td>（僅限下拉式清單、核取方塊和選項按鈕）切換您要用於欄位的選項選取類型。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（僅限文字欄位）選取欄位的寬度。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">顯示當日時間</td> 
      <td>（僅限日期欄位）如果您想在欄位中顯示一天中的時間以及日期，請選取此選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">參考物件類型</td> 
      <td> <p>（僅限Typeaead欄位）選擇要與欄位關聯的對象類型。</p> <p>按一下「應用」或「保存並關閉」後，就無法更改欄位的對象類型。</p> <p><b>附註</b>:   
        <ul> 
         <li>如果您的Workfront管理員在Workfront使用者介面中自訂了Portfolio、方案或專案的名稱，物件的預設Workfront名稱會顯示在此下拉式清單中，而非自訂名稱。 如需相關協助，請洽詢Workfront管理員。<br></li> 
         <li>iOS和Android Workfront行動應用程式支援下列物件類型：用戶、公司、組、職務、Portfolio、方案、項目和模板。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">新增篩選器</td> 
      <td> <p>（僅限Typeaead欄位）為對象類型添加篩選器，以限制用戶在使用該欄位時可以選擇的對象。 </p> <p>例如，您可以限制欄位，以便只有在使用者名稱符合下列條件時，才能選取使用者名稱：</p> 
       <ul> 
        <li>它們屬於您指定的群組</li> 
        <li>它們與您指定的角色或職務相關聯</li> 
        <li>它們與使用欄位的人員屬於相同群組</li> 
       </ul> <p>必須使用文本模式語法為所選對象類型定義篩選器。 如需使用文字模式建立篩選器的相關資訊，請參閱區段 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">在篩選器中編輯文字模式</a> 在文章中 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">文字模式概觀</a>. </p> <p><b>附註</b>:   
        <ul> 
         <li>如果您正在編輯現有的自訂表單，將篩選器新增至Typeahead欄位不會移除使用者已使用欄位新增的任何物件（位於篩選器範圍之外）。</li> 
         <li>行動裝置上無法使用此篩選器。 如果您對Typeahead欄位使用篩選，該欄位將出現在不受篩選影響的使用者行動裝置上。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述文字</td> 
      <td>（僅限描述性文字欄位）輸入要顯示的文字，以提供自訂表單的指示或連結。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">超連結</td> 
      <td>（僅限描述性文字欄位）如果要將超連結套用至您輸入的描述性文字，請在此處新增。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">建立必填欄位</td> 
      <td>如果您希望欄位為必要欄位，讓使用者完成自訂表單，請選取此選項。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">追蹤更新摘要中的欄位變更</td> 
      <td><p>按一下下拉式清單，然後選取您要自動追蹤欄位值變更的物件類型。</p> 
      <p><b>注意</b>:此選項不適用於下列項目：</p> 
      <ul> 
      <li>與以下對象類型關聯的自定義表單：費用、公司、小版本、開單記錄和組。</li> 
      <li>下列欄位類型：計算、描述性文字和區段插播</li> 
      </ul>
      <p><b>重要</b>:在此處選擇或取消選擇對象類型會影響與所選對象類型關聯並包含此欄位的所有自定義表單。 例如，如果您在此處取消選取物件類型並儲存自訂表單，則包含該欄位的任何自訂表單中，將不再追蹤該物件類型欄位的值變更。</p>
       <p>在此為欄位選取物件類型並儲存自訂表單後，欄位會顯示在「設定」中「更新摘要」區域的「自訂欄位」標籤上。</p> 
       <p>反之，如果此欄位在「設定」的「更新摘要」區域中刪除，則在與物件類型關聯且包含此欄位的所有自訂表單上，會取消選取此設定的物件類型。</p> 
       <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">新增您要Workfront追蹤的欄位</a> 在文章中 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">配置系統更新</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">新增邏輯</td> 
      <td>根據使用者在現有欄位中所做的選取，指定表單上應顯示哪些欄位。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">新增顯示邏輯並略過邏輯至自訂表單</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">選擇 </td> 
      <td> <p>(僅限下拉式清單、核取方塊或選項按鈕；可選)</p> 
       <ol> 
        <li> <p>按一下 <b>選項</b>，然後啟用下列任一項：</p> 
           <ul> 
            <li><strong>顯示值</strong>:顯示欄位中每個選項的值。 依預設會顯示每個選項的標籤。</li> 
            <li><strong>排序選擇A-Z</strong>:按字母順序對欄位中添加的選項進行排序。</li> 
           </ul> 
        </li> 
        <li> <p>針對您為使用者新增的每個選項，按一下齒輪圖示 <img src="assets/gear-icon-settings.png">，然後選取下列其中一個選項：</p> 
           <ul> 
            <li><strong>預設選擇</strong>:依預設，在欄位中選取選項。</li> 
            <li> <p><strong>隱藏選項</strong>:隱藏欄位中的選項。 隱藏的選項仍可在報表中存取。</p> </li> 
            <li> <p><strong>刪除選項</strong>:從欄位中移除選項。</p> <p><b>警告</b>:如果您有使用此選項的當前對象，請勿將其從欄位中刪除。 移除會導致歷史資料遺失。 而是選取要隱藏的選項，這會讓使用者無法在日後選取。</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. （條件性）若要變更自訂表單上欄位的顯示類型，請按一下 **顯示類型** 下拉式功能表，然後按一下您想要的類型。

   您可以在下列欄位顯示類型之間切換：

   * **選擇類型欄位**:核取方塊、下拉式清單、選項按鈕。
   * **文字類型欄位**:單行文本欄位，段落文本欄位。 (無法將具有格式的文本欄位切換到不同的顯示類型。 不過，您可以移除它，然後新增其他類型的欄位。)

   例如，如果您已建立核取方塊欄位，則可將其變更為下拉式清單欄位或選項按鈕欄位。 或者，如果已建立了單行文本欄位，則可將其更改為段落文本欄位。

   >[!NOTE]
   >
   >如果要將欄位的顯示類型從核取方塊欄位或多選下拉式欄位（允許選取多個選項的下拉式清單）變更為單選欄位類型，請考量下列事項：
   >
   >* 如果您變更為選項按鈕，Workfront會保留使用者可能在欄位中輸入的任何多選值，直到使用者變更並儲存表單的任何部分資料為止。 此時，使用多選類型欄位選取的任何值，都會由選取的選項按鈕值取代。
   >* 如果您變更為單選下拉式清單，Workfront會保留使用者可能在欄位中輸入的任何多選值，直到使用者變更並將值儲存在欄位中為止。 此時，使用多選類型欄位選取的任何值，都會由選取的下拉式清單值取代。


1. （可選）重複步驟2至6以新增其他自訂欄位。

   或

   新增已為貴組織建立的欄位，如 [在自訂表單中重複使用自訂欄位或介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >在單一自訂表單中，最多可新增500個欄位和Widget。 但是，當表單上存在超過100個時，效能可能會降低，具體取決於表單的複雜性。 複雜表單的範例包括具有階層式參數的表單、計算的自訂資料欄位，以及單一欄位中的多個值選項。

1. 按一下 **套用**.
1. 如果您想以其他方式繼續建立自訂表單，請繼續閱讀下列其中一篇文章：

   * [在自訂表單中放置自訂欄位和小工具](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [在自訂表單中新增或編輯資產介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [為自訂表單新增區段分頁](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [新增顯示邏輯並略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [預覽並完成自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
