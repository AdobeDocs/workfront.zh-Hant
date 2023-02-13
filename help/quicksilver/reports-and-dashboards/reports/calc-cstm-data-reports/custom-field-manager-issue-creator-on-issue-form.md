---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '"計算自訂欄位範例：在期刊自訂表單上顯示期刊建立者的管理員」'
description: 使用計算的自訂欄位，您可以在附加至期刊的自訂表單上顯示期刊建立者經理的名稱。 使用同一語句，可以為項目、問題和其他對象建立類似的計算欄位。
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 計算的自訂欄位範例：在期刊自訂表單上顯示期刊建立者的管理員

使用計算的自訂欄位，您可以在附加至期刊的自訂表單上顯示期刊建立者經理的名稱。 使用同一語句，可以為項目、問題和其他對象建立類似的計算欄位。

>[!TIP]
>
>如需其他客戶的其他自訂文字模式範例相關資訊，請遵循 [文字模式報表](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) 社群網站上的主題。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront授權*</p> </td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>訪問級別配置*</td> 
   <td> <p>管理對自訂表單的存取<br>有關從訪問級別授予管理訪問權限的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>物件權限</p> </td> 
   <td> <p>對表單附加的物件提供存取權，以存取「編輯自訂表單」</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在期刊自訂表單上顯示期刊建立者的管理員

下列步驟顯示如何為問題自訂表單建立計算欄位，以便擷取建立問題之使用者的管理員名稱。 當您想要擷取建立任務、專案、產品組合之使用者（例如）的經理名稱時，此程式相同。

1. 建立問題自訂表單並新增計算欄位。

   如需建立自訂表單及新增計算欄位的相關資訊，請參閱下列文章：

   * [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. 將下列文字模式程式碼複製並貼到 **計算** 自訂表單欄位：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >自訂欄位計算區分大小寫。

1. 按一下 **完成**，然後 **儲存+關閉**.

   當包含欄位的表單附加至問題時，建立問題的使用者管理員會顯示在計算欄位中。
