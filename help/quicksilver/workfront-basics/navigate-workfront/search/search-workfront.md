---
navigation-topic: search
title: 搜尋 [!DNL Adobe Workfront]
description: 您可以輕鬆地在 [!DNL Adobe Workfront] 當你無法記住他們的確切位置時，搜索他們。
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 1%

---

# 搜尋 [!DNL Adobe Workfront]

您可以輕鬆地在 [!DNL Adobe Workfront] 當你無法記住他們的確切位置時，搜索他們。

您可以看到 [!UICONTROL 搜尋] 框(位於 [!DNL Workfront].

![](assets/search-globalnavigationbar-350x62.png)

您必須具有查看對象的權限，然後才能在搜索中找到該對象。 因此，搜尋結果會因使用者而異。

## 存取需求

+++ 展開本區段以檢視執行本文所述步驟所需的存取權。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL視圖]對對象類型的訪問 </p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>您必須具有查看對象的權限，然後才能在搜索中找到該對象。</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

+++

## 了解搜尋

* [[!UICONTROL 可搜索的對象]](#objects-available-for-search)
* [[!UICONTROL 可搜索的欄位]](#fields-available-for-search)

### 可搜索的對象

您可以在Workfront中搜尋下列物件：

* 專案
* 任務
* 問題
* 報告
* 使用者
* 範本
* 文件
* 專案組合
* 計劃
* 儀表板
* 公司
* 附註

### 可搜索的欄位

可用於搜索的欄位基於搜索類型：基本或 [!UICONTROL 進階搜尋].

* **基本搜尋**:在基本搜索中搜索對象時， [!DNL Workfront] 在下列欄位中尋找可能包含關鍵字的文字：

   * 對象名稱
   * 說明
   * 自訂資料欄位
   * 更新
   * 文檔名稱（在特定文檔搜索和基本搜索中）

   有關中的基本搜索的詳細資訊，請參閱 [!DNL Workfront]，請參閱 [基本搜尋](#basic-search) 這篇文章。

* **[!UICONTROL 進階搜尋]**:在 [!UICONTROL 進階搜尋]，您可以設定篩選器來搜尋基本搜尋中無法使用的欄位。 因此， [!UICONTROL 進階搜尋] 可讓您搜尋物件中的任何欄位。

   如需 [!UICONTROL 進階搜尋]，請參閱 [進階搜尋](#advanced-search) 這篇文章。

>[!NOTE]
>
>若要執行 [!UICONTROL 進階搜尋]，您必須選取 [!UICONTROL 進階搜尋] 選項。 您無法將基本搜尋精簡為 [!UICONTROL 進階搜尋].

## 了解 [!DNL Workfront] 搜尋

使用 [!UICONTROL 搜尋] in [!DNL Workfront]:

* 搜尋不區分大小寫
* [!DNL Workfront] 不正確或理解錯字
* 在中搜尋 [!DNL Workfront] 不支援萬用字元
* 在中搜尋 [!DNL Workfront] 支援部分字詞搜尋，但不支援子字串搜尋。\
   例如，搜尋關鍵字「stand」會傳回包含單字「standard」的結果，但不會傳回包含單字「understand」的結果。

## 搜尋多個字詞

在搜索中包括多個單詞，並且只想查找與「搜索」框中所有單詞匹配的對象時，可以按任意順序鍵入這些單詞。

例如，搜尋「行銷示範」（不含引號）會尋找名稱如下的物件：

* 行銷示範
* 示範行銷
* 1月市場分析示範

它也會找出名稱中可能含有「行銷」的物件，以及說明中的「示範」。

不過，您可以在 [!UICONTROL 搜尋] 框，調整顯示的搜索結果：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>包括引號</td> 
   <td> <p>在雙引號內以正確順序輸入字詞，可讓您僅查找完全匹配的對象。<br>例如，搜尋「行銷示範」（含引號）會尋找名稱如下的物件：</p> 
    <ul> 
     <li> 行銷示範</li> 
     <li> 1月行銷示範</li> 
     <li>行銷示範計畫</li> 
    </ul> <p>不過，此搜尋找不到名為「示範行銷」的物件。</p> </td> 
  </tr> 
  <tr> 
   <td>包含或</td> 
   <td> <p>通過"OR"連接單詞（不帶引號），您只能查找與[!UICONTROL搜索]框中至少一個單詞匹配的對象。 可以按任何順序輸入這些字。<br>例如，搜尋「行銷或示範」（不含引號）會找到名稱如下的物件：</p> 
    <ul> 
     <li> 市場分析示範</li> 
     <li>1月市場分析示範</li> 
     <li>示範</li> 
     <li>市場分析</li> 
    </ul> <p>注意：「OR」必須為全大寫。 否則，它會被解釋為您正在搜索的短語中的另一個單詞。</p> </td> 
  </tr> 
  <tr> 
   <td>包含和</td> 
   <td> <p>通過"AND"連接單詞（不帶引號）可以僅查找與[!UICONTROL搜索]框中所有單詞匹配的對象。 可以按任何順序輸入這些字。<br>例如，搜尋「行銷和示範」（不含引號）會尋找名稱如下的物件：</p> 
    <ul> 
     <li>行銷示範</li> 
     <li>示範行銷</li> 
     <li>1月市場分析示範</li> 
    </ul> <p>注意：「AND」必須全大寫。 否則，它會被解釋為您正在搜索的短語中的另一個單詞。 同樣，包括"&amp;"（不帶引號）僅搜索包含&amp;符號的對象。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 在中使用搜尋 [!DNL Workfront]

[!DNL Workfront] 有兩種類型的搜尋：基本和進階。 如果要在常用對象欄位（如名稱或說明）中查找關鍵字，請使用基本搜索。 使用 [!UICONTROL 進階搜尋] 如果要使用篩選器來搜索其他對象欄位。

* [基本搜尋](#basic-search)
* [高級搜尋](#advanced-search)

### 基本搜尋

基本搜尋可讓您在系統中的所有物件或一次只搜尋一個物件（例如專案）上搜尋關鍵字。 [!DNL Workfront] 然後在幾個特定欄位中搜尋這些關鍵字。 然後，您可以根據所選的其他特定對象欄位來調整搜索結果 [!DNL Workfront].

有關在基本搜索中搜索的特定欄位的清單，請參見 [可搜索的欄位](#fields-available-for-search) 這篇文章。

>[!NOTE]
>
>若要執行 [!UICONTROL 進階搜尋]，您必須選取 [!UICONTROL 進階搜尋] 選項。 您無法將基本搜尋精簡為 [!UICONTROL 進階搜尋].

* [執行基本搜索](#perform-a-basic-search)
* [調整基本搜尋](#refine-a-basic-search)

#### 執行基本搜索

您可以透過下列其中一種方式執行基本搜尋：

* 跨系統中的所有對象（一般搜索）。
* 一次只有一個物件（物件專屬搜尋）。

要執行基本搜索：

1. 按一下放大鏡 ![](assets/search-icon.png) 在頁面的右上角。 您也可以輸入 **[!UICONTROL ALT + /]** 或 **[!UICONTROL 選項+ /]** 開啟 [!UICONTROL 搜尋] 功能表。

1. （選用）若要搜尋特定物件，請按一下 **[!UICONTROL 全部]** 下拉式選單中，然後選取您要搜尋的物件。

   ![](assets/search-objecttype.png)

1. 在 **[!UICONTROL 搜尋]** 框中，開始鍵入您正在搜索的資訊。\
   如需中所搜尋欄位的相關資訊， [!DNL Workfront]，請參閱 [了解搜尋](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   當你開始在搜索欄中輸入時， [!DNL Workfront] 會根據您的檢視歷史記錄提供建議，並會以藍色標示您搜尋的關鍵字。

1. 如果您要尋找的項目會顯示在 [!UICONTROL typeahead] ，按一下它。

   或

   Press **[!UICONTROL 輸入]** 執行全面搜索。 此搜尋會查詢整個資料庫，而非您最近檢視的項目。

   此 [!UICONTROL 搜尋結果] 從左側開啟的頁面投影片，涵蓋上一頁的大部分內容。

   如果你執行了一般搜索， [!DNL Workfront] 會傳回任何物件的結果，這些物件符合所搜尋任何欄位中的搜尋詞，如 [了解搜尋](#understand-search). 與搜索匹配的對象顯示在清單中。

   >[!NOTE]
   >
   >有時，字詞的變異會顯示在找到的項目清單中。\
   >例如，搜尋「行銷」會顯示名稱中包含「行銷」或「市場」的物件。

1. （選用）如果您的搜尋產生太多結果，請依照 [調整基本搜尋](#refine-a-basic-search).
1. （選用）若要返回搜尋前所在的頁面，請按一下 **[!UICONTROL 關閉]** 在右上角。

>[!NOTE]
>
>此 [!UICONTROL 搜尋結果] 頁面只有在聚焦時才會保持開啟。 離開頁面或開啟另一個頁面時，會關閉 [!UICONTROL 搜尋結果] 頁面。

#### 調整基本搜尋

執行基本搜尋後 — 如 [[!UICONTROL 執行基本搜索]](#perform-a-basic-search) — 可細化搜索。

使用搜索結果左側的工具欄縮小搜索資訊的範圍。

要定義搜索：

1. （條件性）如果執行了常規搜索，請在結果左上角的對象清單中選擇要搜索的對象。
1. 在結果左側的工具欄中查找搜索中顯示的對象的可用欄位。\
   每個欄位的值會依計數排序，每個欄位最多10個值。
1. 按一下任一欄位內的，可縮短結果清單。\
   您所做的選取會以藍色突出顯示，而您未選取的欄位值會隱藏。\
   選取每個新值後，會動態更新正確的結果。\
   ![](assets/qs-refine-search-350x175.png)

1. （選用）按一下選取的值來取消選取，並再次顯示每個欄位的所有值。

### [!UICONTROL 高級搜尋]

[!UICONTROL 進階搜尋] 可讓您使用基本搜尋無法使用的欄位和篩選器進行搜尋。 例如，您可以搜索具有特定優先順序或文檔所有者名稱的項目。

>[!NOTE]
>
>若要執行 [!UICONTROL 進階搜尋]，您必須選取 [!UICONTROL 進階搜尋] 選項。 您無法將基本搜尋精簡為 [!UICONTROL 進階搜尋].

* [使用 [!UICONTROL 進階搜尋]](#use-advanced-search)

#### 使用 [!UICONTROL 進階搜尋]

您可以使用 [!UICONTROL 進階搜尋] 以根據特定條件篩選您的搜尋。\
如果您無法記住與某個對象關聯的關鍵字，但您知道有關該對象的某些特定資訊，則此類搜索將有所幫助(例如：項目優先順序、文檔所有者名稱等)。

要執行高級搜索，請執行以下操作：

1. 位於 [!DNL Workfront]，按一下 **[!UICONTROL 搜尋]** 圖示 ![](assets/search-icon.png). 此 [!DNL Search] 功能表。

1. 在 [!UICONTROL 搜尋] 按一下 **[!UICONTROL 進階搜尋]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   此 [!UICONTROL 進階搜尋] 頁面投影片會從右側開啟，涵蓋上一頁的大部分內容。

1. 選擇要搜索的對象類型。\
   **[!UICONTROL 專案]** 預設為選取。

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. （選用）在清單頂端的欄位中輸入關鍵字。
1. （選用）按一下 **[!UICONTROL 篩選結果]** 若要根據特定欄位類型篩選搜尋結果，請從清單中選取欄位。 如有必要，也請為欄位選取值。\
   或\
   新增篩選器。

1. 按一下 **[!UICONTROL 搜尋]**.\
   符合搜尋的項目清單會顯示在 [!UICONTROL 進階搜尋] 工具欄。

1. （選用）若要返回搜尋前所在的頁面，請按一下 **[!UICONTROL 關閉]** 在右上角。

>[!NOTE]
>
>此 [!UICONTROL 搜尋結果] 頁面只有在聚焦時才會保持開啟。 離開頁面或開啟另一個頁面時，會關閉 [!UICONTROL 搜尋結果] 頁面。
