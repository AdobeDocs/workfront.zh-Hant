---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文字模式編輯群組
description: 您可以使用文字模式編輯清單或報表中的分組，以存取標準介面中無法使用的欄位，並建立更複雜的分組。
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 0%

---

# 使用文字模式編輯群組

<!-- Audited: 1/2025 -->

您可以使用文字模式編輯清單或報表中的分組，以存取標準介面中無法使用的欄位，並建立更複雜的分組。

>[!TIP]
>
>建議您在標準模式中建立儘可能多的群組，然後將其轉換為文字模式以進行編輯。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯對報告、儀表板、行事曆的存取權以編輯報告中的群組</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報告的許可權，以編輯報告中的分組</p> <p>管理群組的許可權以編輯它</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

在報表或清單中開始使用文字模式之前，請務必熟悉Workfront文字模式語法。

如需詳細資訊，請參閱：

* [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自訂檢視、篩選和分組範例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 使用文字模式編輯群組

使用文字模式編輯群組的方式，在報告和清單上是相同的。 從報表或清單存取分組時不同。

>[!NOTE]
>
>分組是在報表中建立圖表的必要報表元素。 圖表不支援文字模式分組。 如需有關將圖表新增至報表的資訊，請參閱[將圖表新增至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

如需建立群組的詳細資訊，請參閱[在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 執行下列其中一項：

   1. 若要從報告存取分組，請移至報告，然後按一下&#x200B;**報告動作** > **編輯** > **分組**&#x200B;索引標籤。
   1. 若要從清單存取群組，請移至清單，然後從&#x200B;**群組**&#x200B;下拉式功能表，將滑鼠移至您要修改的分組，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

      群組產生器隨即開啟。

1. 按一下&#x200B;**[新增群組]**&#x200B;以新增群組，按一下產生器右上角的&#x200B;**[切換到文字模式]**，然後按一下&#x200B;**[編輯文字模式]**。

   >[!TIP]
   >
   >您可以在標準介面中新增最多3個群組。 您只能使用文字模式新增第4個群組，而在Workfront中不能有超過4個群組層級。

1. 開始輸入您要作為群組依據的欄位名稱。

   當您在清單中看到欄位時，請選取該欄位的名稱。

1. 按一下產生器右上角的&#x200B;**切換至文字模式**。

   然後，分組會以文字模式顯示。

   當您以文字模式編輯群組時，Workfront會新增

   ```
   textmode=true
   ```

   分組的程式碼行。 這表示群組在文字模式中被修改。

   **範例：**&#x200B;若要依專案名稱然後依主要受指派人的名稱來群組任務清單，您的群組在文字模式中應如下所示。

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >粗體行是必填欄位。

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
   >文字模式群組中的關鍵行與建立文字模式檢視所需的行類似。

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
        <li>報表的第一個群組具有群組編號0。 所有參照第一個群組的行都以<code>group.0</code>開頭。</li> 
        <li>報表的第二個群組具有群組編號1。 所有參考第二個群組的行都以<em><code>group.1</code></em>開頭。</li> 
        <li>報表的第三個分組的群組編號為2。 所有參考第三個群組的行都以<em><code>group.2</code></em>開頭。</li> 
        <li>只有在文字模式中，您才能為第四個群組新增群組編號3。 所有參考第四個群組的行都以<em><code>group.3</code></em>開頭。</li> 
       </ul> <p>注意：產生器不支援4個群組。 僅在使用文字模式時支援這些功能。 Workfront不支援超過4個層級的群組。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>這是物件或欄位在資料庫中顯示的名稱。 如需有關物件和欄位如何在資料庫中顯示的詳細資訊，請參閱<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API總管</a>。</p> <p>存在下列情況：</p> 
       <ol> 
        <li value="1"> <p> 如果您顯示的欄位名稱是短語而非單一名詞，則必須使用<code>valuefield</code>的駝峰式大小寫語法。 例如，對於任務的計劃開始日期，程式碼為：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>如果您想要顯示自訂欄位，<code>valuefield</code>值是欄位的實際名稱，如您在介面中所見。 例如，對於名為「更多資訊」的自訂欄位，程式碼為：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>如果您想使用程式碼<code>valuefield</code>行將物件群組為與其他物件相關的物件，則物件名稱和屬性會以冒號分隔。</p> <p>例如，依「Portfolio名稱」對任務清單進行分組，其值欄位行如下：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>這表示您可以從報表（工作）的物件存取下一個相關物件（專案）；從那裡，您可以從專案（專案組合）存取下列相關物件；然後存取專案組合名稱（名稱）。</p> </li> 
       </ol> <p>如需物件如何彼此連結的詳細資訊，請參閱<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">瞭解Adobe Workfront中的物件</a>中的<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">物件相互相依性和階層</a>一節。</p> <p>備註：如果您在文字模式中選擇在標準介面中無效的欄位，並切換至標準介面，則會刪除分組。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>此線條代表用來顯示<code>valuefield</code>的格式。 <code>valueformat</code>會識別物件或欄位是否顯示為文字、數字、百分比或日期。</p> <p>我們建議對您的<code>valueformat</code>使用<code>HTML</code>，尤其是在使用<code>valueexpression</code>時，以確保最準確地顯示您的資訊。</p> <p>如需此行的其他值相關資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">在文字模式中使用條件式格式</a>。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>如果您要依數個欄位之間的計算來群組清單，可以新增此行來取代<code>valuefield</code>。</p> <p>每次在<code>valueexpression</code>中使用物件時，都必須用大括弧括住物件的<code>valuefield</code>。</p> <p>存在下列情況：</p> 
       <ol> 
        <li value="1"> <p>如果要以大寫顯示群組的名稱，請使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>物件的<code>valuefield</code>在API Explorer中的顯示方式是拼字的。</p> </li> 
        <li value="2">如果您想要將多個<code>valuefields</code>串連在<code>valueexpression </code>行中，以將其加入，則必須以句點分隔它們。<p>例如，如果您要在工作清單中以大寫顯示投資組合名稱，可在<code>valueexpression</code>行中使用下列程式碼：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>如果您要在<code>valueexpression</code>行中使用自訂欄位，則必須在欄位名稱前面加上<code>DE:</code>，以表示它是自訂欄位。 欄位名稱在介面中顯示時拼寫。</p><p>重要： <span>當您使用自訂欄位時，若該欄位放置在自訂表格區段中，而該區段對某些使用者具有限制的許可權，則當這些使用者在報表中檢視此計算時，<code>valueexpression </code>的計算為空白。 如需有關調整自訂表格區段許可權的資訊，請參閱</span> <span href="help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">建立自訂表格</a></span>。</p><p>例如，如果您有標示為「開發人員名稱」的自訂欄位，而且您想依此欄位分組並以大寫顯示，您可以使用下列<code>valueexpression</code>來表示這點：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>參照「預先輸入」型別自訂欄位時，請使用下列運算式來參照在標示為「開發人員名稱」的欄位中選取的物件名稱：</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>此行會定義群組標籤。 在此情況下，它會使用根據索引鍵的縮寫值。</p> <p>如果要修改群組名稱，可將此值變更為下列值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> 可讓您輸入群組名稱的任何文字，而<code>namekey</code>需要您輸入用來翻譯群組名稱的金鑰。</p> <p>若要變更群組名稱，您也可以新增<code>displayname </code>行（如果沒有）。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>您可以新增下列行來變更覆寫<code>namekey/name</code>值的資料行名稱：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>當您重新命名群組時，建議移除所有包含<code>name </code>的行。</p> </td> 
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
   >* 當您在檢視清單時手動調整群組，Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
   >* 從圖表元素存取群組結果後，群組結果一律展開顯示。

1. 如果要儲存變更並繼續編輯群組或報告，請按一下&#x200B;**完成**。
1. 按一下清單中的&#x200B;**儲存群組**&#x200B;或&#x200B;**儲存+關閉**&#x200B;以儲存您的報告。
