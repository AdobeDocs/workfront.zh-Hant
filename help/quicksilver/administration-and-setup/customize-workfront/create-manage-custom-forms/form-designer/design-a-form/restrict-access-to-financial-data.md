---
title: 限制存取自訂欄位中的財務資料
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 建立自訂欄位時，您可以定義選擇性設定，以限制對財務資料的存取。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3380cce6-8372-43c0-8520-473442ea0eb4
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 6%

---

# 限制存取自訂欄位中的財務資料

建立自訂欄位時，您可以定義選擇性設定，以限制對財務資料的存取。 如此一來，在存取層級中設定特定許可權的使用者便能檢視資料，且無法檢視不應存取的財務資料。

如需建立自訂欄位的詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

如需存取層級的詳細資訊，請參閱[存取層級概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。 如需關於共用和許可權的資訊，請參閱[物件共用許可權總覽](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td>任何</td> 
  </tr>  
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>管理自訂表單的存取權</td> 
  </tr>  
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 限制對自訂欄位上財務資料的存取

1. 建立新的自訂表單或開啟現有的表單。

   如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 新增自訂欄位至表單或選取現有欄位。

   可根據財務資料存取限制這些欄位型別：

   * 單行文字
   * 段落
   * 單選下拉式清單
   * 多選下拉式清單
   * 核取方塊群組
   * 選項按鈕
   * 外部查詢
   * 多選外部查詢
   * 已計算

1. 在&#x200B;**格式**&#x200B;欄位中，選取&#x200B;**貨幣**。

   >[!NOTE]
   >
   >對於計算欄位，允許任何格式。 所有其他欄位型別都必須使用&#x200B;**貨幣**&#x200B;格式，否則&#x200B;**財務許可權型別**&#x200B;欄位將無法使用。

1. （選擇性）僅針對計算欄位，開啟&#x200B;**自動許可權**&#x200B;選項以允許財務許可權自動來自公式中的欄位。

1. 選取&#x200B;**財務許可權型別**&#x200B;的選項。

   使用者必須有此財務許可權型別，才能檢視或編輯表單上的此自訂欄位。

   * **不需要許可權：**&#x200B;所有使用者都可以看到此欄位
   * **一般：**&#x200B;使用者必須具有編輯或檢視一般財務的許可權
   * **帳單：**&#x200B;使用者必須擁有編輯或檢視收費率的許可權
   * **成本：**&#x200B;使用者必須擁有編輯或檢視成本費率的許可權

   對於計算欄位：

   * 如果已開啟&#x200B;**自動許可權**&#x200B;欄位，**財務許可權型別**&#x200B;欄位將無法用於手動設定許可權。
   * 公式中使用的欄位會決定許可權欄位是否有效。 如果許可權欄位空白（並且未開啟自動許可權），則公式中的欄位不支援財務許可權。
   * 公式中所有欄位都需要存取權。 例如，如果在計算欄位中使用兩個欄位，其中一個已套用計費許可權，而另一個已套用成本許可權，則使用者必須具有檢視計費和成本費率的許可權才能檢視計算值。

1. 若要儲存您的變更，請按一下[套用] ****&#x200B;並繼續建立您的表單。

   或

   按一下&#x200B;**儲存並關閉**。

## 範例

兩個專案已與一個使用者共用：

* 使用者有權編輯第一個專案的所有財務選項
* 使用者有權檢視第二個專案的計費費率和一般財務

當使用者編輯第一個專案時，自訂表單上的所有財務欄位都是可編輯的。 當使用者編輯第二個專案時，設定為&#x200B;**帳單**&#x200B;或&#x200B;**一般**&#x200B;的欄位為僅供檢視，而設定為&#x200B;**成本**&#x200B;的欄位不可見。

當使用者檢視清單或報告中的專案時：

* 財務欄位可根據許可權和報表設定進行檢視或編輯
* 如果使用者沒有許可權檢視財務欄位，則這些欄位為空白

匯出專案詳細資料會顯示與清單相同的財務欄位值（或空白欄位）。

大量編輯這兩個專案時，帳單和一般財務欄位會顯示為唯讀，而成本欄位則顯示N/A。
