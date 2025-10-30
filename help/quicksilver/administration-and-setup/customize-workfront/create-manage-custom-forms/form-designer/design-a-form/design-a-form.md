---
title: 建立自訂表格
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表單設計工具來設計自訂表單。 您可以將自訂表單附加至不同的Workfront物件，以擷取這些物件的相關資料。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: f6e0329ec63038b33006325701007c564c4126cc
workflow-type: tm+mt
source-wordcount: '6933'
ht-degree: 5%

---

# 建立自訂表格

{{preview-fast-release-general}}

<!-- Audited: 6/2025 -->

您可以使用Adobe Workfront中的表單設計工具來設計自訂表單。 您可以將自訂表單附加至不同的Workfront物件，以擷取這些物件的相關資料。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr>  
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 開始設計自訂表單

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**自訂Forms**，然後選取&#x200B;**Forms**。

1. 按一下&#x200B;**新增自訂表格。**
1. 選取您要附加自訂表單的物件型別，然後按一下[繼續]。****

   ![選擇物件型別](assets/choose-object-type.jpg)

1. 在&#x200B;**新增表單名稱**&#x200B;區域中，輸入自訂表單標題。
1. （選擇性）如果您想要新增更多物件型別至表單，以便將其附加到更多物件，請按一下&#x200B;**物件型別**&#x200B;旁的![新增](assets/add-objects-icon.png)圖示&#x200B;**新增物件圖示**，然後在顯示的功能表中選取您想要的型別。 您可以重複此步驟，新增任意數目的物件型別。

   將多個物件新增至表單後，您可以按一下物件型別上的X以將其從表單中刪除。

   >[!CAUTION]
   >
   >刪除自訂表單也會刪除與表單關聯的物件上的所有自訂資料。 無法復原已刪除的資料。 或者，您可以停用不再使用的自訂表單，這會保留所有關聯的歷史資料。
   >
   >如需詳細資訊，請參閱[從現有的自訂表單新增或刪除物件型別](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md)和[停用或重新啟用自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md)。


