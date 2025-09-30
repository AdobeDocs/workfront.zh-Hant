---
title: 建立欄位
description: 在Adobe Workfront Planning中，您可以為每種記錄型別建立自訂欄位。 然後，您可以將此欄位與Workfront Planning記錄建立關聯。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 03c1f17504846fc4b8c4114ddc32df687281bc07
workflow-type: tm+mt
source-wordcount: '5332'
ht-degree: 1%

---


<!--Should the structure of this article be like this other one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

<!--Do we need this for FORMULAS: when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula - not sure is needed??-->

# 建立欄位

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

在Adobe Workfront Planning中，您可以建立記錄型別的自訂欄位。 然後，您可以將這些欄位與Workfront Planning記錄建立關聯，以增強記錄資訊。

您必須先建立記錄型別，然後才能建立欄位以與之關聯。 如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

您可以在Workfront Planning中以下列方式建立欄位：

* [從頭開始](#create-fields-from-scratch)
* [透過連線記錄型別](#create-fields-by-connecting-record-types)
* [藉由建立記錄型別](#create-fields-by-creating-a-record-type)
* [從範本建立工作區](#create-fields-by-creating-a-workspace-from-a-template)
* [使用Excel或CSV檔案匯入記錄型別](#create-fields-when-importing-record-types-from-a-csv-or-excel-file)
* [透過匯入現有Workfront欄位的副本](#create-fields-by-importing-them-from-workfront)

如需Workfront Planning欄位的詳細資訊，請參閱[欄位概觀](/help/quicksilver/planning/fields/fields-overview.md)。

## 存取需求

+++ 展開以檢視存取需求。 

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 產品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選擇</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準 </p>
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區與記錄型別</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區。</p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 透過連線記錄型別建立欄位

當您在兩個記錄型別之間新增連線，或記錄型別和其他應用程式的物件型別之間新增連線時，可以建立連結的記錄欄位。

如需有關連線Workfront Planning記錄型別的資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

<!--## Create fields by importing record types using an Excel or CSV file

For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).-->

## 建立記錄型別以建立欄位

建立記錄型別時，依預設也會建立與新記錄型別相關聯的多個欄位。 如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

## 從範本建立工作區以建立欄位

當您從範本建立工作區時，Adobe Workfront Planning會為記錄型別建立欄位。

如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。



## 從CSV或Excel檔案匯入記錄型別時建立欄位

當您使用CSV或Excel檔案匯入記錄型別時，可以匯入欄位。

如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

## 從Workfront匯入欄位，以建立欄位

您可以匯入現有Workfront欄位的復本。

從Workfront匯入欄位會為Workfront Planning記錄型別建立每個欄位的副本。

複製欄位後，這些欄位彼此獨立，不會交換資訊。

如需詳細資訊，請參閱[從Workfront匯入欄位](/help/quicksilver/planning/fields/import-fields-from-workfront.md)。


## 從頭開始建立欄位 {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

<!--the first 3 steps are the same as in Import fields from Workfront-->

{{step1-to-planning}}

1. 按一下您要為其建立欄位記錄的工作區。

   工作區隨即開啟，且記錄型別隨即顯示。

1. 按一下記錄型別的卡片。

   與記錄型別關聯的所有現有記錄都會顯示在表格檢視的列中。

   >[!TIP]
   >
   >    如果沒有顯示記錄，表示您可能還沒有任何記錄，或者您可能套用了篩選器，以限制您在畫面上看到的內容。

   與記錄型別關聯的所有現有欄位都會顯示在表格檢視的欄中。

   >[!TIP]
   >
   >    某些欄位可能已隱藏。 按一下「欄位」並啟用切換您要以表格檢視中的欄位檢視。

1. 按一下表格檢視右上角的&#x200B;**+**&#x200B;圖示

   或

   將游標暫留在任何欄的標頭上，按一下欄位名稱后面的向下箭頭，然後按一下&#x200B;**插入左側**&#x200B;或&#x200B;**插入右側**&#x200B;以新增欄位。
1. 在&#x200B;**新欄位**&#x200B;索引標籤中，搜尋&#x200B;**欄位型別**&#x200B;方塊中的欄位型別，或從下列欄位型別中選取：

   在&#x200B;**新欄位**&#x200B;索引標籤中，使用任何相關關鍵字搜尋&#x200B;**欄位型別**&#x200B;方塊中的欄位型別，或從下列欄位型別中選取。

   >[!TIP]
   >
   >    您可以輸入「預算」，而「編號」與「幣別」的欄位型態會顯示在簡短清單中。



   * [單行文字](#single-line-text)
   * [段落](#paragraph)
   * [多選](#multi-select)
   * [單選](#single-select)
   * [日期](#date)
   * [數字](#number)
   * [百分比](#percentage)
   * [貨幣](#currency)
   * [核取方塊](#checkbox)
   * [公式](#formula)
   * [人員](#people)
   * [建立者](#created-by)
   * [建立日期](#created-date)
   * [上次修改者](#last-modified-by)
   * [上次修改日期](#last-modified-date)
   * <span class="preview">[核准日期](#approved-date)</span>
   * <span class="preview">[核准者](#approved-by)</span>
     <!--* [Object](#object-field-type)-->

   >[!IMPORTANT]
   >
   >儲存欄位後，您無法變更欄位的欄位型別。

   <!--Add this to the IMPORTANT above and make it a NOTE - should do directly to Prod:
    * You can use any keyword that might be related to any of the field type names. For example, a search for "Budget" will display the Number or Currency field type.-->

1. 繼續新增每個欄位，如下節所述。

### 單行文字 {#single-line-text}

單行文字欄位會擷取有限的英數字元資訊。 例如，您可以在單行文字欄位中擷取「擁有者」、「利害關係人」、「團隊」或「組織」單位資訊。 單行文字欄位的內容最多可包含1,000個字元。<!-- used to be 250 but just tested with 1000 and it allowed this as a maximum. -->

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**單行文字**&#x200B;欄位型別。

   ![單行文字欄位型別](assets/single-line-text-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位名稱，它將顯示在資料表或記錄的詳細資訊頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠懸停在表格中的欄位欄標題上，或當您按一下記錄詳細資訊頁面中欄位名稱旁的資訊圖示時，會顯示欄位說明。
1. 按一下「**建立**」。

   新的單行欄位會新增為記錄型別的欄，其值可以與記錄相關聯。


### 段落 {#paragraph}

段落欄位會擷取有關記錄的其他英數字元資訊，類似於「說明」欄位。

>[!TIP]
>
>* 一個記錄型別最多可以有20個段落欄位。
>
>* 段落欄位的內容最多可包含10,000個字元。
>* 當段落欄位顯示在表格檢視或記錄的詳細資訊頁面時，您可以使用RTF格式來增強段落欄位的內容。 如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。
>


1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**段落**&#x200B;欄位型別。

   ![段落欄位型別](assets/paragraph-field-type.png)


1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位名稱，它將顯示在資料表或記錄的詳細資訊頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
1. 按一下「**建立**」。

   新的段落欄位會新增為記錄型別的欄，其值可以與記錄相關聯。


### 多選 {#multi-select}

您可以從下拉式選單中選取多個選項，使用多選欄位來擷取任何格式的其他資訊。

>[!NOTE]
>
><span class="preview">除了本節中說明的功能外，您也可以在表格檢視中編輯記錄的多重選取欄位值時，新增選項。 如需詳細資訊，請參閱文章[編輯記錄](/help/quicksilver/planning/records/edit-records.md).</span>中的「編輯單一或多重選取欄位的資訊」一節
>

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**多重選取**&#x200B;欄位型別。

   ![多重選取欄位型別](assets/multi-select-field-type.png)


1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位名稱，它將顯示在資料表或記錄的詳細資訊頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **選擇**：使用者在更新此欄位時可以選取的選項。 每個選擇的名稱可以同時使用數字和字母。
1. 按一下&#x200B;**新增選擇**&#x200B;以新增更多選擇。 您可以在多重選取欄位中新增多少選擇，沒有限制。
1. （選用）以所需順序手動拖放每個選項，或選取
   如果您希望選擇自動依字母順序列出，請&#x200B;**將選擇A-Z**&#x200B;選項排序。<!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. （選擇性）若要移除選擇，請按一下選擇右側的&#x200B;**x**&#x200B;圖示。
1. 按一下選項左側的色票，即可展開顏色選取器並自訂每個選項的顏色。

1. 按一下&#x200B;**色票**&#x200B;以選取預先定義的顏色

   或

   按一下&#x200B;**自訂**，使用檢色器或十六進位代碼選取自訂顏色。
1. 按一下顏色方塊外部以將其關閉。
1. 按一下「**建立**」。

   新的多重選取欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 單選 {#single-select}

從下拉式功能表中選取一個選項，單選欄位即可擷取任何格式的其他資訊。

>[!NOTE]
>
><span class="preview">除了本節中說明的功能外，您也可以在表格檢視中編輯記錄的單一選取欄位值時新增選項。 如需詳細資訊，請參閱文章[編輯記錄](/help/quicksilver/planning/records/edit-records.md).</span>中的「編輯單一或多重選取欄位的資訊」一節
>


1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**單選**&#x200B;欄位型別。

   ![單一選取欄位型別](assets/single-select-field-type.png)


1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位名稱，它將顯示在資料表或記錄的詳細資訊頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **選擇**：儲存欄位後，可從下拉式功能表中選取的選項。 每個選擇的名稱可以同時使用數字和字母。

1. 按一下&#x200B;**新增選擇**&#x200B;以新增更多選擇。 您可以新增多少選項至單一選取欄位，沒有限制。
1. （選擇性）以所要的順序手動拖放每個選擇，或選取&#x200B;**將選擇排序A-Z**&#x200B;選項（如果您希望選擇自動依字母順序列出）。<!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. （選擇性）若要移除選擇，請按一下選擇右側的&#x200B;**x**&#x200B;圖示。
1. 按一下選項左側的色票，即可展開顏色選取器並自訂每個選項的顏色。
1. 按一下&#x200B;**色票**&#x200B;以選取預先定義的顏色

   或

   按一下&#x200B;**自訂**，使用檢色器或十六進位代碼選取自訂顏色。

1. 按一下顏色方塊外部以將其關閉。
1. 按一下「**建立**」。

   新的單選欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 日期 {#date}

您可以使用日期欄位來擷取日期和時間格式的其他資訊。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**日期**&#x200B;欄位型別。

   ![日期欄位型別](assets/date-field-type.png)


1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **日期格式**：您要在此欄位中顯示的日期格式型別。<!--update this casing - submitted bug for it-->

     從下列格式中選取：
      * **地區**：符合瀏覽器的地區。
      * **標準**： 05/16/2023
      * **長**：2023年5月16日
      * **歐洲**： 16/05/2023
      * **ISO**： 2023-05-16
      * **包含時間**：若要包含時間戳記，請選取此選項。 預設會取消選取此選項。 您不能在保護欄位之後包含時間。

     從下列選項中選取：

      * **24hr**：例如： 18:00
      * **12hr**：例如：下午6:00

1. 按一下「**建立**」。

   新的日期欄位會新增為記錄型別的欄，其值可以與記錄相關聯。

### 數字 {#number}

數字欄位型別會以數字格式擷取資訊。

>[!TIP]
>
>數字欄位會在請求表單產生器中顯示為「單行」文字欄位型別。
>
>但是，欄位格式會保留，並且這些欄位的值將在提交請求後、在記錄型別和請求詳細資訊頁面中顯示為數字。
>&#x200B;>如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。


1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**數字**&#x200B;欄位型別。

   ![數字欄位型別](assets/number-field-type.png)
1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **精確度**：您要為欄位記錄的小數位數。 您最多可以顯示6個小數位數。
   * **允許負數**：如果您要在此欄位中允許負數，請選取此選項。 預設會取消選取此選項。

   >[!NOTE]
   >
   >    如果您選取「允許負數」，且負值儲存在附加欄位的記錄上，則以後無法再取消選取設定。

1. 按一下「**建立**」。

   新數字欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 百分比 {#percentage}

百分比欄位型別會以數字格式擷取資訊，後面接著百分比符號。

>[!TIP]
>
>百分比欄位在請求表單產生器中顯示為單行文字欄位型別。
>
>但是，欄位格式會保留，並且這些欄位的值將在提交請求後，在記錄型別和請求詳細資訊頁面中顯示為百分比。
>&#x200B;>如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。


1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**百分比**&#x200B;欄位型別。

   ![百分比欄位型別](assets/percentage-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **精確度**：您要為欄位記錄的小數位數。 您最多可以顯示6個小數位數。
   * **允許負數**：若要允許此欄位中有負百分比值，請選取此選項。 預設會取消選取此選項。

     >[!NOTE]
     >
     >如果您選取「允許負數」，且負值儲存在附加欄位的記錄上，則以後無法再取消選取設定。

   * **顯示為**：從下拉式功能表，選擇百分比值在表格檢視中的顯示方式。 從下列選項中選取：
      * **數字**：百分比值顯示為後面跟著百分比符號的數字。
      * **列**：百分比值會在百分比數字旁顯示成列。 長條的填色顏色表示百分比值。 這是預設選取範圍。
      * **圓形**：百分比值在百分比數字旁邊顯示為圓形的外框。 圓形外框的填色顏色表示百分比值。

   >[!NOTE]
   >
   >* 您在「顯示為」欄位中所做的選擇僅適用於表格檢視中顯示的百分比值。 在Workfront Planning中，欄位百分比值會顯示為一個數字，後面跟著其他位置的百分比符號。 當百分比型別欄位在其他記錄的表格檢視中顯示為查閱欄位時，此也會套用至該欄位。
   >* 您稍後編輯欄位時，可以變更「顯示為選取專案」。

1. 按一下「**建立**」。

   新的百分比欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 貨幣 {#currency}

貨幣欄位型別會以數字格式擷取資訊，前面加貨幣符號。

>[!TIP]
>
>貨幣欄位在請求表單產生器中顯示為單行文字欄位型別。
>
>但是，欄位格式會保留，並且這些欄位的值將在提交請求後，在記錄型別和請求詳細資訊頁面中顯示為貨幣。
>&#x200B;>如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**貨幣**&#x200B;欄位型別。

   ![貨幣欄位型別](assets/currency-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **貨幣**：您要在此欄位中顯示的貨幣型別。 這是一份國際標準化組織(ISO)的貨幣清單。
   * **精確度**：您要為欄位記錄的小數位數。 您最多可以顯示6個小數。
   * **允許負數**：如果您要允許此欄位中有負貨幣值，請選取此選項。 預設會取消選取此選項。

   >[!NOTE]
   >
   >    如果您選取「允許負數」，且負值儲存在附加欄位的記錄上，則以後無法再取消選取設定。

1. 按一下「**建立**」。

   新的貨幣欄位會新增為記錄型別的欄，其值可以與記錄相關聯。

### 核取方塊

您可以使用核取方塊欄位型別，將單一核取方塊選項新增至記錄。 您可以使用此欄位來指示該特定記錄的特定屬性或狀態。 例如，您可以將其用作追蹤完成、核准或每個記錄的任何其他二進位屬性的標幟。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**核取方塊**&#x200B;欄位型別。

   ![核取方塊欄位型別](assets/checkbox-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
1. 按一下「**建立**」。

   新的核取方塊欄位會新增為記錄型別的欄，其值可以與記錄相關聯。

### 公式

公式欄位會使用記錄型別中其他欄位的現有值，以及指示應如何計算現有值的函式，來產生新值。

如需詳細資訊，請參閱[公式欄位概述](/help/quicksilver/planning/fields/formula-fields.md)。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**公式**&#x200B;欄位型別。

   ![新的公式欄位，包含運算式清單](assets/new-formula-field-with-list-of-expressions.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：輸入新欄位的名稱。
   * **描述**：新增有關新欄位的資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **公式**：開始輸入至少一個字元以存取運算式，然後在運算式顯示在清單中時選取它。

1. 按一下選取的運算式以顯示定義並檢視其格式。

   ![公式運算式的描述](assets/description-of-formula-expression.png)

   如需支援哪些運算式的詳細資訊，請參閱[公式欄位概觀](/help/quicksilver/planning/fields/formula-fields.md)。


   >[!TIP]
   >
   >編輯或建立公式欄位時，您會收到警告訊息，此訊息可能會造成對本身或共用欄位的循環參照。 您無法儲存參照本身或參照計算中所參照專案的公式欄位。


1. 新增在Workfront Planning中顯示的欄位名稱，以在公式中參照它們。

   >[!NOTE]
   >
   >* 您無法在公式中新增多重選取型別欄位。
   >
   >
   >* 您必須在Workfront Planning中拼出公式中所包含欄位的名稱。 Workfront Planning公式不支援Workfront文字模式語法和萬用字元。
   >
   >* 您可以參照與目前記錄型別相距最多4個欄位（和物件）的欄位。 例如，如果您正在建立「活動」記錄型別(1)的公式欄位，且「活動」已連線至「促銷活動」記錄型別(2)，而該記錄型別已連線至「Workfront專案」(3)，則您可以在針對「活動」記錄型別建立的公式中，參考專案的「預算」欄位(4)。
   >
   >![公式範例專案預算四個欄位已移除](assets/formula-example-project-budget-four-fields-removed.png)
   >

1. （選擇性）按一下&#x200B;**最大化**，在較大的區域中開啟[公式]方塊。

   「公式」方塊會在較大的視窗中開啟。
1. （選擇性和條件式）如果您在較大的區域中開啟公式方塊，請按一下&#x200B;**最小化**&#x200B;以返回原始公式欄位方塊。

1. 在&#x200B;**格式**&#x200B;欄位中，從下列選項中選取，以識別公式型別欄位中顯示結果的格式：

   * **文字**：公式欄位的結果顯示為純文字。
   * **數字**：公式欄位的結果顯示為數字。
   * **百分比**：公式欄位的結果顯示為後面跟著百分比符號的數字。
   * **貨幣**：公式欄位的結果顯示為前面或後面跟著貨幣符號的數字。
   * **標籤**：公式欄位的結果會以標籤與物件名稱一起顯示。

     >[!TIP]
     >
     >我們建議將標籤用於顯示陣列的欄位。 在這種情況下，每個陣列成員都會顯示為個別標籤。

     ![公式欄位格式清單，標籤已選取反白顯示](assets/formula-field-formats-list-with-tag-selected-highlighted.png)

   * **日期**：公式欄位的結果顯示為日期。

     結果預覽會顯示在&#x200B;**格式**&#x200B;欄位下。

     >[!WARNING]
     >
     >如果公式的結果不符合所選的格式，則欄位將顯示錯誤訊息。

1. 按一下「**建立**」。

   新的公式欄位會新增為記錄型別的欄，其值可以與記錄相關聯。

### 人員

您可以使用[人員]欄位型別將使用者<!--, job role, or team-->新增到記錄。 這是預先輸入欄位，您只能新增已在Workfront執行個體中的使用者<!--, roles, or teams-->。

>[!TIP]
>
>* 當您在「人員」欄位中新增使用者名稱時，使用者名稱及其主要工作角色會顯示在該欄位中。
>
>* 在請求表單產生器中，人物欄位會顯示為參考（或連線）欄位型別。
>
>如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**人員**&#x200B;欄位型別。

   ![人員欄位型別](assets/people-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **允許多個值**：如果您要允許使用者在此欄位中新增一個以上的使用者，請選取此選項。 預設會取消選取此選項。

   >[!NOTE]
   >
   >    如果您選取「允許多個值」，且有多個使用者儲存在附加欄位的記錄中，則以後編輯此欄位時，無法再取消選取設定。

1. 按一下「**建立**」。

   新的「人員型別」欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 建立者

您可以使用「建立者」欄位型別，將建立記錄的使用者新增至記錄。 這是唯讀欄位，會自動填入建立記錄時登入的使用者名稱。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**建立者**&#x200B;欄位型別。

   ![由欄位型別](assets/created-by-field-type.png)建立

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。<!--this might change and they might prepopulate it with "Created by"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。

1. 按一下「**建立**」。

   新的「建立者型別」欄位會新增為記錄型別的欄，其值會預先填入建立每個記錄的使用者名稱。


### 建立日期

您可以使用「建立日期」欄位型別，將記錄的建立日期新增至記錄。 這是唯讀欄位，會自動填入建立記錄的日期（以及可選的時間）。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**建立日期**&#x200B;欄位型別。

   ![已建立日期欄位型別](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。<!--this might change and they might prepopulate it with "Created date"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **日期格式**：從下列格式選取：

      * **地區**：符合瀏覽器的地區。
      * **標準**： 05/16/2023
      * **長**：2023年5月16日
      * **歐洲**： 16/05/2023
      * **ISO**： 2023-05-16
   * **包含時間欄位**：若要包含時間戳記，請選取此選項。 預設會取消選取此選項。<!--submitted a UI text change for this - check the UI-->

     從下列選項中選取：

      * **24hr**：例如： 18:00
      * **12hr**：例如：下午6:00

1. 按一下「**建立**」。

   新的「建立日期 — 型別」欄位會新增為記錄型別的欄，其值會預先填入建立記錄的日期（或日期和時間）。


### 上次修改者

您可以使用「上次修改者」欄位型別，將上次修改紀錄的使用者新增至記錄。 這是唯讀欄位，會自動填入上次更新記錄時登入的使用者名稱。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**上次修改者**&#x200B;欄位型別。

   ![上次修改者欄位型別](assets/last-modified-by-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。<!--this might change and they might prepopulate it with "Created by"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。

1. 按一下「**建立**」。

   新的「上次修改者」型別欄位會新增為記錄型別的欄，其值會預先填入上次修改每筆記錄的使用者名稱。


### 上次修改日期

您可以使用「上次修改日期」欄位型別來新增上次將記錄修改至記錄的日期。 這是唯讀欄位，會自動填入上次修改記錄的日期（以及可選的時間）。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**建立日期**&#x200B;欄位型別。

   ![上次修改日期欄位型別](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。<!--this might change and they might prepopulate it with "Created date"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **日期格式**：從下列格式選取：

      * **地區**：符合瀏覽器的地區。
      * **標準**： 05/16/2023
      * **長**：2023年5月16日
      * **歐洲**： 16/05/2023
      * **ISO**： 2023-05-16

   * **包含時間欄位**：若要包含時間戳記，請選取此選項。 預設會取消選取此選項。<!--submitted a UI text change for this - check the UI-->

     從下列選項中選取：

      * **24hr**：例如： 18:00
      * **12hr**：例如：下午6:00

1. 按一下「**建立**」。

   新的上次修改日期型別欄位會新增為記錄型別的欄，其值會預先填入上次修改記錄的日期（或日期和時間）。

<div class="preview">

### 核准日期

您可以使用核准日期欄位型別來新增核准請求並導致建立記錄的日期。 此為唯讀欄位，當最後核准者的請求獲得核準時，會自動填入日期（以及可選的時間）。 在此情況下，核准日期應該與記錄的建立日期一致。

>[!TIP]
>
>「核准日期」欄位只會針對提交與核准者關聯的請求表單所建立的記錄，填入資訊。
>
>如果表單與多個核准者相關聯，則在「核准日期」欄位中僅記錄最後核准決定的日期。


1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**建立日期**&#x200B;欄位型別。

   ![核准的日期欄位型別](assets/approved-date-field-type.png)

   1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。
   * **日期格式**：從下列格式選取：

      * **地區**：符合瀏覽器的地區。
      * **標準**： 05/16/2023
      * **長**：2023年5月16日
      * **歐洲**： 16/05/2023
      * **ISO**： 2023-05-16

   * **包含時間欄位**：若要包含時間戳記，請選取此選項。 預設會取消選取此選項。

     從下列選項中選取：

      * **24hr**：例如： 18:00
      * **12hr**：例如：下午6:00

1. 按一下「**建立**」。

   新的「已核准的日期型別」欄位會新增為記錄型別的欄，如果記錄是由提交與核准者關聯的請求所建立，其值會預先填入記錄請求核准的日期（或日期和時間）。

### 核准者

您可以使用「核准者」欄位型別來新增上次核准請求的使用者，以建立記錄。 這是唯讀欄位，會自動填入核准建立記錄請求的使用者名稱。

>[!TIP]
>
>「核准者」欄位只會針對提交與核准者關聯的請求表單所建立的記錄，填入資訊。
>
>如果表單與多個核准者相關聯，則所有核准者的名稱都會記錄在「核准日期」欄位中，並以逗號分隔。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**核准者**&#x200B;欄位型別。

   ![由欄位型別](assets/approved-by-field-type.png)核准

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位名稱，它將顯示在資料表或記錄頁面中。
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上，或當您在記錄的詳細資訊頁面中按一下欄位名稱旁的資訊圖示時，會顯示欄位說明。

1. 按一下「**建立**」。

   新的「已核准的副檔型別」欄位會新增為記錄型別的欄，其值會預先填入上次修改每筆記錄的使用者名稱。

</div>

<!--

## Object field type

You can use the Object field type when you need to store several fields that might include several pieces of information. For example, you can store the source, code, error message, or details of an object in one field. In this case, instead of having several separate single-line text fields for that, you can use an Object field to store all information in one place. 

For example, when using an Object-type field, you can store the following type of information: 

```
"{
""source"": ""string"",
""code"": ""string"",
""subCode"": ""string"",
""message"": ""string"",
""details"": ""string""
}"

```

You can also store an array of values in one field and you would rather rely on user input for each element of the array, instead of using a multi-select field type for the same purpose. For example, you can store information in the following format: 

`["EMEA", "APAC"] `

Consider the following when using Object-type fields:

* In addition to strings and arrays, you can store other value formats like HTML.
* There is no format validation for this field. 
* Object-type fields have a limit of 10,000 characters.

Create an Object field: 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Created date** field type.

    ![Object field type](assets/object-field-type.png)

1. Add the following information in the **New field** tab:

     * **Name**: The name of the field, as it will appear in a table or the record page. (***********this might change and they might prepopulate it with "Created date"********)
     * **Description**: Additional information about the field. The description of a field displays when you hover over the field's column in a table, or when you click the information icon next to the field name in the record's details page.

1. Click **Create**.

    The new Object-type field is added as a column to the record type.

-->




