---
title: 建立欄位
description: 在Adobe Workfront Planning中，您可以為每種記錄型別建立自訂欄位。 然後，您可以將此欄位與Workfront Planning記錄建立關聯。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '3620'
ht-degree: 2%

---


<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

<!--Do we need this for FORMULAS: when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula - not sure is needed??-->

# 建立欄位

{{planning-important-intro}}

在Adobe Workfront Planning中，您可以建立記錄型別的自訂欄位。 然後，您可以將這些欄位與Workfront Planning記錄建立關聯，以增強記錄資訊。

您必須先建立記錄型別，然後才能建立欄位以與之關聯。 如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

您可以在Workfront Planning中以下列方式建立欄位：

* 從頭開始
* 透過連線記錄型別
* 藉由建立記錄型別
* 從範本建立工作區
  <!--* By importing record types using an Excel or CSV file-->

如需Workfront Planning欄位的詳細資訊，請參閱[欄位概觀](/help/quicksilver/planning/fields/fields-overview.md)。

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

您必須具備下列專案才能存取Workfront Planning：

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
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃計畫*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p> 
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
   <td>   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--
OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level control for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## 從頭開始建立欄位 {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

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

   >[!IMPORTANT]
   >
   >    儲存欄位後，您無法變更欄位的欄位型別。

1. 繼續新增每個欄位，如下節所述。

### 單行文字 {#single-line-text}

