---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: 使用中的函式來對應專案 [!DNL Adobe Workfront Fusion]
description: 對映專案時，您可以使用函式來建立簡單或複雜的公式。
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# 使用中的函式來對應專案 [!DNL Adobe Workfront Fusion]

對映專案時，您可以使用函式來建立簡單或複雜的公式。

中可用的函式 [!DNL Adobe Workfront Fusion] 類似於Excel和某些程式語言中的函式。 它們會評估一般邏輯、數學、文字、日期和陣列。 它們可讓您執行專案值的條件邏輯和轉換，例如將文字轉換為大寫、裁剪文字、將日期轉換為不同格式等。 如需詳細資訊，請參閱 [在Adobe Workfront Fusion中將資訊從一個模組對應到另一個模組](../../workfront-fusion/mapping/map-information-between-modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 將函式插入欄位

如果您按一下欄位， [!UICONTROL 對應] 面板顯示。 對應面板包含數個標籤：

![](assets/functions-toolbar-350x189.png)

第一個索引標籤 ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) （開啟面板時顯示）顯示可從其他模組對應的專案。

其他標籤包含下列型別的函式：

* **一般函式** ![](assets/toolbar-icon-general-function.png)  — 請參閱 [中的一般函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) 以取得詳細資訊。

* **數學函式** ![](assets/toolbar-icon-math-functions.png)  — 請參閱 [中的數學函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) 以取得詳細資訊。

* **文字和二進位函式** ![](assets/toolbar-icon-text&binary-functions.png)  — 請參閱 [中的字串函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) 以取得詳細資訊。

* **日期與時間** ![](assets/toolbar-icon-date&time-functions.png)  — 請參閱 [中的日期和時間函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 和以下文章以取得詳細資訊。

   * [日期和時間格式的Token [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [中用於日期和時間剖析的Token [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **使用陣列的功能** ![](assets/toolbar-icon-functions-for-arrays.png)  — 請參閱 [中的陣列函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) 以取得詳細資訊。

若要將函式插入欄位：

1. 按一下函式名稱。

   或

   將函式拖曳至欄位。

>[!INFO]
>
>**範例：** 有些資料型別會防止使用者輸入超過特定數目的字元。 您可以使用子字串函式來限制值為特定字元數。
>
>在此範例中，子字串函式將專案名稱限製為50個字元。
>
>![](assets/example-meet-length-restriction-350x184.png)

## 巢狀函式

您可以互相巢狀內嵌函式。

## 使用 [!DNL Google Sheets] 函式

若 [!DNL Workfront Fusion] 不提供您想使用的功能，但主要提供 [!DNL Google Sheets]，您可依照下列步驟使用：

1. 在 [!DNL Google Sheets]，建立新的空白試算表。
1. 在 [!DNL Workfront Fusion]，開啟您的情境。
1. 新增 **[!DNL Google Sheets]** >**[!UICONTROL 更新儲存格]** 模組至情境。

   如需新增模組的指示，請參閱 [在情境中新增模組](../../workfront-fusion/scenarios/create-a-scenario.md#add) 在文章中 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 設定模組：

   1. 選擇新建立的試算表於 **[!UICONTROL 試算表]** 欄位。
   1. 插入包含 [!DNL Google Sheets] 函式放入 **[!UICONTROL 值]** 欄位。

      您可以照常使用先前模組的輸出。

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. 插入 **[!UICONTROL Google工作表] >[!UICONTROL 取得儲存格]** 模組，以取得計算結果。
1. 使用您在步驟4中使用的相同儲存格ID來設定模組。

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
