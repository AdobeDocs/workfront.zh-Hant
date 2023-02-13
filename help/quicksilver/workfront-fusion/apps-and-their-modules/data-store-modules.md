---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 資料儲存模組
description: 安 [!DNL Adobe Workfront Fusion] 資料儲存類似於資料庫或簡單表，可儲存來自方案的資料，使得可以在個別方案或方案運行之間傳輸資料。 您可以在同步期間使用資料儲存來儲存來自各種系統的新資料。
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 0%

---

# [!UICONTROL 資料儲存] 模組

安 [!DNL Adobe Workfront Fusion] 資料儲存類似於資料庫或簡單表，可儲存來自方案的資料，使得可以在個別方案或方案運行之間傳輸資料。 您可以在同步期間使用資料儲存來儲存來自各種系統的新資料。

資料存放區模組可讓您新增、取代、更新、擷取、刪除、搜尋或計算 [!DNL Adobe Workfront Fusion] 資料儲存。

如需建立、編輯和疑難排解資料存放區的相關資訊，請參閱 [資料儲存於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!UICONTROL 資料儲存] 模組，您必須先建立資料存放區。

如需建立資料存放區的詳細資訊，請參閱 [資料儲存於 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL 資料儲存] 模組及其欄位

設定資料儲存模組時， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些欄位，還可能會根據應用程式或服務中的存取層級等因素顯示其他資料存放區欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

全部 [!UICONTROL 資料儲存] 模組是動作類型模組。

* [添加/替換記錄](#addreplace-a-record)
* [更新記錄](#update-a-record)
* [取得記錄](#get-a-record)
* [檢查記錄是否存在](#check-the-existence-of-a-record)
* [刪除記錄](#delete-a-record)
* [刪除所有記錄](#delete-all-records)
* [搜索記錄](#search-records)
* [計數記錄](#count-records)

### [!UICONTROL 添加/替換記錄]

此動作模組會新增或取代記錄。

您可指定資料存放區和記錄的金鑰。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

>[!NOTE]
>
>當您嘗試新增已在資料存放區中且名稱相同的記錄時，模組會擲回錯誤 [!UICONTROL 覆蓋現有記錄] 選項。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料儲存]</td> 
   <td> <p> 選取或新增您要建立記錄的資料存放區。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密鑰] </td> 
   <td> <p>輸入要模組添加或替換的記錄的唯一鍵。 該密鑰稍後可用於檢索記錄。 如果將此欄位留空，則會自動產生金鑰。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL覆蓋現有記錄] </td> 
   <td> <p>啟用此選項可覆蓋記錄。 必須在上面的「鍵」欄位中指定要覆蓋的記錄。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄] </td> 
   <td> <p>在記錄欄位中輸入所需值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新記錄]

此動作模組會更新記錄。

您可指定資料存放區和記錄的金鑰。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料儲存]</td> 
   <td> <p> 選取或新增您要建立記錄的資料存放區。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密鑰] </td> 
   <td> <p>輸入要更新模組的記錄的唯一鍵。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL插入缺少記錄] </td> 
   <td> <p>如果具有指定鍵的記錄不存在，則啟用此選項可建立新記錄。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄]</td> 
   <td> <p> 在要更新的記錄欄位中輸入所需值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 取得記錄]

此動作模組會擷取記錄。

您可指定資料存放區和記錄的金鑰。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料儲存]</td> 
   <td> <p> 選擇要從中檢索記錄的資料儲存</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密鑰] </td> 
   <td> <p>輸入要模組檢索的記錄的唯一鍵。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 檢查記錄是否存在]

此操作模組指定特定記錄是否存在。

您可指定資料存放區和記錄的金鑰。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料儲存] </td> 
   <td> <p>選擇要檢查記錄是否存在的資料儲存。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密鑰] </td> 
   <td> <p>輸入要模組檢查是否存在的記錄的唯一鍵。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除記錄]

此動作模組會刪除記錄。

您可指定資料存放區和記錄的金鑰。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料儲存] </td> 
   <td> <p>選擇要檢查記錄是否存在的資料儲存。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密鑰] </td> 
   <td> <p>輸入要刪除模組的記錄的唯一鍵。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除所有記錄]

此動作模組會刪除特定資料存放區中的所有記錄。

您可指定資料存放區。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料儲存] </td> 
   <td> <p>選擇要從中刪除所有記錄的資料儲存。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜索記錄]

此搜索模組在資料儲存區中查找與您指定的搜索查詢匹配的對象記錄。

您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料儲存]</td> 
   <td> <p> 選擇要搜索的資料儲存。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL篩選器]</p> </td> 
   <td> <p>設定搜尋的篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL排序]</p> </td> 
   <td> <p style="font-weight: normal;">對於要排序的每個欄位，填入下列欄位：</p> <p style="font-weight: bold;">[!UICONTROL密鑰]</p> <p>選擇要按結果排序的列名。</p> <p style="font-weight: bold;">[!UICONTROL順序]</p> <p>選擇要按升序還是降序排序結果。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p> 設定搜索結果的最大數量 [!DNL Workfront Fusion] 在一個執行週期中傳回。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL即使模組未返回任何結果，仍繼續執行路由]</td> 
   <td> <p> 如果啟用，即使此模組未返回任何結果，該模組所屬的路由仍會繼續處理。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 計數記錄]

此動作模組會為資料存放區中的記錄編號。

您可指定資料存放區。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL資料儲存] </td> 
   <td> <p>選擇包含要計數的記錄的資料儲存。</p> </td> 
  </tr> 
 </tbody> 
</table>
