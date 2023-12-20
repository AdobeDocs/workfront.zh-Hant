---
product-area: reporting
navigation-topic: text-mode-reporting
title: 編輯群組中的文字模式
description: '注意：讓所有FVG文章在文字模式下編輯時都相同)'
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# 編輯群組中的文字模式

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

您可以使用文字模式編輯清單或報表中的分組，以存取標準介面中無法使用的欄位，並建立更複雜的分組。

>[!TIP]
>
>建議您在標準模式中建立儘可能多的群組，然後將其轉換為文字模式以進行編輯。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯對報告、儀表板、行事曆的存取權以編輯報告中的群組</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報告的許可權，以編輯報告中的分組</p> <p>管理群組的許可權以編輯它</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 先決條件

在報表或清單中開始使用文字模式之前，請務必熟悉Workfront文字模式語法。

如需詳細資訊，請參閱：

* [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自訂檢視、篩選和分組範例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 編輯群組中的文字模式

使用文字模式編輯群組的方式，在報告和清單上是相同的。 從報表或清單存取分組時不同。

>[!NOTE]
>
>分組是在報表中建立圖表的必要報表元素。 圖表不支援文字模式分組。 如需有關將圖表新增至報表的資訊，請參閱 [新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

如需建立群組的詳細資訊，請參閱 [在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 執行下列其中一項：

   1. 若要從報表存取分組，請移至報表，然後按一下 **報表動作** > **編輯** > **群組** 標籤。
   1. 若要從清單存取分組，請移至清單，並從 **分組** 下拉式功能表，將滑鼠移至您要修改的分組上，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png).

      群組產生器隨即開啟。

1. 按一下 **新增群組** 以新增群組，然後按一下 **切換到文字模式** 建立器的右上角。

   >[!TIP]
   >
   您可以在標準介面中新增最多3個群組。 您只能使用文字模式新增第4個群組，而在Workfront中不能有超過4個群組層級。

1. 開始輸入您要作為群組依據的欄位名稱。

   當您在清單中看到欄位時，請選取該欄位的名稱。

1. 按一下 **切換到文字模式** 建立器的右上角。

   然後，分組會以文字模式顯示。

   當您以文字模式編輯群組時，Workfront會新增

   ```
   textmode=true
   ```

   分組的程式碼行。 這表示群組在文字模式中被修改。

   **範例：** 若要依專案名稱再依主要受指派人的名稱將任務清單分組，您的分組在文字模式中應如下所示。

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   粗體行是必填欄位。

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   分組中的每個欄位都有參照該欄位的數行程式碼。

   下表概述文字模式群組中的關鍵行。

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   文字模式群組中的關鍵行與建立文字模式檢視所需的行類似。

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>範例行</strong> </th> 
      <th><strong>說明</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>群組。&lt;number&gt;.</strong> </td> 
      <td> <p>每一行程式碼的前面都會加上此文字。 參考分組中所選相同欄位的程式碼行會以相同編號編號，如下所示：</p> 
       <ul> 
        <li>報表的第一個群組具有群組編號0。 所有參照第一個群組的行都以開頭 <code>group.0</code>.</li> 
        <li>報表的第二個群組具有群組編號1。 所有參考第二個群組的行都以開頭 <em><code>group.1</code></em>.</li> 
        <li>報表的第三個分組的群組編號為2。 所有參考第三個群組的行都以開頭 <em><code>group.2</code></em>.</li> 
        <li>只有在文字模式中，您才能為第四個群組新增群組編號3。 所有參考第四個群組的行都以開頭 <em><code>group.3</code></em>.</li> 
       </ul> <p>注意：產生器不支援4個群組。 僅在使用文字模式時支援這些功能。 Workfront不支援超過4個層級的群組。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>這是物件或欄位在資料庫中顯示的名稱。 如需有關物件和欄位如何在資料庫中顯示的詳細資訊，請參閱 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API總管</a>.</p> <p>存在下列情況：</p> 
       <ol> 
        <li value="1"> <p> 如果您顯示的欄位名稱是短語而不是單一名詞，則必須使用駝峰式大小寫語法 <code>valuefield</code>. 例如，對於任務的計劃開始日期，程式碼為：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>如果您想要顯示自訂欄位，請 <code>valuefield</code> value是欄位的實際名稱，如您在介面中所見。 例如，對於名為「更多資訊」的自訂欄位，程式碼為：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>如果您要依與其他物件相關的物件來群組，請使用 <code>valuefield</code> 程式碼行物件名稱和屬性會以冒號分隔。</p> <p>例如，按Portfolio名稱對任務清單進行分組，值欄位行具有下列值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>這表示您可以從報表（工作）的物件存取下一個相關物件（專案）；從那裡，您可以從專案（專案組合）存取下列相關物件；然後存取專案組合名稱（名稱）。</p> </li> 
       </ol> <p>如需物件如何彼此連線的詳細資訊，請參閱區段 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">物件的相依性和階層</a> 在 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">瞭解Adobe Workfront中的物件</a>.</p> <p>備註：如果您在文字模式中選擇在標準介面中無效的欄位，並切換至標準介面，則會刪除分組。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>值格式=</strong> </td> 
      <td> <p>此線條代表用來顯示 <code>valuefield</code>. 此 <code>valueformat</code> 會識別物件或欄位是否顯示為文字、數字、百分比或日期。</p> <p>我們建議使用 <code>HTML</code> 針對您的 <code>valueformat</code>，尤其是使用 <code>valueexpression</code>，確保以最精確的方式顯示您的資訊。</p> <p>如需此行的其他值相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">在文字模式中使用條件式格式</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>您可以新增此行來取代 <code>valuefield</code>，如果您想使用數個欄位之間的計算來分組清單。</p> <p>您必須將 <code>valuefield</code> 括弧內的物件，每次在 <code>valueexpression</code>.</p> <p>存在下列情況：</p> 
       <ol> 
        <li value="1"> <p>如果要以大寫顯示群組的名稱，請使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>此 <code>valuefield</code> 在API Explorer中顯示的物件會拼寫。</p> </li> 
        <li value="2">如果您想要新增多個 <code>valuefields</code> 將它們串連在 <code>valueexpression </code>行，則必須以句點分隔。<p>例如，如果您想在任務清單中以大寫顯示投資組合的名稱，您將在以下程式碼的 <code>valueexpression</code> 行：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>如果您想在中使用自訂欄位 <code>valueexpression</code> 欄位名稱的前面必須加一行 <code>DE:</code> 以指示它是一個自訂欄位。 欄位名稱在介面中顯示時拼寫。</p><p>重要： <span>當您使用放置在自訂表單區段中的自訂欄位時，如果某些使用者的許可權受到限制，則計算 <code>valueexpression </code>當這些使用者在報告中檢視此計算時為空白。 如需有關調整自訂表格區段許可權的資訊，請參閱</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a></span>.</p><p>例如，如果您有一個標示為「開發人員名稱」的自訂欄位，並且您想要依此欄位分組並以大寫顯示，您可以使用以下專案 <code>valueexpression</code> 以表示此訊息：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>參照「預先輸入」型別自訂欄位時，請使用下列運算式來參照在標示為「開發人員名稱」的欄位中選取的物件名稱：</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>此行會定義群組標籤。 在此情況下，它會使用根據索引鍵的縮寫值。</p> <p>如果要修改群組名稱，可將此值變更為下列值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> 可讓您為群組名稱輸入任何文字，而 <code>namekey</code> 需要您輸入用來翻譯群組名稱的金鑰。</p> <p>若要變更群組名稱，您也可以新增 <code>displayname </code>行（如果不存在）。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>您可以新增下列行來變更欄的名稱，這會覆寫 <code>namekey/name</code> 值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>建議移除所有包含 <code>name </code>當您重新命名群組時。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）將下列其中一行程式碼新增至任何群組，以指出群組中的結果應顯示在展開或收合的清單中。 依預設，群組顯示為展開：


   ```
   group.0.iscollapsed=true
   ```

   如果您希望群組顯示且結果摺疊

   ```
   group.0.iscollapsed=false
   ```

   如果您希望群組顯示且結果展開

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   * 當您在檢視清單時手動調整群組，Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
   * 從圖表元素存取群組結果後，群組結果一律展開顯示。

1. 按一下 **完成** 如果要儲存變更並繼續編輯分組或報告。
1. 按一下 **儲存群組** 在清單或 **儲存+關閉** 以儲存報表。