1. 接下來，您可以開始將欄位新增至自訂表單。 如需詳細資訊，請參閱下列章節：
   * [重複使用已在其他自訂表單中使用的現有欄位或Widget](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [欄位名稱和標籤的附註](#notes-on-field-names-and-labels)
   * [新增文字欄位](#add-text-fields)
   * [新增計算欄位](#add-calculated-fields)
   * [新增選項按鈕、核取方塊群組和下拉式清單](#add-radio-buttons-checkbox-groups-and-drop-downs)
   * [新增預先輸入和日期欄位](#add-typeahead-and-date-fields)
   * [新增外部查詢欄位](#add-external-lookup-fields)
   * [新增影像、PDF和影片](#add-images-pdfs-and-videos)
   * [新增Workfront原生欄位](#add-workfront-native-fields)
   * [新增Adobe XD檔案](#add-adobe-xd-files)
   * [新增Planning連線欄位](#add-planning-connection-fields)

## 新增欄位或現有欄位至您的自訂表單

在設計自訂表單時，您可以使用新的或現有的欄位。

自訂表單限製為500個欄位。 左下方的計數器顯示表單上使用的欄位數，當您在表單設計工具中捲動時，它始終可見。

### 重複使用已在其他自訂表單中使用的現有欄位或Widget

1. 在熒幕的左上角，按一下&#x200B;**欄位程式庫**。

1. 將所需的欄位或Widget拖放至畫布上。 重複此步驟以新增任何其他欄位或Widget。

   >[!NOTE]
   >
   >您最多可以在單一自訂表單中新增500個欄位和Widget。 不過，根據表單的複雜性，當表單上存在超過100個時，可能會發生效能降低。
   >
   >
   >複雜表單的範例包括含有階層式引數的表單、計算的自訂資料欄位，以及單一欄位中的多個值選項。

1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

### 欄位名稱和標籤的附註 {#notes-on-field-names-and-labels}

標籤適用於大多數欄位。 這是描述性標籤，顯示在自訂表單上的欄位或Widget上方。 您可以隨時變更標籤。

>[!NOTE]
>
>請避免在此標籤中使用特殊字元，因為這些字元在報表中無法正確顯示。

每個欄位都必須有名稱。 此名稱是當您新增自訂欄位至Workfront的各個區域時（例如報表、首頁和API互動），系統識別該欄位的方法。 當您首次設定欄位或Widget且輸入標籤時，會自動填入名稱欄位以和欄位相符。 「標籤」和「名稱」欄位未同步。 這可讓您選擇變更使用者看到的標籤，而不必變更系統看到的名稱。

每個自訂欄位名稱在貴組織的Workfront例項中必須是唯一的。 如此一來，您便可重複使用已針對其他自訂表單建立的表單。

>[!NOTE]
>
>雖然可以這樣做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果這樣做，系統將不再識別現在可能在Workfront其他區域參考該欄位的自訂欄位。
>>例如，如果您新增自訂欄位至報表，之後又變更其名稱，Workfront將無法辨識報表中的自訂欄位，且除非您使用新名稱將其重新新增至報表，否則將無法正常運作。
>
>建議您不要輸入已用於內建Workfront欄位的名稱。
>
>建議您不要在自訂欄位名稱中使用句號/點字元，以防止在Workfront的不同區域使用欄位時發生錯誤。

自訂欄位標籤和名稱不支援下列特殊字元。

* \t
* \n
* \r
* \f
* `[`
* `]`
* (
* )
* ：
* `{`
* `}`

### 新增文字欄位

您可以將數個不同的文字欄位新增至自訂表格。

+++ 展開以檢視可用文字欄位的說明。

* **單行文字欄位**：允許使用者在欄位中輸入單行文字。
* **段落欄位**：允許使用者在欄位中輸入多行文字。
* **含格式的文字欄位**：可讓使用者在欄位中輸入多行文字，並以粗體、斜體、底線、專案符號、編號、超連結和區塊引號來格式化文字。 15,000的字元限制可提供大量的文字和格式。

  清單和報告上的篩選器不支援此自訂欄位型別。

  如需有關透過API存取此欄位的資訊，請參閱[ API中的RTF文字欄位儲存體](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md)。

  >[!NOTE]
  >
  >含有格式的文字欄位不適用於Workfront行動應用程式（將於未來發行版本中提供）。

* **描述性文字**：可讓您加入Workfront外部頁面的指示和連結。

+++

若要新增文字欄位：

1. 在畫面左側的&#x200B;**新欄位**&#x200B;索引標籤中，尋找下列文字欄位之一，並將其拖曳至畫布上的區段：

   * 單行文字
   * 段落
   * 含格式的文字
   * 描述文字

   ![將欄位拖曳到節](assets/drag-field-to-section.png)

1. 在畫面的右側，設定您新增之自訂欄位型別的可用選項：

   <table>
    <tr>
    <td>輸入至</td>
    <td>說明</td>
    <td>可用於 </td>
    </tr>
    <tr>
    <td>大小</td>
    <td><p>（選用）變更表單上文字欄位的大小。<p>
   </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落</li>
    <li>含格式的文字</li>
    <li>描述文字</li>
    </ul></td>
    </tr>
    <tr>
    <td>標籤</td>
    <td><p>（必要）輸入描述性標籤以顯示於欄位上方。 您可以隨時變更標籤。<p>
    <p><b>重要</b>：請避免在此標籤中使用特殊字元，因為這些字元在報表中無法正確顯示。 如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p></td>
    <td><ul>
    <li>單行文字</li>
    <li>段落</li>
    <li>含格式的文字</li>
    </ul></td>
    </tr>
    <tr>
     <td>姓名</td>
    <td><p>（必要）此名稱是系統識別欄位的方式。 當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 「標籤」和「名稱」欄位未同步。 這可讓您選擇變更使用者看到的標籤，而不必變更系統看到的名稱。</p>
    <p>如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p>
    </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落</li>
    <li>含格式的文字</li>
    <li>描述文字</li>
    </ul></td>
    </tr>
    <tr>
    <td>指示</td>
    <td>輸入有關欄位的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落</li>
    <li>含格式的文字</li>
    </ul></td>
    </tr>
    <tr>
    <td>格式</td>
    <td><p>選取將在自訂欄位中擷取的資料型別。</p> <p><b>附註</b>：   
    <ul> 
    <li>表單儲存後無法編輯此欄位。 如果您要在數學計算中使用欄位，請務必選取「數字」或「貨幣」格式。</li> 
    <li>當您選取「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</li>
    <li>數字欄位的字元限製為16。 您也可以使用文字欄位來輸入數字並避免限制。</li>
     </ul></p></td> </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落</li>
    </ul></td>
    </tr>
    <tr>
    <td>顯示類型</td>
    <td>在單行與段落文字欄位之間切換。</td>
    <td><ul>
    <li>單行文字</li>
    <li>段落</li>
    </ul></td>
    </tr>
    <tr>
    <td>超連結</td>
    <td> 如果要將超連結套用至您輸入的描述文字，請在此處新增。 描述性文字在附加表單的物件上顯示為連結。</td>
    <td><ul><li>描述文字</li></ul></td>
    </tr>
    <tr>
     <td><span class="preview">作用中</span></td>
     <td><span class="preview"><p>此選項預設為開啟。<p><p>將欄位設為「非使用中」時，該欄位會從報表、篩選器和檢視中排除，並且無法再用於自訂表單欄位程式庫。</p></span></td>
     <td><ul><span class="preview">
     <li>單行文字</li>
     <li>段落</li>
     <li>含格式的文字</li>
     <li>描述文字</li></span></ul></td>
    </tr>
    <tr> 
      <td role="rowheader">設為必要欄位</td>
      <td><p>如果您希望欄位是使用者完成自訂表單的必要欄位，請選取此選項。</p></td>
    <td><ul>
    <li>單行文字</li>
    <li>段落</li>
    <li>含格式的文字</li>
    </ul></td> 
    </tr> 
   </table>

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

### 新增計算欄位

在自訂表單中，您可以新增計算自訂欄位，以在自訂表單附加至物件時，使用現有資料產生新資料。

若要新增計算欄位，請參閱[使用表單設計工具新增計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

### 新增選項按鈕、核取方塊群組和下拉式清單

您可以將選項按鈕、核取方塊群組、下拉式清單及多選下拉式清單新增至自訂表單。

+++ 展開以檢視可用欄位的說明。

* **選項按鈕**：要求使用者只選取一個選項。
* **核取方塊群組**：允許使用者選取多個選項。
* **單選下拉式清單**：提供下拉式清單選項清單。
* **多重選取下拉式清單**：可讓使用者從下拉式清單中選取多個選項。

+++

>[!NOTE]
>
>允許進行多重選取的欄位（例如「核取方塊群組」和「多重選取下拉式清單」）很難在報告中建立圖表和群組。 若要更輕鬆地在報表中進行圖表和分組，您可以為每個選擇建立個別欄位（例如單行文字欄位）。

若要新增選項按鈕、核取方塊群組和下拉式清單：

1. 在畫面左側的&#x200B;**新欄位**&#x200B;索引標籤中，尋找下列其中一個欄位並將其拖曳至畫布上的區段：

   * 選項按鈕
   * 核取方塊群組
   * 單選下拉式清單
   * 多選下拉式清單

   ![將欄位拖曳到畫布上](assets/drag-field-to-section.png)

1. 在畫面的右側，設定您新增之自訂欄位型別的可用選項：

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>輸入至</td>
    <td>說明</td>
    <td>可用於 </td>
    </tr>
    <tr> 
     <td role="rowheader">標籤</td> 
     <td> <p>（必要）輸入描述性標籤，以在自訂欄位上方顯示。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元，因為這些字元在報表中無法正確顯示。 如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td> 
     <td><ul>
    <li>選項按鈕</li>
    <li>核取方塊群組</li>
    <li>單選下拉式清單</li>
    <li>多選下拉式清單</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">姓名</td> 
     <td> <p>（必要）此名稱是系統識別欄位的方式。 當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 「標籤」和「名稱」欄位未同步。 這可讓您選擇變更使用者看到的標籤，而不必變更系統看到的名稱。</p> 
    <p>如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td>
     <td><ul>
    <li>選項按鈕</li>
    <li>核取方塊群組</li>
    <li>單選下拉式清單</li>
    <li>多選下拉式清單</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">指示</td> 
    <td> <p>輸入自訂欄位的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>選項按鈕</li>
    <li>核取方塊群組</li>
    <li>單選下拉式清單</li>
    <li>多選下拉式清單</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">格式</td> 
    <td> <p>選取將在自訂欄位中擷取的資料型別。</p> <p><b>附註</b>：   
     <ul> 
    <li>表單儲存後無法編輯此欄位。 如果您要在數學計算中使用欄位，請務必選取「數字」或「貨幣」格式。<br></li> 
    <li>當您選取「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</li>
    <li>數字欄位的字元限製為16。 您也可以使用文字欄位來輸入數字並避免限制。</li>
     </ul></p></td> 
     <td><ul>
    <li>選項按鈕</li>
    <li>核取方塊群組</li>
    <li>單選下拉式清單</li>
    <li>多選下拉式清單</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">顯示類型</td> 
    <td>在欄位的選項按鈕、核取方塊群組、單選下拉式清單或多選下拉式清單之間切換。</td> 
    <td><ul>
    <li>選項按鈕</li>
    <li>核取方塊群組</li>
    <li>單選下拉式清單</li>
    <li>多選下拉式清單</li>
    </ul></td>
    </tr> 
    <td role="rowheader">選擇 </td> 
    <td> 
    <p>選取下列任一選項：</p> 
    <ul> 
    <li><strong>顯示值</strong>：顯示欄位中每個選擇的值。 依預設，會顯示每個選擇的標籤。</li>
   <li><strong>排序選擇A-Z</strong>：依字母順序排序您在欄位中新增的選擇。</li>
    </ul>
     <p>針對您為使用者新增的每個選擇，按一下齒輪圖示<img src="assets/gear-icon-settings.png">，然後選取下列其中一個選項：</p> 
    <ul> 
    <li><strong>依預設選取</strong>：依預設在欄位中選取選項。</li> 
    <li> <p><strong>隱藏選擇</strong>：隱藏欄位中的選擇。 隱藏的選擇在報表中仍可存取。</p> </li> 
    <li> <p><strong>移除選擇</strong>：從欄位移除選擇。</p> <p><b>警告</b>：如果您有使用此選擇的目前物件，請勿將其從欄位移除。 移除它將會導致歷史資料遺失。 相反地，選取要隱藏它的選項，這會防止使用者在將來選取它。</p> </li> 
    </ul>   
    <p><b>注意：</b>您可以選取的選項數目沒有限制。 </p>    
    </td> 
    <td><ul>
    <li>選項按鈕</li>
    <li>核取方塊群組</li>
    <li>單選下拉式清單</li>
    <li>多選下拉式清單</li>
    </ul>
    </td>
     </tr>
    <tr>
     <td><span class="preview">作用中</span></td>
     <td><span class="preview"><p>此選項預設為開啟。<p><p>將欄位設為「非使用中」時，該欄位會從報表、篩選器和檢視中排除，並且無法再用於自訂表單欄位程式庫。</p></span></td>
     <td><ul><span class="preview">
     <li>選項按鈕</li>
     <li>核取方塊群組</li>
     <li>單選下拉式清單</li>
     <li>多選下拉式清單</li></span></ul></td>
    </tr>
    <tr> 
    <td role="rowheader">設為必要欄位</td> 
    <td>如果您希望欄位是使用者完成自訂表單的必要欄位，請選取此選項。 </td> 
    <td><ul>
    <li>選項按鈕</li>
    <li>核取方塊群組</li>
    <li>單選下拉式清單</li>
    <li>多選下拉式清單</li>
    </ul></td>
     </tr> 
    <tr> 
    </tbody> 
    </table>

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

### 新增預先輸入和日期欄位

您可以將預先輸入和日期欄位新增至自訂表單。

+++ 展開以檢視可用欄位的說明。

* **自動提示**：允許使用者輸入Workfront中存在的物件名稱。 當使用者開始輸入時，建議清單隨即出現。 此欄位型別支援下列物件：
   * 使用者
   * 群組
   * 職務角色
   * 產品組合
   * 方案
   * 專案
   * 團隊
   * 範本
   * 公司
* **日期**：顯示一個行事曆，使用者可以在其中選取日期和時間。

+++

若要新增預先輸入和日期欄位：

1. 在畫面左側的&#x200B;**新欄位**&#x200B;索引標籤中，尋找下列其中一個欄位並將其拖曳至畫布上的區段。

   * 自動提示
   * 日期

   ![將欄位拖曳到節](assets/drag-field-to-section.png)

1. 在畫面的右側，設定您新增之自訂欄位型別的可用選項：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>欄位設定</td>
    <td>說明</td>
    <td>可用於 </td>
    </tr>
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入描述性標籤，以在自訂欄位上方顯示。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元，因為這些字元在報表中無法正確顯示。 如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td> 
       <td><ul>
    <li>自動提示</li>
    <li>日期</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別欄位的方式。 當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 「標籤」和「名稱」欄位未同步。 這可讓您選擇變更使用者看到的標籤，而不必變更系統看到的名稱。</p> 
      <p>如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td>
    <td><ul>
    <li>自動提示</li>
    <li>日期</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入自訂欄位的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>自動提示</li>
    <li>日期</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">顯示當日時間</td> 
      <td>如果您要在欄位中顯示一天中的時間和日期，請選取此選項。</td> 
         <td><ul>
    <li>日期</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">參考物件類型</td> 
      <td> <p>選取您要與欄位關聯的物件型別。</p> <p>按一下<b>套用</b>或<b>儲存並關閉</b>後，您就無法變更欄位的物件型別。</p> <p><b>附註</b>：   
        <ul> 
         <li>如果您的Workfront管理員在Workfront使用者介面中為投資組合、程式或專案自訂名稱，則該物件的預設Workfront名稱會出現在下拉式清單中，而不是自訂名稱。 如果您需要這方面的協助，請洽詢Workfront管理員。<br></li> 
         <li>iOS和Android Workfront Mobile應用程式支援下列物件型別：使用者、公司、群組、工作角色、Portfolio、方案、專案和範本。</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>自動提示</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">新增篩選器</td>
      <td><p>為物件型別新增篩選條件，以限制使用者在使用欄位時可以選擇的物件。 </p> <p>例如，您可以限制欄位，讓使用者名稱只有在符合以下條件時才可選取：</p> 
       <ul> 
        <li>它們屬於您指定的群組。</li> 
        <li>它們與您指定的角色或職稱相關聯。</li> 
        <li>他們與使用欄位的人屬於同一群組。</li> 
       </ul>
       <p>您必須使用「文字模式」語法來定義所選物件型別的濾鏡。 如需有關使用文字模式建立篩選的資訊，請參閱<a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">使用文字模式編輯篩選</a>。</p>
       <p><b>秘訣：</b>您可以先建立報表以測試您的篩選器，然後再將篩選器直接新增至自動提示欄位。 這可協助您驗證篩選器是否傳回正確的物件。 然後，您可以在報表中切換到文字模式、複製文字模式陳述式，並將其新增至自動提示篩選。</p>
       <p><b>附註</b>：
       <ul> 
        <li>如果您正在編輯現有的自訂表單，將篩選條件新增至預先輸入欄位時，不會移除使用者已使用該欄位新增的任何物件（在篩選條件範圍之外）。</li> 
        <li>此篩選器不適用於行動裝置。 如果您針對預先輸入欄位使用篩選器，則該欄位會顯示在不受篩選器影響之使用者的行動裝置上。</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>自動提示</li>
       </ul>
      </td>
     </tr>
     <tr>
      <td><span class="preview">作用中</span></td>
      <td><span class="preview"><p>此選項預設為開啟。<p><p>將欄位設為「非使用中」時，該欄位會從報表、篩選器和檢視中排除，並且無法再用於自訂表單欄位程式庫。</p></span></td>
      <td><ul><span class="preview">
      <li>自動提示</li>
      <li>日期</li></span></ul></td>
     </tr>
     <tr> 
      <td role="rowheader">設為必要欄位</td> 
      <td>如果您希望欄位是使用者完成自訂表單的必要欄位，請選取此選項。 </td> 
       <td><ul>
    <li>自動提示</li>
    <li>日期</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

### 新增外部查詢欄位

外部查詢欄位會呼叫外部API，並在下拉式欄位中傳回值作為選項。 使用自訂表單附加至之物件的使用者可從下拉式清單中選取一或多個這些選項，視外部查閱欄位是單一或多重選取欄位而定。 清單和報告中也提供外部查詢欄位。

如需使用外部查詢欄位來呼叫相同Workfront執行個體或公用API的範例，請參閱[自訂表單中的外部查詢欄位範例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)。

>[!NOTE]
>
>* Outlook外掛程式不支援外部查閱欄位。
>* 當欄位與其他欄位相依時，清單中無法使用外部查詢欄位。

若要新增外部查詢：

1. 在畫面左側的&#x200B;**新欄位**&#x200B;索引標籤中，尋找&#x200B;**外部查詢**&#x200B;或&#x200B;**多重選取外部查詢**，並將其拖曳至畫布上的區段。
1. 在畫面右側，設定自訂欄位的選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入描述性標籤，以在自訂欄位上方顯示。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元，因為這些字元在報表中無法正確顯示。 如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別欄位的方式。 當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 但是「標籤」和「名稱」欄位不同步，因此您可以選擇變更使用者看到的標籤，而不必變更系統看到的名稱。</p>
      <p>如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td>
     </tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入自訂欄位的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td>
      <td><p>選取將在自訂欄位中擷取的資料型別。</p>
      <p><strong>注意：</strong></p>
      <ul><li>您可以在儲存表單後變更格式型別，但有一個限制：物件上的所有現有值都必須能夠轉換為新型別。 （例如，如果格式型別是Text，而物件正在儲存「abc」值，則您無法轉換欄位，且會收到系統無法將「abc」轉換為數字/貨幣的錯誤。） 如果您要在數學計算中使用欄位，請務必選取「數字」或「貨幣」格式。</li>
      <li>當您選取「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</li>
      <li>數字欄位的字元限製為16。 您也可以使用文字欄位來輸入數字並避免限制。</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">基底 API URL</td> 
      <td><p>輸入或貼上API的URL。</p><p>API URL必須傳回您要在下拉式清單中顯示的選項的JSON內容。 您可以使用JSON路徑欄位，從傳回的JSON中選取特定值作為下拉式選項。</p><p>輸入API URL時，您可以選擇在URL中傳遞下列值：</p>
      <ul>
      <li>$$HOST — 這代表目前的Workfront主機，可用來對Workfront API進行/搜尋API呼叫。 使用此萬用字元時，會處理驗證，使用者不需要傳送驗證標題。 （例如，使用者可以使用基本URL <code>$$HOST/attask/api/task/search</code>來搜尋工作，而且它允許搜尋工作並從傳回的工作清單中選取值。）</li>
      <li><p>$$QUERY — 這代表一般使用者在欄位中輸入的搜尋文字，可讓您為一般使用者實作查詢篩選。 （使用者會在下拉式清單中搜尋值。）</p>
      <p>如果您參考的API允許，您也可以在搜尋查詢中包含修飾詞，以識別搜尋應該如何運作。 例如，您可以使用下列作為基礎API URL，以允許人員搜尋包含特定文字的任何Workfront專案： <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>。</p><p>進一步瞭解<a href="/help/quicksilver/wf-api/general/api-basics.md">API基本知識</a>中的Workfront搜尋修飾詞。</p>
      <p><strong>注意：</strong>如果您未使用$$QUERY，而且使用者在搜尋方塊中輸入文字，將會縮小您現有的選擇。 但是，如果您使用$$QUERY且使用者鍵入任何內容，則會對您的API執行新的網路呼叫。 因此，如果您的API中有超過2000個值，且API支援查詢，您便可以利用$$QUERY來不僅搜尋現有2000個值，而且搜尋具有縮小選項的原始API。</p></li>
      <li><p>{fieldName} — 其中fieldName是Workfront中的任何自訂或原生欄位。 這樣，當您將已選取欄位的值傳遞至外部查詢欄位以篩選下拉選項時，您就可以實作階層式下拉選項篩選器。 （例如，「地區」欄位已存在於表單上，而您正在將國家/地區清單從API縮小至特定地區。）</p>
      <p>對於相依於其他欄位（使用{fieldName}語法）的外部查詢欄位，從API傳回的選項僅限於符合在其他欄位中輸入的任何字串或值的選項。 （清單和報告不支援此功能。）</p></li>
      <li>{referenceObject}。{fieldName} — 其中欄位是物件的一部分。 此語法類似於自訂運算式。 (例如，portfolioID={project}。{portfolioID})</li></ul>
      <p><strong>秘訣：</strong>檢閱您正在使用的API檔案，以瞭解您可以定義的特定查詢。</p></td>
     </tr>
     <tr> 
      <td role="rowheader">HTTP 方法</td> 
      <td>為方法選取<strong>Get</strong>、<strong>Post</strong>或<strong>Put</strong>。</td> 
     </tr>
     <tr> 
      <td role="rowheader">JSON 路徑</td>
      <td><p>輸入或貼上API的JSON路徑。</p> <p>此選項允許從API URL傳回的JSON擷取資料。 這可當作選取要讓JSON內的哪些值會出現在下拉式選項中的方式。</p><p>例如，如果您的API URL以下列格式傳回JSON，則您可以使用「$.data[*].name」選取美國和加拿大作為下拉式選項：</br>
      <pre>
      {
       資料： {
         { name： "USA"}，
         { name： "Canada"}
       }
      }
      </pre>
      </p>
     <p>如需有關JSON路徑並確保您撰寫正確JSON路徑的詳細資訊，請參閱<a href="https://jsonpath.com/">https://jsonpath.com/</a>。</p></td>
     </tr>
     <tr> 
      <td role="rowheader">標頭</td>
      <td><p>按一下<strong>新增標題</strong>，然後輸入或貼上使用API驗證所需的金鑰值組。</p><p><strong>注意：</strong>標頭欄位不是儲存認證的安全位置，您應該注意輸入和儲存的內容。</p></td>
     </tr>
     <tr> 
      <td role="rowheader">多選下拉式清單</td>
      <td><p>選取此選項可允許使用者在下拉式清單中選取多個值。</p></td>
     </tr>
     <tr>
      <td><span class="preview">作用中</span></td>
      <td><span class="preview"><p>此選項預設為開啟。<p><p>將欄位設為「非使用中」時，該欄位會從報表、篩選器和檢視中排除，並且無法再用於自訂表單欄位程式庫。</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader">設為必要欄位</td>
      <td><p>如果您希望欄位是使用者完成自訂表單的必要欄位，請選取此選項。</p></td>
     </tr>       
    </tbody>
   </table>

1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

>[!NOTE]
>
>以下專案為呼叫外部API的技術限制：
>
>* 選項最大數量： 2000 （只顯示傳回JSON中的前2000個唯一選項）
>* 逾時： 30秒
>* 重試次數： 3
>* 重試之間的等待持續時間：500毫秒
>* 預期的回應狀態： 2xx

### 新增影像、PDF和影片

您可以將影像、PDF和視訊新增至自訂表單。 使用自訂表單附加至之物件的使用者只能在下列區域檢視影像、PDF或影片：

* 物件的「詳細資訊」區域（例如，針對專案，則為「專案詳細資訊」區域）。
* 物件的「編輯」方塊(如果它具有新的Adobe Workfront體驗外觀) （例如「編輯專案」和「編輯任務」方塊）。

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ 展開以檢視可用欄位的說明。

* **影像**：允許使用者新增影像檔案。
* **PDF**：允許使用者新增PDF
* **影片**：允許使用者新增影片檔案。

+++

若要新增影像、PDF或視訊：

1. 在畫面左側的&#x200B;**新欄位**&#x200B;索引標籤中，尋找下列其中一個欄位並將其拖曳至畫布上的區段。

   * 影像
   * PDF
   * 影片

   ![將欄位拖曳到節](assets/drag-field-to-section.png)

1. 為Widget輸入或編輯下列任一屬性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">大小</td> 
      <td>（選用）視需要變更Widget的顯示大小。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要顯示在Widget上方的描述性標籤。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元，因為這些字元在報表中無法正確顯示。 如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別Widget的方式。 當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 「標籤」和「名稱」欄位未同步。 這可讓您選擇變更使用者看到的標籤，而不必變更系統看到的名稱。</p> <p>如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必要）輸入或貼上儲存於網際網路之Widget的URL。</p> 
      <p>如果您新增視訊Widget，目前可在URL方塊中新增下列內容來完成此操作：</p> 
      <ul> 
      <li> <p>YouTube或Vimeo連結</p> </li> 
      <li> <p>Google Drive影片連結</p> </li> 
      <li> <p>使用MP4和MOV擴充功能的視訊連結</p> </li> 
      <li> <p>視訊連結已上傳至Workfront執行個體中的檔案區域。 如需指示，請參閱本文中的<a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">從檔案區域</a>新增視訊Widget至自訂表單。</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關Widget的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> </td> 
     </tr> 
     <tr>
      <td><span class="preview">作用中</span></td>
      <td><span class="preview"><p>此選項預設為開啟。<p><p>將欄位設為「非使用中」時，該欄位會從報表、篩選器和檢視中排除，並且無法再用於自訂表單欄位程式庫。</p></span></td>
     </tr>
    </tbody> 
   </table>

   >[!NOTE]
   >若是PDF，建議使用「大」作為Widget的顯示大小。
   >瀏覽器的PDF檢視器會影響使用者的顯示效果，而如果PDF顯示效果不是最佳，則他們可能需要調整視窗大小和瀏覽器縮放百分比。

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

#### 從檔案區域新增視訊至自訂表單{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>以這種方式將視訊新增至自訂表單時，使用者存取物件上的表單時，在「檔案」區域中設定的許可權會套用至視訊。

1. 移至[檔案]區域中的視訊並產生其校訂，如[為網站或其他網頁內容建立互動式校訂](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md)中所述。
1. 開啟校訂。
1. 以滑鼠右鍵按一下視訊上的任何位置，然後選取&#x200B;**複製視訊位址**。
1. 在您新增視訊Widget的自訂表單中，將複製的地址貼到&#x200B;**URL**&#x200B;方塊中。
1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

### 新增Workfront原生欄位

您可以將Workfront原生欄位新增至自訂表單。 當自訂表單附加到物件時，會從物件資料填入欄位。 例如，附加到專案的自訂表單上的說明欄位將提取專案說明。 （如果沒有可用資料，欄位可能會顯示「N/A」。）

+++ 展開以檢視支援的原生欄位清單。

此表格列出自訂表單中特定Workfront物件的可用原生欄位。

| 欄位名稱 | 專案 | 任務 | 問題 | 範本 | 範本任務 | 產品組合 | 方案 | 群組 |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| 實際完成日期 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 實際期間 | ✓ |   |   |   |   |   |   |   |
| 實際時數 | ✓ |   | ✓ |   |   |   |   |   |
| 實際開始日期 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 公司 | ✓ |   |   | ✓ |   |   |   |   |
| 條件 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 狀況類型 | ✓ |   |   | ✓ |   |   |   |   |
| 說明 | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| 期間 |   | ✓ |   |   | ✓ |   |   |   |
| 期間類型 |   | ✓ |   |   | ✓ |   |   |   |
| 期間單位 |   | ✓ |   |   | ✓ |   |   |   |
| 輸入者 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| 輸入日期 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| 群組 | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| 上次更新者 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 上次更新日期 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 姓名 | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| 所有者 | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| 規劃完成日期 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 計畫持續時間 | ✓ |   |   | ✓ |   |   |   |   |
| 規劃時數 | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| 規劃開始日期 | ✓ |   |   |   |   |   |   |   |
| 產品組合 | ✓ |   |   | ✓ |   |   | ✓ |   |
| 優先順序 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 方案 | ✓ |   |   | ✓ |   |   |   |   |
| 預計完成日期 | ✓ | ✓ |   |   |   |   |   |   |
| 預計期間 (分鐘) |   | ✓ |   |   |   |   |   |   |
| 預計開始日期 | ✓ | ✓ |   |   |   |   |   |   |
| 參考號碼 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 排程模式 | ✓ |   |   | ✓ |   |   |   |   |
| 嚴重程度 |   |   | ✓ |   |   |   |   |   |
| 贊助者 | ✓ |   |   | ✓ |   |   |   |   |
| 狀態 | ✓ | ✓ |   |   |   |   |   |   |
| 腳本點數 |   | ✓ |   |   |   |   |   |   |
| 範本 | ✓ |   |   |   |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

+++

1. 在畫面左側的&#x200B;**新欄位**&#x200B;索引標籤中，尋找&#x200B;**原生欄位參考**&#x200B;並將其拖曳至畫布上的區段。
1. 在畫面右側，設定自訂欄位的選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">大小</td> 
      <td>（可選）視需要變更欄位的顯示大小。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入描述性標籤以顯示於欄位上方。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元，因為這些字元在報表中無法正確顯示。 如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td>
      <td> <p>（必要）此名稱是系統識別欄位的方式。 當您第一次設定欄位並輸入標籤時，「名稱」欄位會自動填入以和欄位相符。 「標籤」和「名稱」欄位未同步。 這可讓您選擇變更使用者看到的標籤，而不必變更系統看到的名稱。</p>
      <p>如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關欄位的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">參考欄位</td> 
      <td><p>（必要）選取Workfront原生欄位。<p><p>僅表單物件的原生欄位可用。 例如，如果表單設計器頂端的「物件型別」清單顯示「專案」，您將能夠選取專案的原生欄位，但不能選取任務特定的欄位。</p></td>
     </tr>
     <tr>
      <td role="rowheader">新增篩選器</td>
      <td><p>為參考欄位新增篩選器，以限制使用者在使用欄位時可以選擇的專案清單。 </p> <p>例如，您可以限制欄位，讓使用者名稱只有在符合以下條件時才可選取：</p> 
       <ul>
        <li>它們屬於您指定的群組。</li> 
        <li>它們與您指定的角色或職稱相關聯。</li> 
        <li>他們與使用欄位的人屬於同一群組。</li> 
       </ul>
       <p>您必須使用「文字模式」語法來定義所選參考欄位的篩選器。 如需詳細資訊，請參閱<a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">使用文字模式編輯篩選器</a>。</p>
       <p><b>附註</b>：
       <ul> 
        <li>篩選選項僅在您參考原生預先輸入欄位時可用，例如Portfolio、公司或所有者。</li>
        <li>如果您正在編輯現有的自訂表單，將篩選新增至原生欄位時，不會移除使用者已使用該欄位新增的任何物件（在篩選範圍之外）。</li> 
        <li>此篩選器不適用於行動裝置。 如果您將篩選用於原生欄位，該欄位將會顯示在不受篩選影響之使用者的行動裝置上。</li> 
        </ul></p></td> 
      <td>
     </tr>
     <tr>
      <td><span class="preview">作用中</span></td>
      <td><span class="preview"><p>此選項預設為開啟。<p><p>將欄位設為「非使用中」時，該欄位會從報表、篩選器和檢視中排除，並且無法再用於自訂表單欄位程式庫。</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader">設為必要欄位</td>
      <td><p>如果您希望欄位是使用者完成自訂表單的必要欄位，請選取此選項。</p></td>
     </tr> 
    </tbody> 
   </table>

1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

### 新增Adobe XD檔案

您可以將Adobe XD原型直接新增至自訂表單。 使用自訂表單附加至之物件的使用者只能在下列區域中看到Adobe XD檔案：

* 物件的「詳細資訊」區域（例如，專案的「詳細資訊」區域）
* 物件的「編輯」方塊(如果它具有新的Adobe Workfront體驗外觀) （例如「編輯專案」和「編輯任務」方塊）

新增Adobe XD檔案：

1. 在畫面左側的&#x200B;**新欄位**&#x200B;索引標籤中，尋找&#x200B;**Adobe XD**&#x200B;並將其拖曳至畫布上的區段。
1. 為Widget輸入或編輯下列任一屬性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">大小</td> 
      <td>（選用）視需要變更Widget的顯示大小。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要顯示在Widget上方的描述性標籤。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元，因為這些字元在報表中無法正確顯示。 如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別Widget的方式。 當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 「標籤」和「名稱」欄位未同步。 這可讓您選擇變更使用者看到的標籤，而不必變更系統看到的名稱。</p>
    <p>如需詳細資訊，請參閱<a href="design-a-form.md#notes-on-field-names-and-labels">欄位名稱和標籤的附註</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必要）輸入或貼上有效的XD原型連結。</p> 
      <p><b>注意</b>： Adobe XD中「共用」標籤上的「連結存取」設定必須設定為「擁有連結的任何人」。 否則，使用者將無法檢視原型。 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關Widget的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr>
     <tr>
      <td><span class="preview">作用中</span></td>
      <td><span class="preview"><p>此選項預設為開啟。<p><p>將欄位設為「非使用中」時，該欄位會從報表、篩選器和檢視中排除，並且無法再用於自訂表單欄位程式庫。</p></span></td>
     </tr>
    </tbody> 
   </table>

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

### 新增Planning連線欄位

>[!IMPORTANT]
>
>本節中的資訊說明Adobe Workfront的額外功能Adobe Workfront Planning。
>
>您必須具備下列專案才能存取Workfront Planning：
>
>* 新的Workfront計畫和授權。 舊版Workfront計畫或授權無法使用Workfront計畫。
>* 適用於Workfront Planning的額外套件。
>* 貴組織的Workfront執行個體必須上線至Adobe統一體驗。
>
> 如需存取Workfront Planning的完整需求清單，請參閱[Adobe Workfront Planning存取總覽](/help/quicksilver/planning/access/access-overview.md)。
> 
>如需Workfront Planning的詳細資訊，請參閱[Adobe Workfront Planning概觀](/help/quicksilver/planning/general/planning-overview.md)。

您可以將Workfront連線自訂欄位新增至物件的自訂表單，在Workfront物件的自訂欄位中檢視從Planning連線的記錄。

您可以將Planning連線欄位新增至所有物件的自訂表單。 不過，您只能在與Workfront物件(可從Workfront Planning連線)相關聯的自訂表單上顯示連線的記錄。

>[!NOTE]
>
>在自訂欄位中檢視資訊的使用者必須有權存取Workfront Planning，以及包含連線至Workfront物件之記錄型別的工作區。

新增Planning連線欄位：

1. 在畫面左側的&#x200B;**新欄位**&#x200B;索引標籤中，尋找&#x200B;**Planning連線**，並將其拖曳至畫布上的區段。
1. 在畫面右側，設定自訂欄位的選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">大小</td> 
      <td>（選用）視需要變更Widget的顯示大小。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入描述性標籤以顯示於欄位上方。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。</p> 
      <p>建議您選擇一個有助於您輕鬆識別Planning記錄來源的標籤。 新增工作區名稱或記錄型別名稱之類的資訊。 </p>   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td>
      <td> <p>（必要）名稱是系統識別欄位的方式。 當您第一次設定欄位並輸入標籤時，「名稱」欄位會自動填入以和欄位相符。 「標籤」和「名稱」欄位未同步。 這可讓您選擇變更使用者看到的標籤，而不必變更系統看到的名稱。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>（建議）輸入欄位的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p>
      <p>您可以在此處新增有關記錄和您連線之物件的詳細資訊。 </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">物件類型</td> 
      <td><p>（必要）選取已連線至Workfront Planning中記錄型別的Workfront物件型別。</p>
      您可以從下列物件型別中選取：
      <ul><li> 專案</li>
      <li> 產品組合</li><li> 方案</li><li> 公司</li><li> 群組</li></ul>
       <p>只有表單物件型別的Workfront物件型別可用。</p> <p> 例如，如果表單設計器頂端的「物件型別」清單顯示「專案」，則您只能在此欄位中選取「專案」，而不能選取「產品組合」，儘管產品組合也可以連線到記錄型別。</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">工作區</td> 
      <td> <p>（必要）選取您要在Workfront中顯示之記錄來自的Planning工作區。</p> <p> 只有與您在「物件型別」欄位中選取的物件型別連線的工作區才會顯示。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">記錄類型</td> 
      <td><p>（必要）選取與Workfront物件型別有關聯的Workfront Planning記錄型別。</p><p>只有與您在「物件型別」欄位中選取的物件型別有連線的記錄型別才會顯示。 </p></td> 
     </tr>
     <tr> 
      <td role="rowheader">連線欄位</td> 
      <td><p>（必要）選取要顯示在Workfront物件上的所選Planning記錄型別與Workfront物件型別之間的連線欄位。 </p> <p> <b>注意</b>：在相同物件和記錄型別之間可以有多個連線欄位，但只能選取一個欄位。</p>  </td> 
     </tr>

<tr> 
      <td role="rowheader">記錄類型欄位</td> 
      <td><p>（可選）從連線的記錄型別中選取最多7個查詢欄位，以在自訂表單中顯示。 預設會選取主要欄位，且無法編輯。 </p> <p> 您選取的已連線記錄欄位會顯示在自訂表單的表格檢視中。 當表單附加至Workfront物件時，表格檢視是唯讀的。 </p>  
    <img src="assets/planning-connections-field-with-table-on-form-preview.png"></td> 
     </tr>
     <tr>
      <td><span class="preview">作用中</span></td>
      <td><span class="preview"><p>此選項預設為開啟。<p><p>將欄位設為「非使用中」時，該欄位會從報表、篩選器和檢視中排除，並且無法再用於自訂表單欄位程式庫。</p></span></td>
     </tr>
      </tbody> 
   </table>

1. （可選）重複上述步驟以新增任何其他欄位。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存您的變更，請按一下[套用] ****，然後移至其他區段以繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

   您現在可以將表單附加到從Workfront Planning連線的物件，並執行下列任一項作業：

   * 檢視連線至Workfront物件的Workfront記錄型別（如果有的話）。
   * 從Workfront物件連線或中斷連線記錄。

   如需詳細資訊，請參閱[管理來自Workfront物件的記錄連線](/help/quicksilver/planning/records/manage-records-in-planning-section.md)

### 新增UI擴充功能

使用UI擴充功能欄位型別，可將應用程式內嵌於Workfront自訂表單中。 若要建立UI擴充功能，您必須能在Adobe Developer Console中存取Adobe App Builder 。 如需詳細資訊，請參閱文章[使用Workfront App Builder為Workfront建立自訂應用程式](/help/quicksilver/app-builder/app-builder.md#embed-an-app-using-a-workfront-custom-form)中的[使用Adobe自訂表單內嵌應用程式](/help/quicksilver/app-builder/app-builder.md)。

## 使用表單設計工具來組織和預覽表單

有關如何使用分割槽符號組織自訂表單及預覽表單的資訊，請參閱[使用表單設計工具組織和預覽表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)。



