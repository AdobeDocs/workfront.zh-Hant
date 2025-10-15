---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算自訂欄位範例：在問題自訂表單上顯示問題建立者的管理員
description: 使用計算自訂欄位，您可以在附加到問題的自訂表單上顯示問題建立者的經理名稱。 使用相同的陳述式，您可以為專案、問題和其他物件建置類似的計算欄位。
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 計算自訂欄位範例：在問題自訂表單上顯示問題建立者的管理員

使用計算自訂欄位，您可以在附加到問題的自訂表單上顯示問題建立者的經理名稱。 使用相同的陳述式，您可以為專案、問題和其他物件建置類似的計算欄位。

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront套件</p> </td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront授權</p> </td> 
   <td>
      <p>標準</p>
      <p>規劃</p></td>
  </tr> 
  <tr> 
   <td><p>存取層級設定</p></td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr> 
  <tr> 
   <td> <p>物件許可權</p> </td> 
   <td> <p>貢獻對表單所附加物件的存取權以編輯自訂表單</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在問題自訂表單上顯示問題建立者的管理員

下列步驟顯示如何為問題自訂表單建立計算欄位，您可以在其中擷取建立問題之使用者的管理員名稱。 例如，當您想要擷取建立任務、專案和投資組合之使用者的經理姓名時，程式是相同的。

1. 建立問題自訂表單，並在其中新增計算欄位。

   如需建立自訂表單及新增計算欄位的相關資訊，請參閱下列文章：

   * [建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [新增計算欄位至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. 將下列文字模式程式碼複製並貼到自訂表單的&#x200B;**計算**&#x200B;欄位中：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >自訂欄位計算區分大小寫。

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存+關閉**。

   當包含欄位的表單附加到問題時，建立問題的使用者的管理員顯示在計算欄位中。
