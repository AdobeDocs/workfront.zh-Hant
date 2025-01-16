---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 在 [!DNL Adobe] Workfront Fusion中對應陣列
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中對應陣列

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [對應陣列或陣列元素](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-an-array.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

陣列是一種特殊型別的專案，可包含下列專案：

* 一或多個文字值（簡單陣列）
* 相同型別（複雜陣列）的一或多個集合

>[!INFO]
>
>**範例：** [!UICONTROL 觀看電子郵件]模組傳回每個電子郵件的附件陣列。 每個附件代表一個集合，其中可能包含名稱、內容、大小等。

如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)中的[專案資料型別。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。



## 對應整個陣列

1. 在您對應陣列的模組中，按一下您要對應陣列的欄位。 這是陣列對應的欄位。

1. 在顯示的方塊中，對應專案。

   面板可讓您以與其他任何型別專案相同的方式對應欄位。 如果您不想分別填入每個專案，但想將另一個陣列對應到目標欄位，請使用[!UICONTROL 對應]按鈕。 在此情況下，請確定兩個陣列（來源陣列和目標陣列）具有相同的結構。

   您可以新增任意數量的專案至陣列。

您可以使用疊代器將陣列分割成個別的組合。 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/modules/iterator-module.md)中的[[!UICONTROL 迭代器]模組。

## 將專案對應至新陣列

Workfront Fusion中的某些欄位可讓您將元素對應至陣列。 例如，您可以在「Workfront面板>新增檢查清單專案模組」中建立一系列檢查清單專案。 執行模組時，所有檢查清單專案都會新增至卡片。

任何顯示「新增專案」的模組欄位都會建立陣列。

![新增專案](assets/add-item.png)

若要將元素新增至陣列：

1. 按一下&#x200B;**新增專案**
1. 在開啟的面板中，輸入有關專案的詳細資訊。
1. 按一下&#x200B;**新增**。
1. （選擇性）針對您想要新增至陣列的每個元素，重複步驟1至3。

## 對應陣列元素


### 依數字對應陣列元素

陣列元素會在陣列名稱后方括弧中顯示為數字。 您可以使用此索引編號將陣列的個別元素對應到欄位中。

![](assets/map-array-1st-element.png)

>[!NOTE]
>
>Workfront Fusion中的陣列索引從1開始。

若要對應陣列元素：

1. 按一下您要對應元素的欄位。

   對應面板隨即開啟。

1. 找到包含您要對應的元素的陣列。
1. 按一下陣列旁的下拉箭頭。
1. 按一下您要對應的元素。

   元素會進行對應，索引為1。 這會對映陣列中的第一個元素。

1. 若要對應陣列的不同元素，請按一下[1]並輸入您要對應的陣列元素的索引編號。

   ![](assets/access-another-element.png)

### 使用指定索引鍵對應陣列的元素

某些陣列包含具有索引鍵值專案（例如中繼資料、屬性等）的集合。 若要使用其中一個值，您可以依照元素指定的索引鍵值來查詢元素，並從值專案中取得對應的值。 我們建議使用採用`map()`與`get()`函式組合的公式。



>[!BEGINSHADEBOX]

下列範例顯示[!DNL Jira]應用程式的輸出。

![](assets/output-of-jira-app-350x100.png)

此範例會針對識別碼為10108的特定附件，從附件的陣列取得檔案名稱。

此範例會產生下列輸出：

![](assets/output-from-jira-350x261.png)

公式的說明如下：

* `map`

   1. `map()`函式的第一個引數是整個陣列專案。
   1. 第二個引數是值專案的原始名稱。 若要取得原始名稱，請將游標停留在[!UICONTROL 對應]面板中的專案上：

      ![](assets/obtain-raw-name-350x124.png)

      >[!NOTE]
      >
      >所有引數都區分大小寫。 即使在此特定範例中，專案的標籤與其原始名稱不同（僅在大寫中），但必須使用原始名稱。

   1. 第三個引數是關鍵專案的原始名稱：

      ![](assets/3rd-parameter-350x166.png)

   1. 第四個引數是指定的機碼值。

  由於`map()`函式傳回陣列（因為可能有更多具有指定索引鍵值的元素），所以必須套用`get()`函式才能取得其第一個元素：

* `get`

   1. `get()`函式的第一個引數是`map()`函式的結果。

   1. 第二個引數是元素的索引。 在此範例中，索引為`1`。

此範例會產生下列輸出：

![](assets/output-from-jira-350x261.png)

>[!ENDSHADEBOX]

如需`map()`函式的詳細資訊，請參閱[陣列函式](/help/quicksilver/workfront-fusion/functions/array-functions.md)。

如需`get()`函式的詳細資訊，請參閱[一般函式](/help/quicksilver/workfront-fusion/functions/general-functions.md)。

## 將陣列元素轉換為一系列組合

可以使用[!UICONTROL 疊代器]模組將陣列轉換為一系列組合。 如需詳細資訊，請參閱[[!UICONTROL 迭代器]模組](/help/quicksilver/workfront-fusion/modules/iterator-module.md)。

![](assets/series-of-bundles.png)

