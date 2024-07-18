---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 「計算自訂欄位範例：在問題自訂表單上顯示問題建立者的管理員」
description: 使用計算自訂欄位，您可以在附加到問題的自訂表單上顯示問題建立者的經理名稱。 使用相同的陳述式，您可以為專案、問題和其他物件建置類似的計算欄位。
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '413'
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

您必須具有下列存取權才能執行本文中的步驟：

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
   <td>存取層級設定*</td> 
   <td> <p>對自訂表單的管理存取權<br>如需從存取層級授與管理存取權的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授與使用者對特定區域的管理存取權</a>。</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>物件許可權</p> </td> 
   <td> <p>Contribute對表單附加所在物件的存取權以及編輯自訂表單的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 在問題自訂表單上顯示問題建立者的管理員

下列步驟顯示如何為問題自訂表單建立計算欄位，您可以在其中擷取建立問題之使用者的管理員名稱。 例如，當您想要擷取建立任務、專案和投資組合之使用者的經理姓名時，程式是相同的。

1. 建立問題自訂表單，並在其中新增計算欄位。

   如需建立自訂表單及新增計算欄位的相關資訊，請參閱下列文章：

   * [建立或編輯自訂表格](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [新增計算資料至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. 將下列文字模式程式碼複製並貼到自訂表單的&#x200B;**計算**&#x200B;欄位中：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >自訂欄位計算區分大小寫。

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存+關閉**。

   當包含欄位的表單附加到問題時，建立問題的使用者的管理員顯示在計算欄位中。
