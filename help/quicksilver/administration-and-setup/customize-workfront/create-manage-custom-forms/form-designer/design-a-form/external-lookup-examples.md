---
title: 自訂表單中的外部查詢欄位範例
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 自訂表單中的外部查詢欄位會呼叫外部API，並在下拉式欄位中傳回值作為選項。 本文提供使用外部查詢欄位來呼叫Workfront或公用API的相同例項的範例。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 101a5a80d00a8113ce31222b92f77300a5b0ce8a
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# 自訂表單中的外部查詢欄位範例

自訂表單中的外部查詢欄位會呼叫外部API，並在下拉式欄位中傳回值作為選項。 使用自訂表單附加至之物件的使用者可以從下拉式清單中選取一個或多個選項。

本文提供使用外部查詢欄位來呼叫Workfront或公用API的相同例項的範例。 您也可以使用外部查詢與外部系統（例如Jira、Salesforce或ServiceNow）通訊。

外部查詢欄位僅在新的表單設計工具中可用，不能在舊版表單產生器中使用。 如需將外部查詢欄位新增至自訂表單的詳細資訊，以及外部查詢元件的其他定義，請參閱 [使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## 為相同的Workfront執行個體設定外部查詢欄位

您可以使用外部查詢，將Workfront例項的資料匯入自訂表單。

此範例說明如何呼叫Workfront API，並將現有「狀態查詢」欄位的資料匯入外部查詢欄位。

1. 開啟自訂表單。
1. 在畫面左側，尋找 **外部查詢** 並將其拖曳至畫布上的區段。
1. 輸入 **標籤** 和 **名稱** 欄位的。
1. 選取 **格式** 欄位的。
1. 在中輸入API URL呼叫 **基本API URL** 欄位。

   * 您可以新增$$HOST來參照相同例項。
   * 您可以新增$$QUERY以根據查詢其他欄位來篩選結果。

   **範例**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. 檢閱 **相依性** 用於此查詢欄位在API中參照的欄位。

   相依性欄位可以是物件詳細資訊頁面中的任何自訂或原生欄位。

   在此範例中， `{DE:StatusQuery}` 將會取代為StatusQuery自訂欄位的值。

1. 選取 **HTTP方法**.

   這很可能 **Get**.

1. 輸入 **JSON路徑** 以從您的API呼叫取得結果。

   **範例**
   `$.data[*].name`

   >[!NOTE]
   >
   >**頁首** 呼叫同一個Workfront執行個體不需要資訊。

1. 按一下 **套用**.

   ![以自訂表單設定Workfront的API呼叫](assets/external-lookup-to-workfront.png)

   將自訂表單新增到Workfront物件（在此範例中為專案）時，它會看起來類似這樣。

   ![具有外部查詢欄位的自訂表單](assets/external-lookup-project-status-example1.png)

   ![基於狀態的外部查詢選項](assets/external-lookup-project-status-example2.png)

## 設定公用API的外部查詢欄位

您可以使用外部查詢來呼叫外部公用API並擷取資料。

此範例說明如何呼叫國家的API (例如 <https://api.first.org/data/v1/countries>)，因此您不必在下拉式選項中硬式編碼所有國家/地區名稱。

1. 開啟自訂表單。
1. 在畫面左側，尋找 **外部查詢** 並將其拖曳至畫布上的區段。
1. 輸入 **標籤** 和 **名稱** 欄位的。
1. 選取 **格式** 欄位的。
1. 在中輸入API URL呼叫 **基本API URL** 欄位。

   * 您可以新增$$QUERY以針對一般使用者實施查詢篩選。

   **範例**
列出所有國家/地區： <https://api.first.org/data/v1/countries>

   允許使用者在下拉式欄位中搜尋任何國家/地區： <https://api.first.org/data/v1/countries?q=$$QUERY>

   允許使用者搜尋區域中的國家： <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * 可用的區域是在Workfront中的獨立自訂欄位中定義。
   * 當使用者在表單上選取區域時，外部查詢欄位只會顯示該區域的國家（在API中定義哪個國家/地區）。 使用者也可以在選取的區域中搜尋國家/地區。

1. 檢閱 **相依性** 用於此查詢欄位在API中參照的欄位。

   相依性欄位可以是物件詳細資訊頁面中的任何自訂或原生欄位。

   在此範例中， `{DE:Region}` 將會取代為區域自訂欄位的值。

1. 選取 **HTTP方法**.

   這很可能 **Get**.

1. 輸入 **JSON路徑** 以從您的API呼叫取得結果。

   此選項允許從API URL傳回的JSON擷取資料。 這可當作選取要讓JSON內的哪些值出現在下拉選項中的方式。

   **範例**
   `$.data[*].country`

1. （選用）按一下 **新增頁首**，然後輸入或貼上使用API驗證所需的金鑰值組。

   >[!NOTE]
   >
   >標題欄位不是儲存認證的安全位置，您應該注意輸入和儲存的內容。

1. （選用）選取 **多選下拉式清單** 以讓使用者在下拉式清單中選取多個值。

1. 按一下 **套用**.

   ![以自訂表單設定公開API的API呼叫](assets/external-lookup-to-api-for-countries.png)

   將自訂表單新增到Workfront物件（在此範例中為專案）時，它會看起來類似這樣。

   ![具有外部查詢欄位的自訂表單](assets/external-lookup-countries-example1.png)

   ![根據地區的國家/地區的外部查閱選項](assets/external-lookup-countries-example2.png)
