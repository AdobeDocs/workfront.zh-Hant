---
title: 使用表單設計工具設計表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表單設計工具來設計自訂表單。 您可以將自訂表單附加至不同的Workfront物件，以擷取這些物件的相關資料。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: 83036270d430dcc80069f4de87b6ac1e8da689e3
workflow-type: tm+mt
source-wordcount: '6079'
ht-degree: 4%

---

# 使用表單設計工具設計表單

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅適用於所有客戶的預覽環境，或適用於啟用快速發行的客戶的生產環境。</span>

<span class="preview">如需快速發行版本的相關資訊，請參閱 [啟用或停用組織的快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">如需目前版本的相關資訊，請參閱 [2024年第二季版本總覽](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

您可以使用表單設計工具來設計自訂表單。 您可以將自訂表單附加至不同的Workfront物件，以擷取這些物件的相關資料。

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr>  
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 開始設計自訂表單

{{step-1-to-setup}}

1. 按一下 **自訂Forms** 在左側面板中。

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. 按一下 **新增自訂表格。**
1. 選取您要附加自訂表單的物件型別，然後按一下 **繼續**.

   ![](assets/choose-object-type.jpg)

1. 在 **標題為必填** 區域，輸入自訂表單標題。
1. （選擇性）如果要將更多物件型別加入表單，以便將其附加到更多物件，請按一下 **新增** 圖示 ![](assets/add-objects-icon.png) 晚於 **物件型別**，然後在顯示的功能表中選取您想要的型別。 您可以重複此步驟，新增任意數目的物件型別。

   您也可以按一下物件型別上的X，將其從表單中刪除。

   >[!CAUTION]
   >
   >刪除自訂表單也會刪除與表單關聯的物件上的所有自訂資料。 已刪除的資料無法復原。 請考慮改為停用自訂表單 — 當停用您不再使用的自訂表單時，您可保留所有關聯的歷史資料。
   >
   >如需詳細資訊，請參閱 [刪除自訂表單上的物件型別](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).


1. 接下來，您可以開始將欄位新增至自訂表單。 請參閱下列章節：
   * [重複使用已在其他自訂表單中使用的現有欄位或Widget](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [新增文字欄位](#add-text-fields)
   * [新增計算欄位](#add-calculated-fields)
   * [新增選項按鈕、核取方塊群組和下拉式清單](#add-radio-buttons-checkboxes-and-dropdowns)
   * [新增預先輸入和日期欄位](#add-typeahead-and-date-fields)
   * [新增外部查詢欄位](#add-external-lookup-fields)
   * [新增影像、PDF和影片](#add-images-pdfs-and-videos)
   * [新增Workfront原生欄位](#add-workfront-native-fields)
   * [新增Adobe XD檔案](#add-adobe-xd-files)

## 新增欄位或現有欄位至您的自訂表單

在設計自訂表單時，您可以使用新的或現有的欄位。

## 重複使用已在其他自訂表單中使用的現有欄位或Widget

1. 在熒幕的左上角，按一下 **欄位程式庫**.

1. 將您想要的欄位或Widget拖曳至此以自訂表單顯示。
1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   >[!NOTE]
   >
   >您最多可以在單一自訂表單中新增500個欄位和Widget。 不過，根據表單的複雜性，當表單上存在超過100個時，可能會發生效能降低。
   >
   >
   >複雜表單的範例包括含有階層式引數的表單、計算的自訂資料欄位，以及單一欄位中的多個值選項。

1. 若要儲存變更，請按一下 **套用** 並移至另一個區段，以繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

### 新增文字欄位

您可以將數個不同的文字欄位新增至自訂表格。

+++ **展開以檢視可用文字欄位的說明**

* **單行文字欄位**：可讓使用者在欄位中輸入單行文字。
* **段落文字欄位**：可讓使用者在欄位中輸入多行文字。
* **含格式的文字欄位**：可讓使用者在欄位中輸入多行文字，並以粗體、斜體、底線、專案符號、編號、超連結和區塊引號格式化文字。 15,000的字元限制可提供大量的文字和格式。

  清單和報告上的篩選器不支援此自訂欄位型別。

  如需有關透過API存取此欄位的資訊，請參閱 [API中的RTF文字欄位儲存](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md).

  >[!NOTE]
  >
  >含有格式的文字欄位不適用於Workfront行動應用程式（將於未來發行版本中提供）。

* **描述文字**：可讓您加入指示，並連結至Workfront以外的頁面。

+++

若要新增文字欄位：

1. 在熒幕左側，找到下列其中一個文字欄位，並將其拖曳至畫布上的區段：

   * 單行文字
   * 段落文字
   * 含格式的文字欄位
   * 描述文字

   ![](assets/drag-field-to-section.png)

1. 在畫面的右側，設定您新增之自訂欄位型別的可用選項：

   <table>
    <tr>
    <td>輸入至</td>
    <td>說明</td>
    <td>可用於 </td>
    </tr>
    <tr>
    <td>大小</td>
    <td><p>變更表單上文字欄位的大小。<p>
   </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    <li>含格式的文字</li>
    <li>描述文字 — 即將推出</li>
    </ul></td>
    </tr>
    <tr>
    <td>標籤</td>
    <td><p>輸入要顯示在Widget上方的描述性標籤。 您可以隨時變更標籤。<p>
    <p>重要：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p></td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    <li>含格式的文字</li>
    </ul></td>
    </tr>
    <tr>
     <td>姓名</td>
    <td><p>（必要）此名稱是系統識別欄位的方式。 當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p>
    <p><b>重要</b>：   
      <ul> 
      <li>雖然可以這樣做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果這樣做，系統將不再識別現在可能在Workfront其他區域參考該欄位的自訂欄位。 <p>例如，如果您新增自訂欄位至報表，之後又變更其名稱，Workfront將無法辨識報表中的自訂欄位，且除非您使用新名稱將其重新新增至報表，否則將無法正常運作。</p> </li>
      <li> <p>建議您不要輸入已用於內建Workfront欄位的名稱。</p> </li>
      <li><p>建議您不要在自訂欄位名稱中使用句號/點字元，以防止在Workfront的不同區域使用欄位時發生錯誤。</p></li>
    </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    <li>含格式的文字</li>
    <li>描述文字</li>
    </ul></td>
    </tr>
    <tr>
    <td>指示</td>
    <td>輸入有關Widget的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    <li>含格式的文字</li>
    </ul></td>
    </tr>
    <tr>
    <td>格式</td>
    <td><p>選取將在自訂欄位中擷取的資料型別。</p> <p><b>注意</b>：   
    <ul> 
    <li>表單儲存後即無法編輯此欄位。 如果您要在數學計算中使用欄位，請務必選取「數字」或「貨幣」格式。</li> 
    <li>當您選取「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</li>
    <li>數字欄位的字元限製為16。 您也可以使用文字欄位來輸入數字並避免限制。</li>
     </ul></p></td> </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    </ul></td>
    </tr>
    <tr>
    <td>顯示類型</td>
    <td>在單行與段落文字欄位之間切換。</td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    </ul></td>
    </tr>
    <tr>
    <td>超連結</td>
    <td> 如果要將超連結套用至您輸入的描述文字，請在此處新增。 描述性文字在附加表單的物件上顯示為連結。</td>
    <td><ul><li>描述文字</li></ul></td>
    </tr>
   </table>

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至另一個區段，以繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

### 新增計算欄位

在自訂表單中，您可以新增計算自訂欄位，以在自訂表單附加至物件時，使用現有資料產生新資料。

若要新增計算欄位，請參閱 [使用表單設計工具新增計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### 新增選項按鈕、核取方塊和下拉式清單

您可以新增選項按鈕、核取方塊和下拉式清單至自訂表單。

+++ **展開以檢視可用欄位的說明**

* **選項按鈕**：要求使用者僅選取一個選項。
* **核取方塊群組**：可讓使用者選取多個選項。
* **下拉式清單**：提供下拉式清單選項的清單。

+++

>[!NOTE]
>
>允許進行多項選擇的欄位（例如「核取方塊群組」和「下拉式清單」）很難在報告中建立圖表和群組。 若要更輕鬆地在報表中進行圖表和分組，您可以為每個選擇建立個別欄位（例如，單行文字欄位）。

若要新增選項按鈕和核取方塊：

1. 在畫面的左側，找到下列其中一個欄位，並將其拖曳至畫布上的區段。

   * 單選按鈕
   * 核取方塊群組
   * 下拉

   ![](assets/drag-field-to-section.png)

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
     <td> <p>（必要）輸入描述性標籤，以在自訂欄位上方顯示。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
     <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">姓名</td> 
     <td> <p>（必要）此名稱是當您新增自訂欄位至Workfront的各個區域時（例如報表、首頁和API互動），系統識別該欄位的方法。</p> <p>當您第一次設定自訂欄位並輸入標籤時，會自動填入「名稱」欄位以符合它。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p> 
    <p><b>重要</b>：   
     <ul> 
    <li>雖然可以這樣做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果這樣做，系統將不再識別現在可能在Workfront其他區域參考該欄位的自訂欄位。 <p>例如，如果您新增自訂欄位至報表，之後又變更其名稱，Workfront將無法辨識報表中的自訂欄位，且除非您使用新名稱將其重新新增至報表，否則將無法正常運作。</p> </li>
    <li> <p>建議您不要輸入已用於內建Workfront欄位的名稱。</p> </li>
     <li><p>建議您不要在自訂欄位名稱中使用句號/點字元，以防止在Workfront的不同區域使用欄位時發生錯誤。</p></li>
     </ul> <p>每個自訂欄位名稱在貴組織的Workfront例項中必須是唯一的。 如此一來，您便可重複使用已針對其他自訂表單建立的表單。 如需詳細資訊，請參閱 <a href="#Add" class="MCXref xref">新增自訂欄位至自訂表單</a> 本文章內容。</p> </td>
     <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">指示</td> 
    <td> <p>輸入自訂欄位的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">格式</td> 
    <td> <p>選取將在自訂欄位中擷取的資料型別。</p> <p><b>注意</b>：   
     <ul> 
    <li>表單儲存後即無法編輯此欄位。 如果您要在數學計算中使用欄位，請務必選取「數字」或「貨幣」格式。<br></li> 
    <li>當您選取「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</li>
    <li>數字欄位的字元限製為16。 您也可以使用文字欄位來輸入數字並避免限制。</li>
     </ul></p></td> 
     <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">顯示類型</td> 
    <td>在欄位的選項按鈕、核取方塊群組、下拉式清單或多選下拉式清單之間切換。</td> 
    <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">建立必要欄位</td> 
    <td>如果您希望欄位是使用者完成自訂表單的必要欄位，請選取此選項。 </td> 
    <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">選擇 </td> 
    <td> 
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
    <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至另一個區段，以繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

### 新增預先輸入和日期欄位

您可以將預先輸入和日期欄位新增至自訂表單。

+++ **展開以檢視可用欄位的說明**

* **自動提示**：可讓使用者輸入Workfront中存在的物件名稱。 當使用者開始輸入時，建議清單隨即出現。 此欄位型別支援下列物件：
   * 使用者
   * 群組
   * 職務角色
   * 專案組合
   * 方案
   * 專案
   * 團隊
   * 範本
   * 公司
* **日期欄位**：顯示行事曆，使用者可在其中選取日期和時間。

+++

若要新增預先輸入和日期欄位：

1. 在畫面的左側，找到下列其中一個欄位，並將其拖曳至畫布上的區段。

   * 自動提示
   * 日期欄位

   ![](assets/drag-field-to-section.png)

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
      <td> <p>（必要）輸入描述性標籤，以在自訂欄位上方顯示。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
       <td><ul>
    <li>自動提示</li>
    <li>日期欄位</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是當您新增自訂欄位至Workfront的各個區域時（例如報表、首頁和API互動），系統識別該欄位的方法。</p> <p>當您第一次設定自訂欄位並輸入標籤時，會自動填入「名稱」欄位以符合它。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p> 
      <p><b>重要</b>：   
      <ul> 
      <li>雖然可以這樣做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果這樣做，系統將不再識別現在可能在Workfront其他區域參考該欄位的自訂欄位。 <p>例如，如果您新增自訂欄位至報表，之後又變更其名稱，Workfront將無法辨識報表中的自訂欄位，且除非您使用新名稱將其重新新增至報表，否則將無法正常運作。</p> </li>
      <li> <p>建議您不要輸入已用於內建Workfront欄位的名稱。</p> </li>
      <li><p>建議您不要在自訂欄位名稱中使用句號/點字元，以防止在Workfront的不同區域使用欄位時發生錯誤。</p></li>
      </ul> <p>每個自訂欄位名稱在貴組織的Workfront例項中必須是唯一的。 如此一來，您便可重複使用已針對其他自訂表單建立的表單。 如需詳細資訊，請參閱 <a href="#Add" class="MCXref xref">新增自訂欄位至自訂表單</a> 本文章內容。</p> </td>
         <td><ul>
    <li>自動提示</li>
    <li>日期欄位</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入自訂欄位的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>自動提示</li>
    <li>日期欄位</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">顯示當日時間</td> 
      <td>如果您要在欄位中顯示一天中的時間和日期，請選取此選項。</td> 
         <td><ul>
    <li>日期欄位</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">參考物件類型</td> 
      <td> <p>選取您要與欄位關聯的物件型別。</p> <p>按一下「套用」或「儲存+關閉」後，就無法變更欄位的物件型別。</p> <p><b>注意</b>：   
        <ul> 
         <li>如果您的Workfront管理員在Workfront使用者介面中為「Portfolio」、「程式」或「專案」自訂名稱，此下拉式清單中會顯示物件的預設Workfront名稱，而非自訂名稱。 如果您需要這方面的協助，請洽詢Workfront管理員。<br></li> 
         <li>iOS和Android Workfront Mobile應用程式支援下列物件型別：使用者、公司、群組、工作角色、Portfolio、方案、專案和範本。</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>自動提示</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">新增篩選器</td>
      <td><p>為物件型別新增篩選條件，以限制使用者在使用欄位時可以選擇的物件。 </p> <p>例如，您可以限制欄位，以便只有在使用者符合以下條件時才可選取使用者名稱：</p> 
       <ul> 
        <li>它們屬於您指定的群組</li> 
        <li>它們與您指定的角色或職稱相關聯</li> 
        <li>他們與使用欄位的人屬於同一群組</li> 
       </ul> <p>您必須使用「文字模式」語法來定義所選物件型別的濾鏡。 如需有關使用文字模式建立篩選的資訊，請參閱 <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">使用文字模式編輯篩選器</a>.</p>
       <p><b>注意</b>：
       <ul> 
        <li>如果您正在編輯現有的自訂表單，將篩選條件新增至預先輸入欄位時，不會移除使用者已使用該欄位新增的任何物件（在篩選條件範圍之外）。</li> 
        <li>此篩選器不適用於行動裝置。 如果您針對「預先輸入」欄位使用篩選器，則該欄位將會顯示在不受篩選器影響之使用者的行動裝置上。</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>自動提示</li>
       </ul>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">建立必要欄位</td> 
      <td>如果您希望欄位是使用者完成自訂表單的必要欄位，請選取此選項。 </td> 
       <td><ul>
    <li>自動提示</li>
    <li>日期欄位</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至另一個區段，以繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

### 新增外部查詢欄位

外部查詢欄位會呼叫外部API，並在下拉式欄位中傳回值作為選項。 使用自訂表單附加至之物件的使用者可以從下拉式清單中選取一個或多個選項。 清單和報告中也提供外部查詢欄位。

如需使用外部查詢欄位來呼叫相同Workfront執行個體或公用API的範例，請參閱 [自訂表單中的外部查詢欄位範例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>Document或User物件沒有外部查閱功能。
>
>儀表板目前不支援來自自訂表單的外部查閱欄位。 您無法內嵌編輯欄位值，而且該欄位值在儀表板中可能無法正確顯示。

若要新增外部查詢：

1. 在畫面左側，尋找 **外部查詢** 並將其拖曳至畫布上的區段。
1. 在畫面右側，設定自訂欄位的選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入描述性標籤，以在自訂欄位上方顯示。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別自訂欄位的方式。</p> <p>當您第一次設定自訂欄位並輸入標籤時，會自動填入「名稱」欄位以符合它。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p> 
      <p><b>重要</b>：   
      <ul> 
      <li>雖然可以這樣做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果這樣做，系統將不再識別現在可能在Workfront其他區域參考該欄位的自訂欄位。 <p>例如，如果您新增自訂欄位至報表，之後又變更其名稱，Workfront將無法辨識報表中的自訂欄位，且除非您使用新名稱將其重新新增至報表，否則將無法正常運作。</p> </li>
      <li> <p>建議您不要輸入已用於內建Workfront欄位的名稱。</p> </li>
      <li><p>建議您不要在自訂欄位名稱中使用句號/點字元，以防止在Workfront的不同區域使用欄位時發生錯誤。</p></li>
      </ul> <p>每個自訂欄位名稱在貴組織的Workfront例項中必須是唯一的。 如此一來，您便可重複使用已針對其他自訂表單建立的表單。 如需詳細資訊，請參閱 <a href="#Add" class="MCXref xref">新增自訂欄位至自訂表單</a> 本文章內容。</p> </td>
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
      <td><p>輸入或貼上API的URL。</p><p>API URL必須傳回您要在下拉式清單中顯示的選項JSON內容。 您可以使用JSON路徑欄位，從傳回的JSON中選取特定值作為下拉式選項。</p><p>輸入API URL時，您可以選擇在URL中傳遞下列值：</p>
      <ul>
      <li>$$HOST — 這代表目前的Workfront主機，可用來對Workfront API進行/search API呼叫。 使用此萬用字元時，會處理驗證，使用者不需要傳送驗證標題。 (例如，使用者可以使用基本URL來搜尋任務 <code>$$HOST/attask/api/task/search</code> 而且它允許搜尋任務並從傳回的任務清單中選取值。)</li>
      <li><p>$$QUERY — 這代表一般使用者在欄位中輸入的搜尋文字，可讓您為一般使用者實作查詢篩選。 （使用者會在下拉式清單中搜尋值。）</p>
      <p>如果您參考的API允許，您也可以在搜尋查詢中包含修飾詞，以識別搜尋應該如何運作。 例如，您可以使用下列專案作為基礎API URL，讓人們搜尋包含特定文字的任何Workfront專案： <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>進一步瞭解Workfront搜尋修飾詞於 <a href="/help/quicksilver/wf-api/general/api-basics.md">API基本需知</a>.</p>
      <p><strong>注意：</strong> 如果您未使用$$QUERY，且使用者在搜尋方塊中輸入文字，將會縮小您已擁有的選擇範圍。 但是，如果您使用$$QUERY且使用者鍵入任何內容，則會對您的API執行新的網路呼叫。 因此，如果您的API中有超過2000個值，且API支援查詢，您便可以利用$$QUERY來不僅搜尋現有2000個值，而且搜尋具有縮小選項的原始API。</p></li>
      <li><p>{fieldName}  — 其中fieldName是Workfront中的任何自訂或原生欄位。 這樣，當您將已選取欄位的值傳遞至外部查詢欄位以篩選下拉選項時，您就可以實作階層式下拉選項篩選器。 （例如，「地區」欄位已存在於表單上，而您正在將國家/地區清單從API縮小至特定地區。）</p>
      <p>對於相依於其他欄位的外部查詢欄位(使用 {fieldName} 語法)，從API傳回的選項僅限於符合在其他欄位中輸入的任何字串或值的選項。 （清單和報告不支援此功能。）</p></li>
      <li>{referenceObject}.{fieldName}  — 其中欄位是物件的一部分。 此語法類似於自訂運算式。 (例如，portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>注意：</strong> 檢閱您正在使用的API的檔案，以瞭解您可以定義的特定查詢。</p></td>
     </tr>
     <tr> 
      <td role="rowheader">HTTP 方法</td> 
      <td>選取 <strong>Get</strong>， <strong>Post</strong>，或 <strong>Put</strong> 用於方法。</td> 
     </tr>
     <tr> 
      <td role="rowheader">JSON 路徑</td>
      <td><p>輸入或貼上API的JSON路徑。</p> <p>此選項允許從API URL傳回的JSON擷取資料。 這可當作選取要讓JSON內的哪些值出現在下拉選項中的方式。</p><p>例如，如果您的API URL傳回此格式的JSON：</br>
      <pre>
      { data： { { name： "USA"}， { name： "Canada"} }
      </pre>
      </p>
      <p>然後您可以使用「$.data[*].name」選取美國和加拿大作為下拉式清單選項。</p> <p>如需JSON路徑的相關資訊，以及確保您撰寫正確的JSON路徑，請參閱 <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">標頭</td>
      <td><p>按一下 <strong>新增頁首</strong>，然後輸入或貼上使用API驗證所需的金鑰值組。</p><p><strong>注意：</strong> 標題欄位不是儲存認證的安全位置，您應該注意輸入和儲存的內容。</p></td>
     </tr>
     <tr> 
      <td role="rowheader">多選下拉清單</td>
      <td><p>選取此選項可允許使用者在下拉式清單中選取多個值。</p></td>
     </tr>
     </tr>
     <tr> 
      <td role="rowheader">建立必要欄位</td>
      <td><p>如果您希望欄位是使用者完成自訂表單的必要欄位，請選取此選項。</p></td>
     </tr>       
    </tbody>
   </table>

1. 若要儲存變更，請按一下 **套用** 並移至另一個區段，以繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

>[!NOTE]
>
>以下專案為呼叫外部API的技術限制：
>
>* 選項最大數量： 2000 （只顯示傳回JSON中的前2000個唯一選項）
>* 逾時： 3秒
>* 重試次數： 3
>* 重試之間的等待持續時間：500毫秒
>* 預期的回應狀態： 2xx

### 新增影像、PDF和影片

您可以將影像、PDF和視訊新增至自訂表單。 使用已附加自訂表單的物件的使用者只能在下列區域檢視影像、PDF或影片：

* 物件的「詳細資訊」區域（例如，專案的「詳細資訊」區域）
* 物件的「編輯」方塊(如果它具有新的Adobe Workfront體驗外觀) （例如「編輯專案」和「編輯任務」方塊）

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **展開以檢視可用欄位的說明**

* **影像**：允許使用者新增_____影像檔案。
* **PDF**：允許使用者新增PDF
* **影片**：允許使用者新增____視訊檔案。

+++

若要新增影像、PDF或影片：

1. 在畫面的左側，找到下列其中一個欄位，並將其拖曳至畫布上的區段。

   * 影像
   * PDF
   * 影片

   ![](assets/drag-field-to-section.png)

1. 為Widget輸入或編輯下列任一屬性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要顯示在Widget上方的描述性標籤。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別Widget的方式。</p> <p>當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p> <p><b>重要</b>：雖然可以這樣做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果這樣做，系統將無法再辨識Widget，而此時它可能會在Workfront的其他區域中被參照。 </p> <p>每個Widget名稱在貴組織的Workfront例項中必須是唯一的。 如此一來，您便可重複使用已針對其他自訂表單建立的表單。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必要）輸入或貼上儲存於網際網路之Widget的URL。</p> 
      <p>如果您新增視訊Widget，目前可在URL方塊中新增下列內容來完成此操作：</p> 
      <ul> 
      <li> <p>YouTube或Vimeo連結</p> </li> 
      <li> <p>Google Drive影片連結</p> </li> 
      <li> <p>使用MP4和MOV擴充功能的視訊連結</p> </li> 
      <li> <p>視訊連結已上傳至Workfront執行個體中的檔案區域。 如需指示，請參閱 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">從檔案區域新增視訊Widget至自訂表單</a> 本文章內容。</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關Widget的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>視需要變更Widget的顯示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至另一個區段，以繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

#### 從檔案區域新增視訊Widget至自訂表單{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>以這種方式將視訊新增至自訂表單時，當使用者存取物件上的表單時，只有針對自訂表單設定的許可權會套用至視訊，而不是檔案區域中為視訊設定的許可權。

1. 前往檔案區域中的影片，並為其產生校樣，如中所述 [為網站或其他網頁內容建立互動式校樣](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. 開啟校訂。
1. 以滑鼠右鍵按一下視訊上的任何位置，然後選取「 」 **複製視訊位址**.
1. 在您新增視訊Widget的自訂表單中，將複製的地址貼到 **URL** 方塊。
1. 若要儲存變更，請按一下 **套用** 並移至另一個區段，以繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

<div class="preview">

### 新增Workfront原生欄位

您可以將Workfront原生欄位新增至自訂表單。 當自訂表單附加到物件時，會從物件資料填入欄位。 例如，附加到專案的自訂表單上的說明欄位將提取專案說明。 （如果沒有可用資料，欄位可能會顯示「N/A」。）

+++ **展開以檢視支援的原生欄位清單**

此表格列出自訂表單中特定Workfront物件的可用原生欄位。

| 欄位名稱 | 專案 | 任務 | 問題 | 範本 | 範本任務 | 專案組合 | 方案 | 群組 |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| 實際完成日期 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |   |   |   |
| 實際期間 | ✓ (A) |   |   |   |   |   |   |   |
| 實際時數 | ✓ (A) |   | ✓ (A) |   |   |   |   |   |
| 實際開始日期 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |   |   |   |
| 公司 | ✓ (A) |   |   | ✓ (A) |   |   |   |   |
| 狀況 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |   |   |   |
| 狀況類型 | ✓ (A) |   |   | ✓ (A) |   |   |   |   |
| 說明 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |
| 期間 |   | ✓ (A) |   |   | ✓ (A) |   |   |   |
| 期間類型 |   | ✓ (A) |   |   | ✓ (A) |   |   |   |
| 期間單位 |   | ✓ (A) |   |   | ✓ (A) |   |   |   |
| 輸入者 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |   | ✓ (A) |
| 輸入日期 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |   | ✓ (A) |
| 群組 | ✓ (A) |   |   | ✓ (A) |   | ✓ (A) | ✓ (A) |   |
| 上次更新者 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |   |   |
| 上次更新日期 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |   |   |
| 姓名 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |
| 所有者 | ✓ (A) |   |   | ✓ (A) |   | ✓ (A) | ✓ (A) |   |
| 規劃完成日期 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |   |   |   |
| 計畫持續時間 | ✓ (A) |   |   | ✓ (A) |   |   |   |   |
| 規劃時數 | ✓ (A) | ✓ (A) | ✓ (A) |   | ✓ (A) |   |   |   |
| 規劃開始日期 | ✓ (A) |   |   |   |   |   |   |   |
| 專案組合 | ✓ (A) |   |   | ✓ (A) |   |   | ✓ (A) |   |
| 優先順序 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |   |   |
| 方案 | ✓ (A) |   |   | ✓ (A) |   |   |   |   |
| 預計完成日期 | ✓ (A) | ✓ (A) |   |   |   |   |   |   |
| 預計期間 (分鐘) |   | ✓ (A) |   |   |   |   |   |   |
| 預計開始日期 | ✓ (A) | ✓ (A) |   |   |   |   |   |   |
| 參考號碼 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |   |   |
| 排程模式 | ✓ (A) |   |   | ✓ (A) |   |   |   |   |
| 嚴重程度 |   |   | ✓ (A) |   |   |   |   |   |
| 贊助者 | ✓ (A) |   |   | ✓ (A) |   |   |   |   |
| 狀態 | ✓ (A) | ✓ (A) |   |   |   |   |   |   |
| 腳本點數 |   | ✓ (A) |   |   |   |   |   |   |
| 範本 | ✓ (A) |   |   |   |   |   |   |   |
| URL | ✓ (A) | ✓ (A) |   | ✓ (A) | ✓ (A) |   |   |   |

{style="table-layout:auto"}

+++

1. 在畫面左側，尋找 **原生欄位** 並將其拖曳至畫布上的區段。
1. 在畫面右側，設定自訂欄位的選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入描述性標籤以顯示於欄位上方。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別欄位的方式。</p><p> 當您第一次設定欄位並輸入標籤時，「名稱」欄位會自動填入以和欄位相符。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p>
      <p><b>重要</b>：
      <ul> 
      <li>雖然可以這樣做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果這樣做，系統將不再識別現在可能在Workfront其他區域參考它的欄位。</p> </li>
      <li> <p>每個欄位名稱在貴組織的Workfront例項中必須是唯一的。 如此一來，您便可重複使用已針對其他自訂表單建立的表單。</p> </li>
      <li><p>建議您不要在自訂欄位名稱中使用句號/點字元，以防止在Workfront的不同區域使用欄位時發生錯誤。</p></td> 
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
      <td role="rowheader">大小</td> 
      <td>（可選）視需要變更欄位的顯示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. 若要儲存變更，請按一下 **套用** 並移至另一個區段，以繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

</div>

### 新增Adobe XD檔案

您可以將Adobe XD原型直接新增至自訂表單。 使用自訂表單附加至之物件的使用者只能在下列區域中看到Adobe XD檔案：

* 物件的「詳細資訊」區域（例如，專案的「詳細資訊」區域）
* 物件的「編輯」方塊(如果它具有新的Adobe Workfront體驗外觀) （例如「編輯專案」和「編輯任務」方塊）

新增Adobe XD檔案：

1. 在畫面左側，尋找 **Adobe XD** 並將其拖曳至畫布上的區段。
1. 為Widget輸入或編輯下列任一屬性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要顯示在Widget上方的描述性標籤。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別Widget的方式。 當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p>
    <p><b>重要</b>：   
      <ul> 
      <li>雖然可以這樣做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果這樣做，系統將不再識別現在可能在Workfront其他區域參考該欄位的自訂欄位。 <p>例如，如果您新增自訂欄位至報表，之後又變更其名稱，Workfront將無法辨識報表中的自訂欄位，且除非您使用新名稱將其重新新增至報表，否則將無法正常運作。</p> </li>
      <li> <p>建議您不要輸入已用於內建Workfront欄位的名稱。</p> </li>
      <li><p>建議您不要在自訂欄位名稱中使用句號/點字元，以防止在Workfront的不同區域使用欄位時發生錯誤。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必要）輸入或貼上有效的XD原型連結。</p> 
      <p>注意：在Adobe XD中，共用標籤上的連結存取設定必須設定為具有連結的任何人。 否則，使用者將無法檢視原型。 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關Widget的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（選用）視需要變更Widget的顯示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）重複上一步驟，新增任何其他欄位或Widget。

   或

   若要複製欄位，請將游標移至欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至另一個區段，以繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

## 使用表單設計工具來組織和預覽表單

有關如何組織和檢視表單預覽的資訊，請參閱 [使用表單設計工具來組織和預覽表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
