---
content-type: reference
product-area: reporting
keywords: 審核，跟蹤，自定義，欄位
navigation-topic: calculate-custom-data-reports
title: '"計算自訂欄位範例：顯示欄位的編輯歷史記錄」'
description: 如果使用者定期更新自訂欄位，而您想要擷取對欄位所做所有變更的記錄，以及變更發生的日期，則您可以在計算的自訂欄位中擷取此資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# 計算的自訂欄位範例：顯示欄位的編輯歷史記錄

如果使用者定期更新自訂欄位，而您想要擷取對欄位所做所有變更的記錄，以及變更發生的日期，則您可以在計算的自訂欄位中擷取此資訊。

下列範例會示範如何建立 *說明編輯歷史記錄* 計算欄位，擷取對名為的單行文字欄位所做的所有變更 *說明*.

>[!TIP]
>
>您可以針對所有類型的自訂欄位遵循此範例，而不只是單行文字欄位。

這會執行下列動作： 

* 限制 *說明編輯歷史記錄* 欄位中填入2000個字元，以保留在Workfront資料庫限制內。
* 檢查 *說明* 欄位與 *說明編輯歷史記錄* 值；此變數假設為空白，若非空白，則會執行下列動作： 

   * 如果兩者相符，則會離開 *說明編輯歷史記錄* 原樣；
   * 如果不相符，則會取代 *說明編輯歷史記錄* 的 *說明* 欄位，後跟括弧中的目前日期、垂直條和上一個 *說明編輯歷史記錄*，可保留先前值和輸入日期。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront授權*</p> </td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>管理存取自訂Forms</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>管理自訂表單的權限 </p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共用自訂表單</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## 必要條件

若要將顯示欄位編輯歷史記錄的計算欄位新增至自訂表單，您必須先：

* 建立自訂表單
* 將您要擷取其歷史記錄的欄位新增至自訂表單

## 顯示欄位的編輯歷史記錄

1. 移至您要新增計算欄位的自訂表單。

1. 例如，要建立單行文本自定義欄位，請執行以下操作：

   1. 按一下 **單行文本欄位**.
   1. 指定 **標籤** (例如 *說明*.
   1. 按一下 **阿普利耶**.

1. 選擇 **新增欄位**，然後選取 **計算** 新增計算的自訂欄位至表單。
1. 指定 **標籤** ，例如 *說明編輯歷史記錄*.

   這是欄位，會擷取對您建立的第一個欄位(*說明*)。

1. 按一下 **儲存+關閉**.
1. 按一下您已新增兩個欄位以重新開啟的表單名稱。
1. 按一下計算的自訂欄位 *說明編輯歷史記錄，* 然後複製並貼到「計算」方塊中：
1. 在 **計算** 欄位，為自訂欄位指定下列計算：

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. （建議）將相同的計算貼入 **說明** 欄位（在表單的計算欄位上）。
1. 確保  **文字** 在 **格式** 欄位，將計算的自訂欄位格式為文字。

   這是預設值。

1. 按一下 **儲存並關閉**.

   現在，當您將自訂表單附加至物件，然後有人變更 *說明* 欄位中，*Instructions Edit History」欄位會顯示最新值，後面跟括弧中的目前日期，並加上垂直條。 如果進行了進一步的變更，則會以相同方式將其新增至此資訊。

   在上述計算中，您可以取代 *說明* 包含您要追蹤其歷史記錄的單行文字欄位的確切名稱，以及 *說明編輯歷史記錄* 填入計算欄位的確切名稱。