單行文字欄位會擷取有限的英數字元資訊。 例如，您可以在單行文字欄位中擷取「擁有者」、「利害關係人」、「團隊」或「組織」單位資訊。 單行文字欄位的內容最多可包含1,000個字元。<!-- used to be 250 but just tested with 1000 and it allowed this as a maximum. -->

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**單行文字**&#x200B;欄位型別。

   ![](assets/single-line-text-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位型別的名稱，它將顯示在資料表或記錄的詳細資訊頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠懸停在表格中的欄位欄標題上時，會顯示欄位說明。
1. 按一下「**建立**」。

   新的單行欄位會新增為記錄型別的欄，其值可以與記錄相關聯。


### 段落 {#paragraph}

段落欄位會擷取有關記錄的其他英數字元資訊，類似於「說明」欄位。

>[!TIP]
>
>* 一個記錄型別最多可以有20個段落欄位。
>
>* 段落欄位的內容最多可包含100,000個字元。
>* 當段落欄位顯示在表格檢視或記錄的詳細資訊頁面時，您可以使用RTF格式來增強段落欄位的內容。 如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。
>


1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**段落**&#x200B;欄位型別。

   ![](assets/paragraph-field-type.png)


1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位型別的名稱，它將顯示在資料表或記錄的詳細資訊頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
1. 按一下「**建立**」。

   新的段落欄位會新增為記錄型別的欄，其值可以與記錄相關聯。


### 多選 {#multi-select}

您可以從下拉式選單中選取多個選項，使用多選欄位來擷取任何格式的其他資訊。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**多重選取**&#x200B;欄位型別。

   ![](assets/multi-select-field-type.png)


1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位型別的名稱，它將顯示在資料表或記錄的詳細資訊頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
   * **選擇**：儲存欄位後，可從下拉式功能表中選取的選項。 每個選擇的名稱可以同時使用數字和字母。
1. 按一下&#x200B;**新增選擇**，視需要新增多個選擇。 您可以在多重選取欄位中新增多少選擇，沒有限制。
1. （選用）以所需順序手動拖放每個選項，或選取
   如果您希望選擇自動依字母順序列出，請&#x200B;**將選擇A-Z**&#x200B;選項排序。<!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. （選擇性）若要移除選擇，請按一下選擇右側的&#x200B;**x**&#x200B;圖示。
1. 按一下選項左側的色票，即可展開顏色選取器並自訂每個選項的顏色。
1. 按一下「**建立**」。

   新的多重選取欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 單選 {#single-select}

從下拉式功能表中選取一個選項，單選欄位即可擷取任何格式的其他資訊。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**單選**&#x200B;欄位型別。

   ![](assets/single-select-field-type.png)


1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位型別的名稱，它將顯示在資料表或記錄的詳細資訊頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
   * **選擇**：儲存欄位後，可從下拉式功能表中選取的選項。 每個選擇的名稱可以同時使用數字和字母。

1. 按一下&#x200B;**新增選擇**，視需要新增多個選擇。 您可以新增多少選項至單一選取欄位，沒有限制。
1. （選擇性）以所要的順序手動拖放每個選擇，或選取&#x200B;**將選擇排序A-Z**&#x200B;選項（如果您希望選擇自動依字母順序列出）。<!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. （選擇性）若要移除選擇，請按一下選擇右側的&#x200B;**x**&#x200B;圖示。
1. 按一下選項左側的色票，即可展開顏色選取器並自訂每個選項的顏色。
1. 按一下「**建立**」。

   新的單選欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 日期 {#date}

您可以使用日期欄位來擷取日期和時間格式的其他資訊。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**日期**&#x200B;欄位型別。

   ![](assets/date-field-type.png)


1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
   * **日期格式**：您要在此欄位中顯示的日期格式型別。<!--update this casing - submitted bug for it-->

     從下列格式中選取：
      * **地區**：符合瀏覽器的地區。
      * **標準**： 05/16/2023
      * **長**：2023年5月16日
      * **歐洲**： 16/05/2023
      * **ISO**： 2023-05-16
   * **包含時間欄位**：若要包含時間戳記，請選取此選項。 預設會取消選取此選項。<!--update this setting name - submitted bug for it to be changed-->

     從下列選項中選取：

      * **24hr**：例如： 18:00
      * **12hr**：例如：下午6:00

1. 按一下「**建立**」。

   新的日期欄位會新增為記錄型別的欄，其值可以與記錄相關聯。

### 數字 {#number}

數字欄位型別會以數字格式擷取資訊。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**數字**&#x200B;欄位型別。

   ![](assets/number-field-type.png)
1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
   * **精確度**：您要為欄位記錄的小數位數。 您最多可以顯示6個小數。
   * **允許負數**：如果您要在此欄位中允許負數，請選取此選項。 預設會取消選取此選項。

   >[!NOTE]
   >
   >    如果您選取「允許負數」，且負值儲存在附加欄位的記錄上，則以後無法再取消選取設定。

1. 按一下「**建立**」。

   新數字欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 百分比 {#percentage}

百分比欄位型別會以數字格式擷取資訊，後面接著百分比符號。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**百分比**&#x200B;欄位型別。

   ![](assets/percentage-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
   * **精確度**：您要為欄位記錄的小數位數。 您最多可以顯示6個小數。
   * **允許負數**：若要允許此欄位中有負百分比值，請選取此選項。 預設會取消選取此選項。

   >[!NOTE]
   >
   >    如果您選取「允許負數」，且負值儲存在附加欄位的記錄上，則以後無法再取消選取設定。

1. 按一下「**建立**」。

   新的百分比欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 貨幣 {#currency}

貨幣欄位型別會以數字格式擷取資訊，前面加貨幣符號。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**貨幣**&#x200B;欄位型別。

   ![](assets/currency-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
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

   ![](assets/checkbox-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
1. 按一下「**建立**」。

   新的核取方塊欄位會新增為記錄型別的欄，其值可以與記錄相關聯。

### 公式

公式欄位會使用記錄型別中其他欄位的現有值，以及指示應如何計算現有值的函式，來產生新值。

如需詳細資訊，請參閱[公式欄位概述](/help/quicksilver/planning/fields/formula-fields.md)。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**公式**&#x200B;欄位型別。

   ![](assets/new-formula-field-with-list-of-expressions.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：輸入新欄位的名稱。
   * **描述**：新增有關新欄位的資訊。
   * **公式**：開始輸入至少一個字元以存取運算式，然後在運算式顯示在清單中時選取它。

1. 按一下選取的運算式以顯示定義並檢視其格式。

   ![](assets/description-of-formula-expression.png)

   如需支援哪些運算式的詳細資訊，請參閱[公式欄位概觀](/help/quicksilver/planning/fields/formula-fields.md)。

1. 新增在Workfront Planning中顯示的欄位名稱，以在公式中參照它們。

   >[!NOTE]
   >
   >* 您無法在公式中新增多重選取型別欄位。
   >
   >* 您可以參考與目前記錄型別相距最多4個層級的欄位。 例如，如果您正在建立「活動」記錄型別的公式欄位，且「活動」已連線至「產品」記錄型別，而該記錄型別已連線至「行銷活動」記錄型別，而該記錄型別已連線至「Workfront專案」，則您可以在針對「活動」記錄型別建立的公式中參考專案的「預算」。

1. 在&#x200B;**格式**&#x200B;欄位中，從下列選項中選取，以識別公式型別欄位中顯示結果的格式：

   * **文字**：公式欄位的結果顯示為純文字。
   * **數字**：公式欄位的結果顯示為數字。
   * **百分比**：公式欄位的結果顯示為後面跟著百分比符號的數字。
   * **貨幣**：公式欄位的結果顯示為前面或後面跟著貨幣符號的數字。
   * **標籤**：公式欄位的結果會以標籤與物件名稱一起顯示。

     >[!TIP]
     >
     >我們建議將標籤用於顯示陣列的欄位。 在這種情況下，每個陣列成員都會顯示為個別標籤。

     ![](assets/formula-field-formats-list-with-tag-selected-highlighted.png)

   * **日期**：公式欄位的結果顯示為日期。

     結果預覽會顯示在&#x200B;**格式**&#x200B;欄位下。

     >[!WARNING]
     >
     >如果公式的結果不符合所選的格式，則欄位將顯示錯誤訊息。

1. 按一下「**建立**」。

   新的公式欄位會新增為記錄型別的欄，其值可以與記錄相關聯。

### 人員

您可以使用[人員]欄位型別將使用者<!--, job role, or team-->新增到記錄。 這是預先輸入欄位，您只能新增已在Workfront執行個體中的使用者<!--, roles, or teams-->。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**人員**&#x200B;欄位型別。

   ![](assets/people-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：
   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
   * **允許多個值**：如果您要允許使用者在此欄位中新增一個以上的使用者，請選取此選項。 預設會取消選取此選項。

   >[!NOTE]
   >
   >    如果您選取「允許多個值」，且有多個使用者儲存在附加欄位的記錄中，則以後編輯此欄位時，無法再取消選取設定。

1. 按一下「**建立**」。

   新的「人員型別」欄位會新增為記錄型別的欄，其值可與記錄相關聯。

### 建立者

您可以使用「建立者」欄位型別，將建立記錄的使用者新增至記錄。 這是唯讀欄位，會自動填入建立記錄時登入的使用者名稱。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**建立者**&#x200B;欄位型別。

   ![](assets/created-by-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。<!--this might change and they might prepopulate it with "Created by"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。

1. 按一下「**建立**」。

   新的「建立者型別」欄位會新增為記錄型別的欄，其值會預先填入建立每個記錄的使用者名稱。


### 建立日期

您可以使用「建立日期」欄位型別，將記錄的建立日期新增至記錄。 這是唯讀欄位，會自動填入建立記錄的日期（以及可選的時間）。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**建立日期**&#x200B;欄位型別。

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。<!--this might change and they might prepopulate it with "Created date"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
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

   ![](assets/last-modified-by-field-type.png)

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。<!--this might change and they might prepopulate it with "Created by"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。

1. 按一下「**建立**」。

   新的「上次修改者」型別欄位會新增為記錄型別的欄，其值會預先填入上次修改每筆記錄的使用者名稱。


### 上次修改日期

您可以使用「上次修改日期」欄位型別來新增上次將記錄修改至記錄的日期。 這是唯讀欄位，會自動填入上次修改記錄的日期（以及可選的時間）。

1. 依照本文中[從頭開始建立欄位](#create-fields-from-scratch)一節的說明開始建立欄位，然後選取&#x200B;**建立日期**&#x200B;欄位型別。

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 在&#x200B;**新欄位**&#x200B;索引標籤中新增下列資訊：

   * **名稱**：欄位型別的名稱，它會出現在資料表或記錄頁面中。<!--this might change and they might prepopulate it with "Created date"-->
   * **描述**：有關欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
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

## 透過連線記錄型別建立欄位

當您在兩個記錄型別之間新增連線，或記錄型別和其他應用程式的物件型別之間新增連線時，可以建立連結的記錄欄位。

如需有關連線Workfront Planning記錄型別的資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)

<!--## Create fields by importing record types using an Excel or CSV file

For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).-->

## 建立記錄型別以建立欄位

建立記錄型別時，依預設也會建立與新記錄型別相關聯的多個欄位。 如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

## 從範本建立工作區以建立欄位

當您從範本建立工作區時，Adobe Workfront Planning會為記錄型別建立欄位。

如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。