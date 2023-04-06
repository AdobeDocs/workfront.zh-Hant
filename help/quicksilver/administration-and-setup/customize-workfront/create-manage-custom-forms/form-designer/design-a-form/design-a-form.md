---
title: 使用表單設計工具設計表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表單設計器來設計自訂表單。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 使用表單設計工具設計表單

您可以使用表單設計器來設計自訂表單。 您可以將自訂表單附加至不同的Workfront物件，以擷取這些物件的相關資料。

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
   <td>
   <p>當前計畫：標準</p>
   <p>或</p>
   <p>舊計畫：計畫</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 開始設計自訂表單

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms** 中。

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. 按一下 **新自訂表單。**
1. 選取您要將自訂表單附加至哪些物件類型，然後按一下 **繼續**.

   ![](assets/choose-object-type.jpg)

1. 在 **需要標題** 區域，鍵入自定義表單標題。
1. （可選）如果要將更多對象類型添加到窗體中，以便它可以附加到更多對象，請按一下 **新增** 圖示 ![](assets/add-objects-icon.png) after **物件類型**，然後在顯示的功能表中選取您要的類型。 您可以重複此操作，以新增任意數量的物件類型。

   您也可以按一下物件類型上的X，將其從表單中刪除。

   >[!CAUTION]
   >
   >刪除自訂表單也會刪除與表單關聯之物件上的所有自訂資料。 已刪除的資料無法恢復。 請考慮停用自訂表單 — 停用您不再使用的自訂表單時，您會保留所有相關的歷史資料。
   >
   >如需詳細資訊，請參閱 [刪除自訂表單上的物件類型](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).


