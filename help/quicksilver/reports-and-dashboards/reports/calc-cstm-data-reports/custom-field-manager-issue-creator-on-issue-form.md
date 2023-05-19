---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '"計算的自定義欄位示例：顯示問題建立者在問題自定義窗體上的經理」'
description: 使用計算的自定義欄位，可以在附加到問題的自定義表單上顯示問題建立者的管理員名稱。 使用同一語句，可以為項目、問題和其他對象構建類似的計算欄位。
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# 計算的自定義欄位示例：在問題自定義窗體上顯示問題建立者的經理

使用計算的自定義欄位，可以在附加到問題的自定義表單上顯示問題建立者的管理員名稱。 使用同一語句，可以為項目、問題和其他對象構建類似的計算欄位。

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront計畫</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront許可證*</p> </td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>訪問級別配置*</td> 
   <td> <p>對自定義表單的管理訪問<br>有關從訪問級別授予管理訪問權限的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>。</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何更改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>對象權限</p> </td> 
   <td> <p>參與訪問表單所附加的對象，並訪問「編輯自定義表單」</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 在問題自定義窗體上顯示問題建立者的經理

以下步驟顯示如何為問題自定義表單建立計算欄位，在該表單中可以捕獲建立問題的用戶的經理的姓名。 當您要捕獲建立任務、項目、項目組合的用戶的經理的姓名時，該過程是相同的。

1. 建立問題自定義表單並向其添加計算欄位。

   有關建立自定義表單和向其添加計算欄位的資訊，請參閱以下文章：

   * [建立或編輯自定義表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [將計算資料添加到自定義窗體](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. 將以下文本模式代碼複製並貼上到 **計算** 自定義窗體的欄位：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >自定義欄位計算區分大小寫。

1. 按一下 **完成**，則 **保存+關閉**。

   建立問題的用戶的經理在包含該欄位的表單附加到問題時顯示在計算欄位中。
