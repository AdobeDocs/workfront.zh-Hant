---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: 使用 [!DNL Adobe Workfront Fusion]中的函式對應專案
description: 對映專案時，您可以使用函式來建立簡單或複雜的公式。
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: d175a3d43f13338661d8b7e1cb79038a36522ff9
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 使用[!DNL Adobe Workfront Fusion]中的函式對應專案

對映專案時，您可以使用函式來建立簡單或複雜的公式。 [!DNL Adobe Workfront Fusion]中可用的函式類似於Excel中的函式以及某些程式語言中的函式：

* 它們會評估一般邏輯、數學、文字、日期和陣列。
* 它們可讓您執行專案值的條件邏輯和轉換，例如將文字轉換為大寫、裁剪文字、將日期轉換為不同格式等等。

如需詳細資訊，請參閱[在Adobe Workfront Fusion中將資訊從一個模組對應到另一個模組](../../workfront-fusion/mapping/map-information-between-modules.md)。


## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">

<col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td>  
   <td> <p>任何</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td>  
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Work]或更高版本</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td>  
   <td> 
   <p>目前：無[!DNL Workfront Fusion]授權需求。</p> 
   <p>或</p> 
   <p>舊版：任何 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">產品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]計畫：您的組織必須購買[!DNL Adobe Workfront Fusion]。</li><li>已包含[！UICONTROL Ultimate] [!DNL Workfront]計畫： [!DNL Workfront Fusion]。</li></ul> 
   <p>或</p> 
   <p>目前：您的組織必須購買[!DNL Adobe Workfront Fusion]。</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。


## 對應索引標籤概觀

若要開啟欄位的[!UICONTROL 對應]面板：

1. 按一下左側面板中的&#x200B;**情境**。
1. 選擇情境。

![](assets/open-functions-bar.png)


### 對應面板索引標籤

以下是對映面板中的標籤：

* **一般函式** ![](assets/toolbar-icon-general-function.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md)中的[一般函式。

* **數學函式** ![](assets/toolbar-icon-math-functions.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md)中的[數學函式。

* **文字和二進位函式** ![](assets/toolbar-icon-text&binary-functions.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md)中的[字串函式。

* **日期與時間** ![](assets/toolbar-icon-date&time-functions.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md)中的[日期與時間函式，以及下列文章：

   * [ [!DNL Adobe Workfront Fusion]中日期和時間格式的Token](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [ [!DNL Adobe Workfront Fusion]中日期和時間剖析的權杖](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **使用陣列的函式** ![](assets/toolbar-icon-functions-for-arrays.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md)中的[陣列函式。

* **對應其他函式** ![](assets/toolbar-icon-functions-you-map-from-other-modules.png)會顯示您可以從其他模組對應的專案。 此標籤並非總是可用。

![](assets/functions-toolbar-350x189.png)

## 將函式插入欄位

若要將函式插入欄位：

1. 按一下函式名稱。

   或

   將函式拖曳至欄位。


>[!BEGINSHADEBOX]

**範例：**&#x200B;有些資料型別會防止使用者輸入超過特定數目的字元。 您可以使用子字串函式將值限製為特定字元數。

在此範例中，子字串函式將專案名稱限製為50個字元。

![](assets/example-meet-length-restriction-350x184.png)

>[!ENDSHADEBOX]

## 巢狀函式

您可以巢狀內嵌函式。

## 使用[!DNL Google Sheets]函式

如果[!DNL Workfront Fusion]沒有您要使用的功能，但它由[!DNL Google Sheets]所提供，您可以依照下列步驟來使用：

1. 在[!DNL Google Sheets]中建立新的空白試算表。
1. 在[!DNL Workfront Fusion]中，開啟您的情境。
1. 將&#x200B;**[!DNL Google Sheets]** >**[!UICONTROL 更新儲存格]**&#x200B;模組至情境。

   如需新增模組的說明，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立情境[在情境中新增模組](../../workfront-fusion/scenarios/create-a-scenario.md#add)。

1. 設定模組：

   1. 在&#x200B;**[!UICONTROL 試算表]**&#x200B;欄位中選擇新建立的試算表。
   1. 將包含[!DNL Google Sheets]函式的公式插入&#x200B;**[!UICONTROL 值]**&#x200B;欄位。

      您可以照常使用先前模組的輸出。

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. 插入&#x200B;**[!UICONTROL Google工作表] >[!UICONTROL 取得儲存格]**&#x200B;模組以取得計算結果。
1. 使用您在步驟4中使用的相同儲存格ID來設定模組。

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
