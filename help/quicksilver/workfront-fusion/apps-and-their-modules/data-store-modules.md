---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 資料存放區模組
description: ' [!DNL Adobe Workfront Fusion] 資料存放區（類似資料庫或簡單表格）可儲存案例的資料，因此可在個別案例或案例執行之間傳輸資料。 您可以在同步期間使用資料存放區來儲存來自不同系統的新資料。'
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---

# [!UICONTROL 資料存放區]模組

[!DNL Adobe Workfront Fusion]資料存放區（類似資料庫或簡單表格）可以儲存案例的資料，因此可以在個別案例或案例執行之間傳輸資料。 您可以在同步期間使用資料存放區來儲存來自不同系統的新資料。

資料存放區模組可讓您新增、取代、更新、擷取、刪除、搜尋或計算[!DNL Adobe Workfront Fusion]資料存放區中的記錄。

如需有關建立、編輯和疑難排解資料存放區的資訊，請參閱[資料存放區位於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

如需有關Workfront Fusion中資料存放區的影片簡介，請參閱：

* [資料存放區](https://video.tv.adobe.com/v/3427029/){target=_blank}

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要使用[!UICONTROL 資料存放區]模組，您必須先建立資料存放區。

如需建立資料存放區的資訊，請參閱[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)中的[資料存放區

## [!UICONTROL 資料存放區]模組及其欄位

當您設定資料存放區模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除此之外，其他資料存放區欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

所有[!UICONTROL 資料存放區]模組都是動作型別模組。

* [新增/取代記錄](#addreplace-a-record)
* [更新記錄](#update-a-record)
* [取得記錄](#get-a-record)
* [檢查記錄是否存在](#check-the-existence-of-a-record)
* [刪除記錄](#delete-a-record)
* [刪除所有記錄](#delete-all-records)
* [搜尋記錄](#search-records)
* [計算記錄](#count-records)

### [!UICONTROL 新增/取代記錄]

此動作模組新增或取代記錄。

您可以指定資料存放區和記錄的索引鍵。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

>[!NOTE]
>
>當您嘗試以相同名稱新增資料存放區中的記錄時，模組擲回錯誤，且[!UICONTROL 覆寫現有記錄]選項已停用。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料存放區]</td> 
   <td> <p> 選取或新增要建立記錄的資料存放區。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>輸入您要模組新增或取代之記錄的唯一索引鍵。 此金鑰稍後可用於擷取記錄。 如果您將此欄位留空，則會自動產生索引鍵。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL覆寫現有記錄] </td> 
   <td> <p>啟用此選項以覆寫記錄。 您必須在上方的[索引鍵]欄位中指定您要覆寫的記錄。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄] </td> 
   <td> <p>在記錄的欄位中輸入所需的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新記錄]

此動作模組會更新記錄。

您可以指定資料存放區和記錄的索引鍵。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料存放區]</td> 
   <td> <p> 選取或新增要建立記錄的資料存放區。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>輸入您要模組更新的記錄唯一索引鍵。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL插入遺漏的記錄] </td> 
   <td> <p>啟用此選項以在指定索引鍵的記錄不存在時建立新記錄。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄]</td> 
   <td> <p> 在您要更新的記錄欄位中輸入所需的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 取得記錄]

此動作模組會擷取記錄。

您可以指定資料存放區和記錄的索引鍵。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料存放區]</td> 
   <td> <p> 選取您要從中擷取記錄的資料存放區</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>輸入您要模組擷取之記錄的唯一索引鍵。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 檢查記錄是否存在]

此動作模組會指定特定記錄是否存在。

您可以指定資料存放區和記錄的索引鍵。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料存放區] </td> 
   <td> <p>選取您要檢查記錄是否存在的資料存放區。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>輸入您要模組檢查其是否存在之記錄的唯一索引鍵。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除記錄]

此動作模組會刪除記錄。

您可以指定資料存放區和記錄的索引鍵。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料存放區] </td> 
   <td> <p>選取您要檢查記錄是否存在的資料存放區。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Key] </td> 
   <td> <p>輸入您要模組刪除之記錄的唯一關鍵值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除所有記錄]

此動作模組會從特定資料存放區中刪除所有記錄。

您可以指定資料存放區。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料存放區] </td> 
   <td> <p>選取要刪除所有記錄的資料存放區。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜尋記錄]

此搜尋模組會在資料存放區中尋找符合您指定之搜尋查詢的物件記錄。

您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料存放區]</td> 
   <td> <p> 選取您要搜尋的資料存放區。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL篩選器]</p> </td> 
   <td> <p>設定搜尋的篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL排序]</p> </td> 
   <td> <p style="font-weight: normal;">針對您要排序的每個欄位，填寫以下欄位：</p> <p style="font-weight: bold;">[！UICONTROL Key]</p> <p>選取要作為結果排序依據的欄名稱。</p> <p style="font-weight: bold;">[！UICONTROL順序]</p> <p>選取您要以遞增或遞減順序排序結果。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p> 設定在一個執行週期內傳回的搜尋結果數目上限[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL即使模組未傳回任何結果，仍繼續執行路由]</td> 
   <td> <p> 如果啟用，即使此模組未傳回任何結果，此模組所屬的路由仍會繼續處理。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 記錄數]

此動作模組對資料存放區中的記錄進行編號。

您可以指定資料存放區。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL資料存放區] </td> 
   <td> <p>選取包含您要計算之記錄的資料存放區。</p> </td> 
  </tr> 
 </tbody> 
</table>
