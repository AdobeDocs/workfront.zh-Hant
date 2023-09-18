---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用舊版表單產生器新增自訂欄位至自訂表單
description: 處理自訂表單時，您可以建立新的自訂欄位並將其新增到自訂表單。 您也可以新增已新增至其他自訂表單的自訂欄位。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: 9b4faccb6b4d61970abb69af60a0e8d47c9408e7
workflow-type: tm+mt
source-wordcount: '2305'
ht-degree: 2%

---

# 使用舊版表單產生器新增自訂欄位至自訂表單

處理自訂表單時，您可以建立新的自訂欄位並將其新增到自訂表單。

您也可以新增已新增至其他自訂表單的自訂欄位。 如需指示，請參閱 [在自訂表單中重複使用自訂欄位或Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

如需將資產Widget新增至自訂表單的相關資訊（類似於新增自訂欄位的程式），請參閱 [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>在包含許多自訂欄位或在自訂欄位中有許多多選選項的自訂表單中，使用者在這些欄位中新增或變更值時可能會遇到效能變慢的情況。 例如，包含100個自訂欄位的表單，或包含超過200個選項的多選自訂欄位，在使用者與其互動時可能會較慢。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>管理自訂表單的存取權</p> <p>如需Workfront管理員如何授予此存取許可權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取層級設定，請聯絡Workfront管理員。

## 新增自訂欄位至自訂表單

1. 開始建立或編輯自訂表單，如所述 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 開啟 **新增欄位** 標籤。

   ![](assets/add-a-field.jpg)

1. 替換為 **新欄位** ![](assets/new-field.jpg) 選取，選取下列其中一個欄位型別：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">單行文字欄位</td> 
      <td>允許使用者在欄位中輸入單行文字。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">段落文字欄位</td> 
      <td>允許使用者在欄位中輸入多行文字。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">含格式的文字欄位</td> 
      <td>允許使用者在欄位中輸入多行文字，並以粗體、斜體、底線、專案符號、編號、超連結和區塊引號來格式化文字。 這可在首頁、更新區域、清單和Workfront物件的詳細資訊區域中取得。 15,000的字元限制可提供大量的文字和格式。</p> <p>如需有關透過API存取此欄位的資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">API中的RTF文字欄位儲存</a>.</p> <p><b>注意</b>：含有格式的文字欄位不適用於Workfront行動應用程式（將於未來發行版本中提供）。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">下拉</td> 
      <td>提供下拉式選項清單。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自動提示 </td> 
      <td>允許使用者輸入Workfront中存在的物件名稱。 當使用者開始輸入時，建議清單隨即出現。
      此欄位型別支援下列物件：
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
      <td>可讓您定義運算式並在自訂表單上顯示結果。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">新增計算資料至自訂表單</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">日期</td> 
      <td>顯示一個行事曆，使用者可以在其中選取日期和時間。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">核取方塊</td> 
      <td>可讓使用者選取多個選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">單選按鈕</td> 
      <td>要求使用者僅選取一個選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述文字</td> 
      <td>可讓您加入指示，並連結至Workfront以外的頁面。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">分節符號</td> 
      <td>分割槽符號實際上並非欄位。 您可以使用分割槽符號來組織自訂欄位和Widget到分割槽中，並在必要時為每個分割槽設定不同的檢視和編輯許可權。 有關新增和設定分割槽符號的資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">新增分割槽符號至自訂表單</a>.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >允許進行多項選擇的欄位（例如核取方塊和下拉式清單）很難在報告中建立圖表和群組。 若要更輕鬆地在報表中進行圖表和分組，您可以為每個選擇建立個別欄位（例如，單行文字欄位）。

1. 在 **欄位設定** 索引標籤中，設定您新增之自訂欄位型別的可用選項：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入描述性標籤，以在自訂欄位上方顯示。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td> <p>（必要）此名稱是當您新增自訂欄位至Workfront的各個區域時（例如報表、首頁和API互動），系統識別該欄位的方法。</p> <p>當您第一次設定自訂欄位並輸入標籤時，會自動填入「名稱」欄位以符合它。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p> 
      <p><b>重要</b>：   
      <ul> 
      <li>雖然可以這樣做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果這樣做，系統將不再識別現在可能在Workfront其他區域參考該欄位的自訂欄位。 <p>例如，如果您新增自訂欄位至報表，之後又變更其名稱，Workfront將無法辨識報表中的自訂欄位，且除非您使用新名稱將其重新新增至報表，否則將無法正常運作。</p> </li>
      <li> <p>建議您不要輸入已用於內建Workfront欄位的名稱。</p> </li>
      <li><p>建議您不要在自訂欄位名稱中使用句號/點字元，以防止在Workfront的不同區域使用欄位時發生錯誤。</p></li>
      </ul> <p>每個自訂欄位名稱在貴組織的Workfront例項中必須是唯一的。 如此一來，您便可重複使用已針對其他自訂表單建立的表單。 如需詳細資訊，請參閱 <a href="#Add" class="MCXref xref">新增自訂欄位至自訂表單</a> 本文章內容。</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入自訂欄位的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td> 
      <td> <p>選取將在自訂欄位中擷取的資料型別。 您可以在儲存表單後變更格式選擇，但新格式必須支援輸入的值。</p>

   <p><strong>範例：</strong> 如果您將某個欄位的數值儲存為至少一個物件上文字格式的欄位，稍後又將格式變更為數字或貨幣，則不會發生錯誤。 </p>
      <p>不過，如果您將英數字元值儲存在欄位中，且此欄位具有至少一個物件的「文字」格式，然後嘗試將格式變更為「數字」或「貨幣」，您將會遇到錯誤，因為儲存的英數字元值與「數字」或「貨幣」格式不相容。 </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">顯示類型</td> 
      <td>（僅限下拉式清單、核取方塊和選項按鈕）切換您要用於欄位的選項選取型別。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（僅限文字欄位）選取欄位寬度。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">顯示當日時間</td> 
      <td>（僅限日期欄位）如果您想要在欄位中顯示一天中的時間和日期，請選取此選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">參考物件類型</td> 
      <td> <p>（僅限預先輸入欄位）選取您要與欄位關聯的物件型別。</p> <p>按一下「套用」或「儲存+關閉」後，就無法變更欄位的物件型別。</p> <p><b>附註</b>:   
        <ul> 
         <li>如果您的Workfront管理員在Workfront使用者介面中為「Portfolio」、「程式」或「專案」自訂名稱，此下拉式清單中會顯示物件的預設Workfront名稱，而非自訂名稱。 如果您需要這方面的協助，請洽詢Workfront管理員。<br></li> 
         <li>iOS和Android Workfront Mobile應用程式支援下列物件型別：使用者、公司、群組、工作角色、Portfolio、方案、專案和範本。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">新增篩選器</td> 
      <td> <p>（僅限預先輸入欄位）為物件型別新增篩選條件，以限制使用者在使用欄位時可以選擇的物件。 </p> <p>例如，您可以限制欄位，以便只有在使用者符合以下條件時才可選取使用者名稱：</p> 
       <ul> 
        <li>它們屬於您指定的群組</li> 
        <li>它們與您指定的角色或職稱相關聯</li> 
        <li>他們與使用欄位的人屬於同一群組</li> 
       </ul> <p>您必須使用「文字模式」語法來定義所選物件型別的濾鏡。 如需使用「文字模式」建立篩選的詳細資訊，請參閱區段 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">在篩選器中編輯文字模式</a> 在文章中 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">文字模式概觀</a>. </p> <p><b>附註</b>:   
        <ul> 
         <li>如果您正在編輯現有的自訂表單，將篩選條件新增至預先輸入欄位時，不會移除使用者已使用該欄位新增的任何物件（在篩選條件範圍之外）。</li> 
         <li>此篩選器不適用於行動裝置。 如果您針對「預先輸入」欄位使用篩選器，則該欄位將會顯示在不受篩選器影響之使用者的行動裝置上。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述文字</td> 
      <td>（僅限描述性文字欄位）輸入您要顯示的文字，以提供自訂表單上的指示或連結。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">超連結</td> 
      <td>（僅限描述性文字欄位）如果要將超連結套用至已輸入的描述性文字，請在此處新增。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">建立必要欄位</td> 
      <td>如果您希望欄位是使用者完成自訂表單的必要欄位，請選取此選項。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">追蹤更新摘要中的欄位變更</td> 
      <td><p>按一下下拉式清單，然後選取您要自動追蹤欄位值變更的物件型別。</p> 
      <p><b>注意</b>：此選項不適用於下列專案：</p> 
      <ul> 
      <li>與下列物件型別相關聯的自訂表單：費用、公司、反複專案、記帳記錄和群組。</li> 
      <li>下列欄位型別：計算、描述性文字和分割槽符號</li> 
      </ul>
      <p><b>重要</b>：在這裡選取或取消選取物件型別會影響與所選物件型別關聯且包含此欄位的所有自訂表單。 例如，如果您在此取消選取物件型別並儲存自訂表單，則不再追蹤包含該欄位之任何自訂表單中該物件型別的欄位值變更。</p>
       <p>在這裡為欄位選擇物件型別並儲存自訂表單後，該欄位會顯示在「設定」中「更新摘要」區域的「自訂欄位」索引標籤上。</p> 
       <p>反之，若在「設定」的「更新摘要」區域中刪除此欄位，則會在與物件型別關聯且包含此欄位的所有自訂表單上，取消選取此設定的物件型別。</p> 
       <p>如需詳細資訊，請參閱區段 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">新增您希望Workfront追蹤的欄位</a> 在文章中 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">設定系統更新</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">新增邏輯</td> 
      <td>根據使用者在現有欄位中所做的選擇，指定哪些欄位應該顯示在表單上。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">新增顯示邏輯和略過邏輯至自訂表單</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">選擇 </td> 
      <td> <p>（僅限下拉式清單、核取方塊或選項按鈕；選擇性）</p> 
       <ol> 
        <li> <p>按一下 <b>選項</b>，然後啟用下列任一專案：</p> 
           <ul> 
            <li><strong>顯示值</strong>：顯示欄位中每個選擇的值。 依預設，會顯示每個選擇的標籤。</li> 
            <li><strong>將選擇按A-Z排序</strong>：依字母順序排序您在欄位中新增的選擇。</li> 
           </ul> 
        </li> 
        <li> <p>針對您為使用者新增的每個選擇，按一下齒輪圖示 <img src="assets/gear-icon-settings.png">，然後選取下列其中一個選項：</p> 
           <ul> 
            <li><strong>預設選取</strong>：在欄位中選取預設選項。</li> 
            <li> <p><strong>隱藏選擇</strong>：隱藏欄位中的選擇。 隱藏的選擇在報表中仍可存取。</p> </li> 
            <li> <p><strong>移除選擇</strong>：從欄位中移除選擇。</p> <p><b>警告</b>：如果您有使用此選項的目前物件，請勿將其從欄位中移除。 移除它將會導致歷史資料遺失。 相反地，選取要隱藏它的選項，這會防止使用者在將來選取它。</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. （視條件而定）若要變更自訂表單上欄位的顯示型別，請按一下 **顯示型別** 下拉式功能表，然後按一下您想要的型別。

   您可以在下列欄位顯示型別之間切換：

   * **選擇型別欄位**：核取方塊、下拉式清單、選項按鈕。
   * **文字型別欄位**：單行文字欄位、段落文字欄位。 (您無法將「格式化文字欄位」切換為不同的顯示型別。 不過，您可以將其移除並新增其他型別的欄位。)

   例如，如果您已建立「核取方塊」欄位，則可將其變更為「下拉式清單」欄位或「選項按鈕」欄位。 或者，如果您已建立「單行文字欄位」，您可以將其變更為「段落文字欄位」。

   >[!NOTE]
   >
   >當您想要將欄位的顯示型別從核取方塊欄位或多選下拉式欄位（允許選擇多個選項的下拉式清單）變更為單選欄位型別時，請考慮以下事項：
   >
   >* 如果您變更為選項按鈕，Workfront會保留使用者在欄位中可能輸入的任何多選值，直到使用者變更並儲存表單任何部分的資料為止。 此時，使用「多重選取型別」欄位選取的任何值都會被選取的「選項按鈕」值取代。
   >* 如果您變更為單選下拉式清單，Workfront會保留使用者在欄位中可能輸入的任何多選值，直到使用者變更並儲存欄位中的值為止。 此時，使用「多重選取型別」欄位選取的任何值都會被選取的「下拉式清單」值取代。

1. （選用）重複步驟2至6以新增其他自訂欄位。

   或

   新增已為貴組織建立的欄位，如中所述 [在自訂表單中重複使用自訂欄位或Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >您最多可以在單一自訂表單中新增500個欄位和Widget。 不過，根據表單的複雜性，當表單上存在超過100個時，可能會發生效能降低。 複雜表單的範例包括含有階層式引數的表單、計算的自訂資料欄位，以及單一欄位中的多個值選項。

1. 按一下 **套用**.
1. 如果您想以其他方式繼續建置自訂表單，請繼續閱讀下列其中一篇文章：

   * [在自訂表單中定位自訂欄位和Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [新增計算資料至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [新增分割槽符號至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [新增顯示邏輯和略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [預覽並完成自訂表格](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
