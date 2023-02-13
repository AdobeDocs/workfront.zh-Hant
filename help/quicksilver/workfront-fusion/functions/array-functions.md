---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的陣列函式
description: Adobe Workfront Fusion對應面板中提供下列陣列函式。
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Adobe Workfront Fusion中的陣列函式

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

## [!UICONTROL add(array)value1;value2;...)]

將參數中指定的值添加到陣列並返回該陣列。

## [!UICONTROL 包含(array)value)]

驗證陣列是否包含值。

## [!UICONTROL 相異（陣列） [key])]

移除陣列內的重複項目。 使用「[!UICONTROL key]&quot;參數，用於訪問複雜對象內的屬性。 若要存取巢狀屬性，請使用點記號。 陣列中的第一個項是索引1。

>[!INFO]
>
>**範例：** `distinct(Contacts[];name)`
>
>通過比較&quot;name&quot;屬性來刪除聯繫人陣列內的重複項

## [!UICONTROL 平面化（陣列）]

建立新陣列，將所有子陣列元素以遞歸方式串連到其中，直至指定的深度。


## [!UICONTROL 連接（陣列）分隔符號]

使用每個項目之間指定的分隔符將陣列的所有項目串連到字串中。

## [!UICONTROL 索引鍵（物件）]

返回給定對象或陣列屬性的陣列。

## [!UICONTROL length（陣列）]

傳回陣列中的項目數。

## [!UICONTROL 地圖（複雜陣列）鍵；[篩選索引鍵];[篩選的可能值])]

返回包含複雜陣列的值的基元陣列。 此函式可允許篩選值。 對索引鍵使用原始變數名稱。

>[!INFO]
>
>**範例:**
>
>* `map(Emails[];email)`
  >
>  傳回包含電子郵件的原始陣列
>
>* `map(Emails[];email;label;work;home)`
  >
>  傳回原始陣列，其電子郵件的標籤等於工作或家庭

如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL 合併(array1)array2;...)]

將一個或多個陣列合併到一個陣列中。

## [!UICONTROL 刪除（陣列）value1;value2;...)]

移除陣列參數中指定的值。 此函式僅對文本或數字的基元陣列有效。

## [!UICONTROL 反向（陣列）]

陣列的第一個元素變成最後一個元素，第二個元素變成倒數第二個，以此類推。

## [!UICONTROL 片（陣列）開始； [結束])]

傳回僅包含所選項目的新陣列。

## [!UICONTROL 排序（陣列） [訂購]; [key])]

對陣列的值進行排序。 的有效值 `order` 參數為：

* `asc`

   （預設） — 遞增順序：1, 2, 3, ...，用於類型編號。 A, B, C, a, b, c, ...，用於類型文本

* `desc`

   降序順序：..., 3, 2, 1，表示類型編號。... c、b、a、C、B、A表示類型文字。

* `asc ci`

   不區分大小寫的升序：A, a, B, b, C, c, ...，用於「文本」類型。

* `desc ci`

   不區分大小寫的降序順序：..., C, c, B, b, A, a，表示「文字」。

使用 `key` 參數來存取複雜物件內的屬性。

對索引鍵使用原始變數名稱。

若要存取巢狀屬性，請使用點記號。

陣列中的第一個項是索引1。

>[!INFO]
>
>**範例:**
>
>* `sort(Contacts[];name)`
   >
   >    按預設升序按「name」屬性對聯繫人陣列進行排序
>
>* `sort(Contacts[];desc;name)`
   >
   >   按「name」屬性以降序對聯繫人陣列進行排序
>
>* `sort(Contacts[];asc ci;name)`
   >
   >    按不區分大小寫的升序按&quot;name&quot;屬性對聯繫人陣列進行排序
>
>* `sort(Emails[];sender.name)`
   >
   >    按照「sender.name」屬性對電子郵件陣列進行排序


## [!UICONTROL arrayDifference [array1, array2, mode]]

傳回兩個陣列之間的差異。

為 `mode` 參數。

* `classic`:傳回包含 `array1` 中不存在 `array2`.

* `symmetric`:傳回兩個陣列不通用的元素陣列。

   換言之，函式會傳回包含 `array1` 中不存在 `array2`，以及 `array2` 中不存在 `array1`.

   >[!INFO]
   >
   >**範例:**
   >
   >提供下列陣列：
   >
   >
   ```
   >myArray = [1,2,3,4,5]
   >```
   >
   >
   ```
   >yourArray = [3,4,5,6,7]
   >```
   >
   >* `arrayDifference [myArray, yourArray, classic]`
      >
      >    傳回 `[1,2]`
   >
   >* `arrayDifference [yourArray, myArray, classic]`
      >
      >    傳回 `[6,7]`
   >
   >* `arrayDifference [myArray, yourArray, symmetric]`
      >
      >    傳回 `[1,2,6,7]`

