---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: 在中使用函式映射項目 [!DNL Adobe Workfront Fusion]
description: 映射項目時，可以使用函式建立簡單或複雜的公式。
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 在中使用函式映射項目 [!DNL Adobe Workfront Fusion]

映射項目時，可以使用函式建立簡單或複雜的公式。

中可用的函式 [!DNL Adobe Workfront Fusion] 類似於Excel和某些寫程式語言中的函式。 他們會評估一般邏輯、數學、文字、日期和陣列。 它們可讓您執行條件式邏輯和項目值的轉換，例如將文字轉換為大寫、修剪文字、將日期轉換為不同格式等。 如需詳細資訊，請參閱 [在Adobe Workfront Fusion中，將資訊從一個模組對應至另一個模組](../../workfront-fusion/mapping/map-information-between-modules.md).

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 將函式插入欄位

如果按一下欄位，則 [!UICONTROL 映射] 面板隨即顯示。 「對應」面板包含數個索引標籤：

![](assets/functions-toolbar-350x189.png)

第一個標籤 ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) （在開啟面板時顯示）會顯示您可從其他模組對應的項目。

其他索引標籤包含下列類型的函式：

* **一般函式** ![](assets/toolbar-icon-general-function.png)  — 請參閱 [中的一般函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) 以取得更多資訊。

* **數學函式** ![](assets/toolbar-icon-math-functions.png)  — 請參閱 [中的數學函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) 以取得更多資訊。

* **文本和二進位函式** ![](assets/toolbar-icon-text&binary-functions.png)  — 請參閱 [中的字串函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) 以取得更多資訊。

* **日期和時間** ![](assets/toolbar-icon-date&time-functions.png)  — 請參閱 [日期和時間函式，於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 以及以下文章以取得詳細資訊。

   * [日期和時間格式的代號，位於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [日期和時間剖析的代號(在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **使用陣列的功能** ![](assets/toolbar-icon-functions-for-arrays.png)  — 請參閱 [中的陣列函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) 以取得更多資訊。

要將函式插入欄位：

1. 按一下函式名稱。

   或

   將函式拖曳至欄位。

>[!INFO]
>
>**範例：** 有些資料類型會防止使用者輸入超過特定數量的字元。 您可以使用子字串函式將值限制為特定數量的字元。
>
>在此範例中，子字串函式將專案名稱限制為50個字元。
>
>![](assets/example-meet-length-restriction-350x184.png)

## 嵌套函式

您可以相互巢狀內嵌函式。

## 使用 [!DNL Google Sheets] 函式

若 [!DNL Workfront Fusion] 不提供您想使用的函式，但是此功能為 [!DNL Google Sheets]，您可以依照下列步驟來使用：

1. 在 [!DNL Google Sheets]，建立新的空白試算表。
1. 在 [!DNL Workfront Fusion]，開啟您的藍本。
1. 新增 **[!DNL Google Sheets]** >**[!UICONTROL 更新儲存格]** 模組至案例。

   如需新增模組的指示，請參閱 [在案例中新增模組](../../workfront-fusion/scenarios/create-a-scenario.md#add) 在文章中 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 設定模組：

   1. 在中選擇新建立的試算表 **[!UICONTROL 試算表]** 欄位。
   1. 插入包含 [!DNL Google Sheets] 函式到 **[!UICONTROL 值]** 欄位。

      您可以照常使用先前模組的輸出。

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. 插入 **[!UICONTROL Google工作表] >[!UICONTROL 獲取手機]** 模組獲取計算結果。
1. 使用您在步驟4中使用的相同儲存格ID來設定模組。

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