1. 接下來，您可以開始將欄位新增至自訂表單。 請參閱下列章節：
   * [重複使用已在其他自定義表單中使用的現有欄位或介面工具集](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [新增文字欄位](#add-text-fields)
   * [新增計算欄位](#add-calculated-fields)
   * [新增選項按鈕、核取方塊群組和下拉式清單](#add-radio-buttons-checkboxes-and-dropdowns)
   * [新增提前類型和日期欄位](#add-typeahead-and-date-fields)
   * [新增影像、PDF和影片](#add-images-pdfs-and-videos)
   * [新增Adobe XD檔案](#add-adobe-xd-files)

## 新增或現有欄位至自訂表單

設計自訂表單時，您可以使用新欄位或現有欄位。

## 重複使用已在其他自定義表單中使用的現有欄位或介面工具集

1. 在畫面左上方，按一下 **欄位程式庫**.

1. 將欄位或介面工具集拖曳至您要的自訂表單中。
1. （可選）重複上一步以新增任何其他欄位或小工具。

   >[!NOTE]
   >
   >在單一自訂表單中，最多可新增500個欄位和Widget。 但是，當表單上存在超過100個時，效能可能會降低，具體取決於表單的複雜性。
   >
   >
   >複雜表單的範例包括具有階層式參數的表單、計算的自訂資料欄位，以及單一欄位中的多個值選項。

1. 若要儲存變更，請按一下 **套用** 並移至其他區段，繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

### 新增文字欄位

您可以將數個不同的文字欄位新增至自訂表單。

+++ **展開以查看可用文本欄位的說明**

* **單行文本欄位**:可讓使用者在欄位中輸入單行文字。
* **段落文本欄位**:可讓使用者在欄位中輸入多行文字。
* **具有格式的文本欄位**:允許用戶在欄位中鍵入多行文本，並使用粗體、斜體、下划線、項目符號、編號、超連結和塊引號來格式化文本。 字元限制為15,000，可容納大量文字和格式。

   如需透過API存取此欄位的相關資訊，請參閱API中的RTF欄位儲存。

   >[!NOTE]
   >
   >Workfront行動應用程式無法使用格式化的文字欄位（未來版本提供）。

* **描述性文字**:可讓您加入指示並連結至Workfront以外的頁面。

+++

若要新增文字欄位：

1. 在畫面左側，尋找下列其中一個文字欄位，並將其拖曳至畫布上的區段：

   * 單行文本：
   * 段落文字
   * 具有格式的文本欄位
   * 描述文字

   ![](assets/drag-field-to-section.png)

1. 在畫面右側，設定您所新增之自訂欄位類型可用的選項：

   <table>
    <tr>
    <td>輸入</td>
    <td>說明</td>
    <td>適用於 </td>
    </tr>
    <tr>
    <td>大小</td>
    <td><p>更改表單上文本欄位的大小。<p>
   </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    <li>含格式的文字</li>
    <li>描述性文字 — 即將推出</li>
    </ul></td>
    </tr>
    <tr>
    <td>標籤</td>
    <td><p>輸入要在介面工具集上方顯示的描述性標籤。 您隨時都可以變更標籤。<p>
    <p>重要：請避免在此標籤中使用特殊字元。 報表中無法正確顯示。</p></td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    <li>含格式的文字</li>
    </ul></td>
    </tr>
    <tr>
     <td>名稱</td>
    <td><p>（必要）此名稱是系統識別欄位的方式。 當您第一次設定介面工具集並輸入標籤時，「名稱」欄位會自動填入以符合標籤。 但「標籤」和「名稱」欄位未同步，因此您可以自由地更改用戶看到的標籤，而不必更改系統看到的名稱。</p>
    <p><b>重要</b>:   
      <ul> 
      <li>雖然可以這麼做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果您這麼做，系統將不再識別自訂欄位，現在可能會在Workfront的其他區域參照該欄位。 <p>例如，如果您將自訂欄位新增至報表，之後又變更其名稱，Workfront在報表中將無法辨識該欄位，除非您使用新名稱將其重新新增至報表，否則該欄位將停止正常運作。</p> </li>
      <li> <p>建議您不要輸入已用於內建Workfront欄位的名稱。</p> </li>
      <li><p>建議您不要在自訂欄位名稱中使用句點/點字元，以防止在Workfront不同區域使用欄位時發生錯誤。</p></li>
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
    <td>輸入有關介面工具集的任何其他資訊。 當使用者填寫自訂表單時，可將滑鼠移至問號圖示上方，檢視包含您在此輸入之資訊的工具提示。
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
    <td><p>選取要在自訂欄位中擷取的資料類型。</p> <p><b>附註</b>:   
    <ul> 
    <li>表單儲存後無法編輯此欄位。 如果要在數學計算中使用欄位，請確保選擇數字或貨幣格式。<br></li> 
    <li>選擇「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</li> 
     </ul></p></td> </td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    </ul></td>
    </tr>
    <tr>
    <td>顯示類型</td>
    <td>在單行和段落文本欄位之間切換。</td>
    <td><ul>
    <li>單行文字</li>
    <li>段落文字</li>
    </ul></td>
    </tr>
    <tr>
    <td>超連結</td>
    <td> 如果要將超連結應用到已鍵入的描述性文本，請在此處添加它。 描述性文字會顯示為附加表單之物件的連結。</td>
    <td><ul><li>描述文字</li></ul></td>
    </tr>
   </table>

1. （可選）重複上一步以新增任何其他欄位或小工具。

   或

   若要複製欄位，請將滑鼠指標暫留在欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至其他區段，繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

### 新增計算欄位

在自訂表單中，您可以在自訂表單附加至物件時，新增使用現有資料產生新資料的計算自訂欄位。

若要新增計算欄位，請參閱 [使用表單設計器添加計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### 新增選項按鈕、核取方塊和下拉式清單

您可以將選項按鈕、核取方塊和下拉式清單新增至自訂表單。

+++ **展開以查看可用欄位的說明**

* **選項按鈕**:僅要求使用者選取一個選項。
* **核取方塊群組**:允許用戶選擇多個選項。
* **下拉式清單**:提供下拉式選項清單。

+++

添加單選按鈕和複選框：

1. 在畫面左側，尋找下列其中一個欄位，並將其拖曳至畫布上的區段。

   * 單選按鈕
   * 核取方塊群組
   * 下拉

   ![](assets/drag-field-to-section.png)

1. 在畫面右側，設定您所新增之自訂欄位類型可用的選項：

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>輸入</td>
    <td>說明</td>
    <td>適用於 </td>
    </tr>
    <tr> 
     <td role="rowheader">標籤</td> 
     <td> <p>（必要）輸入要在自訂欄位上方顯示的描述性標籤。 您隨時都可以變更標籤。</p> <p><b>重要</b>:請避免在此標籤中使用特殊字元。 報表中無法正確顯示。</p> </td> 
     <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
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
     <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">指示</td> 
    <td> <p>輸入有關自訂欄位的任何其他資訊。 當使用者填寫自訂表單時，可將滑鼠移至問號圖示上方，檢視包含您在此輸入之資訊的工具提示。</p> 
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
    <td> <p>選取要在自訂欄位中擷取的資料類型。</p> <p><b>附註</b>:   
     <ul> 
    <li>表單儲存後無法編輯此欄位。 如果要在數學計算中使用欄位，請確保選擇數字或貨幣格式。<br></li> 
    <li>選擇「數字」或「貨幣」時，系統會自動截斷以0開頭的數字。</li> 
     </ul></p></td> 
     <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">顯示類型</td> 
    <td>在欄位的選項按鈕、核取方塊群組或下拉式清單之間切換。</td> 
    <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">建立必要欄位</td> 
    <td>如果您希望欄位為必要欄位，讓使用者完成自訂表單，請選取此選項。 </td> 
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
    <td><ul>
    <li>單選按鈕</li>
    <li>核取方塊群組</li>
    <li>下拉</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. （可選）重複上一步以新增任何其他欄位或小工具。

   或

   若要複製欄位，請將滑鼠指標暫留在欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至其他區段，繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

### 新增提前類型和日期欄位

您可以在自訂表單中新增提前類型和日期欄位。

+++ **展開以查看可用欄位的說明**

* **Typeahead**:可讓使用者輸入Workfront中存在之物件的名稱。 當使用者開始輸入時，會顯示建議清單。 此欄位類型支援下列物件：
   * 使用者
   * 群組
   * 職務角色
   * 專案組合
   * 方案
   * 專案
   * 團隊
   * 範本
   * 公司
* **日期欄位**:顯示日曆，使用者可在其中選取日期和時間。

+++

若要新增預先輸入日期欄位：

1. 在畫面左側，尋找下列其中一個欄位，並將其拖曳至畫布上的區段。

   * 自動提示
   * 日期欄位

   ![](assets/drag-field-to-section.png)

1. 在畫面右側，設定您所新增之自訂欄位類型可用的選項：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>欄位設定</td>
    <td>說明</td>
    <td>適用於 </td>
    </tr>
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要在自訂欄位上方顯示的描述性標籤。 您隨時都可以變更標籤。</p> <p><b>重要</b>:請避免在此標籤中使用特殊字元。 報表中無法正確顯示。</p> </td> 
       <td><ul>
    <li>自動提示</li>
    <li>日期欄位</li>
    </ul></td>
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
         <td><ul>
    <li>自動提示</li>
    <li>日期欄位</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關自訂欄位的任何其他資訊。 當使用者填寫自訂表單時，可將滑鼠移至問號圖示上方，檢視包含您在此輸入之資訊的工具提示。</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>自動提示</li>
    <li>日期欄位</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">顯示當日時間</td> 
      <td>如果您想在欄位中顯示一天中的時間以及日期，請選取此選項。</td> 
         <td><ul>
    <li>日期欄位</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">參考物件類型</td> 
      <td> <p>選擇要與欄位關聯的對象類型。</p> <p>按一下「應用」或「保存並關閉」後，就無法更改欄位的對象類型。</p> <p><b>附註</b>:   
        <ul> 
         <li>如果您的Workfront管理員在Workfront使用者介面中自訂了Portfolio、方案或專案的名稱，物件的預設Workfront名稱會顯示在此下拉式清單中，而非自訂名稱。 如需相關協助，請洽詢Workfront管理員。<br></li> 
         <li>iOS和Android Workfront行動應用程式支援下列物件類型：用戶、公司、組、職務、Portfolio、方案、項目和模板。</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>自動提示</li>
    </ul></td>
     </tr>
     <tr> 
      <td role="rowheader">建立必要欄位</td> 
      <td>如果您希望欄位為必要欄位，讓使用者完成自訂表單，請選取此選項。 </td> 
       <td><ul>
    <li>自動提示</li>
    <li>日期欄位</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. （可選）重複上一步以新增任何其他欄位或小工具。

   或

   若要複製欄位，請將滑鼠指標暫留在欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至其他區段，繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

### 新增影像、PDF和影片

您可以將影像、PDF和影片新增至自訂表單。 使用自訂表單所附加之物件的使用者，只能在下列區域看到影像、PDF或影片：

* 對象的「詳細資訊」區域（例如，對於項目，為「項目詳細資訊」區域）
* 物件的「編輯」方塊(如果具有新的Adobe Workfront體驗外觀)（例如「編輯專案」和「編輯工作」方塊）

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **展開以查看可用欄位的說明**

* **影像**:允許用戶添_____影像檔案。
* **PDF**:允許使用者新增PDF
* **影片**:允許用戶添____視頻檔案。

+++

若要新增影像、PDF或影片：

1. 在畫面左側，尋找下列其中一個欄位，並將其拖曳至畫布上的區段。

   * 影像
   * PDF
   * 視訊

   ![](assets/drag-field-to-section.png)

1. 為介面工具集鍵入或編輯以下任何屬性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要在介面工具集上方顯示的描述性標籤。 您隨時都可以變更標籤。</p> <p><b>重要</b>:請避免在此標籤中使用特殊字元。 報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td> <p>（必要）此名稱是系統識別介面工具集的方式。</p> <p>當您第一次設定介面工具集並輸入標籤時，「名稱」欄位會自動填入以符合標籤。 但「標籤」和「名稱」欄位未同步，因此您可以自由地更改用戶看到的標籤，而不必更改系統看到的名稱。</p> <p><b>重要</b>:雖然可以這麼做，但建議您不要在您或其他使用者開始使用Widget中的自訂表單後變更此名稱。 如果您這麼做，系統將不再識別介面工具集，現在可能會在Workfront的其他區域參照該介面工具集。 </p> <p>在貴組織的Workfront例項中，每個介面工具集名稱必須是唯一的。 這樣，您就可以重複使用已針對其他自訂表單建立的表單。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必要）輸入或貼上Widget的URL，該URL儲存在網際網路上。</p> 
      <p>如果您新增視訊介面工具集，目前可在URL方塊中新增下列內容，以完成新增：</p> 
      <ul> 
      <li> <p>YouTube或Vimeo連結</p> </li> 
      <li> <p>Google驅動器視頻連結</p> </li> 
      <li> <p>連結至MP4和MOV擴充功能的影片</p> </li> 
      <li> <p>連結至已上傳至Workfront執行個體中「檔案」區域的影片。 如需指示，請參閱 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">從「文檔」區域將視頻介面工具集添加到自定義表單中</a> 這篇文章。</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關介面工具集的任何其他資訊。 當使用者填寫自訂表單時，可將滑鼠移至問號圖示上方，檢視包含您在此輸入之資訊的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>視需要變更介面工具集的顯示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）重複上一步以新增任何其他欄位或小工具。

   或

   若要複製欄位，請將滑鼠指標暫留在欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至其他區段，繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

#### **從「文檔」區域將視頻介面工具集添加到自定義表單中**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>以這種方式將視訊新增至自訂表單時，當使用者存取物件上的表單時，只有為自訂表單設定的權限才會套用至視訊，而非在「檔案」區域為視訊設定的權限。

1. 前往「檔案」區域中的影片，並產生校樣，如 [為網站或其他網路內容建立互動式校樣](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. 開啟校樣。
1. 以滑鼠右鍵按一下視訊的任一位置，然後選取 **複製視訊地址**.
1. 在您新增視訊介面工具集的自訂表單中，將複製的位址貼入 **URL** 框。
1. 若要儲存變更，請按一下 **套用** 並移至其他區段，繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

### 新增Adobe XD檔案

您可以直接將Adobe XD原型新增至自訂表單。 使用自訂表單所附加之物件的使用者，只能在下列區域看到Adobe XD檔案：

* 對象的「詳細資訊」區域（例如，對於項目，為「項目詳細資訊」區域）
* 物件的「編輯」方塊(如果具有新的Adobe Workfront體驗外觀)（例如「編輯專案」和「編輯工作」方塊）

新增Adobe XD檔案：

1. 在畫面左側，尋找 **Adobe XD** 並拖曳至畫布上的區段。
1. 為介面工具集鍵入或編輯以下任何屬性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要在介面工具集上方顯示的描述性標籤。 您隨時都可以變更標籤。</p> <p><b>重要</b>:請避免在此標籤中使用特殊字元。 報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td> <p>（必要）此名稱是系統識別介面工具集的方式。 當您第一次設定介面工具集並輸入標籤時，「名稱」欄位會自動填入以符合標籤。 但「標籤」和「名稱」欄位未同步，因此您可以自由地更改用戶看到的標籤，而不必更改系統看到的名稱。</p>
    <p><b>重要</b>:   
      <ul> 
      <li>雖然可以這麼做，但建議您不要在您或其他使用者開始使用Workfront中的自訂表單後變更此名稱。 如果您這麼做，系統將不再識別自訂欄位，現在可能會在Workfront的其他區域參照該欄位。 <p>例如，如果您將自訂欄位新增至報表，之後又變更其名稱，Workfront在報表中將無法辨識該欄位，除非您使用新名稱將其重新新增至報表，否則該欄位將停止正常運作。</p> </li>
      <li> <p>建議您不要輸入已用於內建Workfront欄位的名稱。</p> </li>
      <li><p>建議您不要在自訂欄位名稱中使用句點/點字元，以防止在Workfront不同區域使用欄位時發生錯誤。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必要）輸入或貼上有效的XD原型連結。</p> 
      <p>注意：Adobe XD中「共用」標籤上的「連結存取」設定必須設為「具有連結的任何人」。 否則，使用者將無法檢視原型。 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關介面工具集的任何其他資訊。 當使用者填寫自訂表單時，可將滑鼠移至問號圖示上方，檢視包含您在此輸入之資訊的工具提示。
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（可選）視需要變更介面工具集的顯示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）重複上一步以新增任何其他欄位或小工具。

   或

   若要複製欄位，請將滑鼠指標暫留在欄位上，然後按一下復製圖示。

   ![復製圖示](assets/copy-field.png)

1. 若要儲存變更，請按一下 **套用** 並移至其他區段，繼續建立您的表單。

   或

   按一下 **儲存並關閉**.

## 使用表單設計工具組織和預覽表單

有關如何組織和查看表單預覽的資訊，請參閱 [使用表單設計工具組織和預覽表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).