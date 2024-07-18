---
content-type: reference
product-area: reporting
keywords: 稽核，追蹤，自訂，欄位
navigation-topic: calculate-custom-data-reports
title: 「計算自訂欄位範例：顯示欄位的編輯歷史記錄」
description: 如果使用者定期更新自訂欄位，而您想要擷取對欄位進行的所有變更的記錄以及變更發生的日期，則可以在計算的自訂欄位中擷取此資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# 計算自訂欄位範例：顯示欄位的編輯歷史記錄

如果使用者定期更新自訂欄位，而您想要擷取對欄位進行的所有變更的記錄以及變更發生的日期，則可以在計算的自訂欄位中擷取此資訊。

下列範例說明如何建置&#x200B;*指示編輯歷史記錄*&#x200B;計算欄位，以擷取對名為&#x200B;*指示*&#x200B;的單行文字欄位所做的所有變更。

>[!TIP]
>
>您可以依照此範例，使用所有型別的自訂欄位，而不只是單行文字欄位。

這會執行下列動作： 

* 將&#x200B;*指示編輯歷史記錄*&#x200B;欄位限製為最近2000個字元，以保持在Workfront資料庫限制內。
* 檢查&#x200B;*指示*&#x200B;欄位的目前值是否與&#x200B;*指示編輯歷史記錄*&#x200B;值的前端相符；它會假設為空白，如果不是，則會執行下列動作： 

   * 如果兩者相符，則會將&#x200B;*指示編輯歷史記錄*&#x200B;保留不變；
   * 如果兩者不符，會將&#x200B;*指示編輯歷史記錄*&#x200B;取代為&#x200B;*指示*&#x200B;欄位中的最新值，後面接著括弧中的目前日期、垂直列，以及先前的&#x200B;*指示編輯歷史記錄*，這會保留先前的值和輸入時的日期。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。</p> 
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
   <td><strong>存取層級設定*</strong> </td> 
   <td> <p>自訂Forms的管理存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>物件許可權</strong> </p> </td> 
   <td> <p>管理自訂表單的許可權 </p> <p>如需詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共用自訂表格</a>。<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## 先決條件

若要將顯示欄位編輯歷史記錄的計算欄位新增至自訂表單，您必須先：

* 建立自訂表單
* 將您要擷取其記錄的欄位新增至自訂表單

## 顯示欄位的編輯歷史記錄

1. 前往您要新增計算欄位的自訂表單。

1. 例如，若要建立單行文字自訂欄位，請執行下列動作：

   1. 按一下&#x200B;**單行文字欄位**。
   1. 指定自訂欄位的&#x200B;**標籤**，例如&#x200B;*指示*。
   1. 按一下&#x200B;**套用**。

1. 選取&#x200B;**新增欄位**，然後選取&#x200B;**已計算**&#x200B;以將已計算的自訂欄位新增至表單。
1. 指定計算自訂欄位的&#x200B;**標籤**，例如&#x200B;*指示編輯歷程記錄*。

   此欄位會擷取對您建立的第一個欄位所做的任何變更（*指示*）。

1. 按一下「**儲存並關閉**」。
1. 按一下已新增兩個欄位的表單名稱，以重新開啟。
1. 按一下計算自訂欄位&#x200B;*指示編輯歷程記錄，*，然後將下列內容複製並貼到計算方塊中：
1. 在&#x200B;**計算**&#x200B;欄位中，為您的自訂欄位指定下列計算：

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. （建議）將相同的計算貼到表單上計算欄位的&#x200B;**指示**&#x200B;欄位中。
1. 請確定  已在&#x200B;**格式**&#x200B;欄位中選取&#x200B;**文字**，以將計算的自訂欄位格式化為文字。

   這是預設值。

1. 按一下&#x200B;**儲存+關閉**。

   現在，當您將自訂表單附加到物件，然後有人在&#x200B;*指示*&#x200B;欄位中變更資訊時，*指示編輯歷程記錄」欄位會顯示最新值，後面接著括弧中的目前日期，以及垂直列。 若有進一步的變更，則會以相同的方式新增至此資訊。

   在上述計算中，您可以將&#x200B;*指示*&#x200B;取代為您要追蹤其歷程記錄的單行文字欄位的確切名稱，並將&#x200B;*指示編輯歷程記錄*&#x200B;取代為您計算欄位的確切名稱。
