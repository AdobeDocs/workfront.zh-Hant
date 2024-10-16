---
title: 自訂表單中的外部查詢欄位範例
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 自訂表單中的外部查詢欄位會呼叫外部API，並在下拉欄位中傳回值作為選項。 本文提供使用外部查詢欄位來呼叫Workfront或公用API的相同例項的範例。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 7a1df83c0dd7ddf7dd6cf41643ba65c5903d6eba
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 0%

---

# 自訂表單中的外部查詢欄位範例

自訂表單中的外部查詢欄位會呼叫外部API，並在下拉欄位中傳回值作為選項。 使用自訂表單附加至之物件的使用者可以從下拉式清單中選取一個或多個選項。

本文提供使用外部查詢欄位來呼叫Workfront或公用API的相同例項的範例。 您也可以使用外部查詢與外部系統(例如Jira、Salesforce或ServiceNow)通訊。

如需將外部查閱欄位新增至自訂表單的詳細資訊，以及外部查閱元件的其他定義，請參閱[使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 為相同的Workfront執行個體設定外部查詢欄位

您可以使用外部查詢功能，將Workfront例項的資料匯入自訂表單中。

### 在外部查詢中使用原生Workfront欄位值

此範例說明如何呼叫Workfront API，並將現有「狀態查詢」欄位的資料匯入外部查詢欄位。

1. 開啟自訂表單。
1. 在熒幕左側，尋找&#x200B;**外部查詢**&#x200B;並將其拖曳至畫布上的區段。
1. 輸入欄位的&#x200B;**標籤**&#x200B;和&#x200B;**名稱**。
1. 選取欄位的&#x200B;**格式**。
1. 在&#x200B;**基本API URL**&#x200B;欄位中輸入API呼叫。

   * 若要參照自訂表單所在的相同Workfront例項，請在URL使用$$HOST。
   * 若要根據查詢其他欄位來篩選結果，請新增$$QUERY。

   **範例**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. 檢閱此查詢欄位在API中參考的欄位的&#x200B;**相依性**。

   相依性欄位可以是物件詳細資訊頁面中的任何自訂或原生欄位。

   在此範例中，`{DE:StatusQuery}`將由StatusQuery自訂欄位的值取代。

1. 選取&#x200B;**HTTP方法**。

   這很可能是&#x200B;**Get**。

1. 輸入&#x200B;**JSON路徑**&#x200B;以取得API呼叫的結果。

   **範例**
   `$.data[*].name`

   >[!NOTE]
   >
   >**標題**&#x200B;資訊不是呼叫相同Workfront執行個體的必要專案。

1. 按一下&#x200B;**套用**。

   ![以自訂表單設定API呼叫Workfront](assets/external-lookup-to-workfront.png)

   將自訂表單新增到Workfront物件（在此範例中為專案）時，它會看起來類似這樣。

   ![具有外部查閱欄位的自訂表單](assets/external-lookup-project-status-example1.png)

   根據狀態的![外部查閱選項](assets/external-lookup-project-status-example2.png)

### 在外部查詢中使用自訂欄位值

此範例顯示如何呼叫Workfront API，並將自訂欄位的資料匯入外部查詢欄位。 範例自訂欄位稱為「自訂顏色」。

1. 開啟自訂表單。
1. 在熒幕左側，尋找&#x200B;**外部查詢**&#x200B;並將其拖曳至畫布上的區段。
1. 輸入欄位的&#x200B;**標籤**&#x200B;和&#x200B;**名稱**。
1. 選取欄位的&#x200B;**格式**。
1. 在&#x200B;**基本API URL**&#x200B;欄位中輸入API URL呼叫。

   **範例**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. 檢閱此查詢欄位在API中參考的欄位的&#x200B;**相依性**。

   相依性欄位可以是物件詳細資訊頁面中的任何自訂或原生欄位。

1. 選取&#x200B;**HTTP方法**。

   這很可能是&#x200B;**Get**。

1. 輸入&#x200B;**JSON路徑**&#x200B;以取得API呼叫的結果。

   **範例**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * 「parameterValues」是指Workfront中您所在物件的任何自訂欄位。
   * 在此範例中，「DE：組合顏色」是包含您要擷取之值的特定自訂欄位。

   >[!NOTE]
   >
   >**標題**&#x200B;資訊不是呼叫相同Workfront執行個體的必要專案。

1. 按一下&#x200B;**套用**。

   將自訂表單新增至Workfront物件時，「組合顏色」欄位中的所有值都會出現在外部查詢欄位下拉式清單中。

## 設定Workfront Planning API的外部查詢欄位

[Workfront Planning API](/help/quicksilver/planning/general/planning-api-basics.md)中有端點可透過Get方法依記錄型別ID搜尋記錄。 您可以使用此端點來參考外部查閱欄位中的Planning記錄。

* **基礎API URL：** `$$HOST/maestro/api/v1/records/search?recordTypeId={recordTypeID}`
* **HTTP方法：** Get
* **JSON路徑：** `$.records[*].data.{fieldID}`

  **{fieldID}**&#x200B;是要在使用者自訂表單的外部查詢搜尋結果中顯示的欄位。

## 設定公用API的外部查詢欄位

您可以使用外部查詢來呼叫外部公用API並擷取資料。

此範例說明如何呼叫國家/地區的API （例如<https://api.first.org/data/v1/countries>），如此您就不必在下拉式選項中硬式編碼所有國家/地區名稱。

1. 開啟自訂表單。
1. 在熒幕左側，尋找&#x200B;**外部查詢**&#x200B;並將其拖曳至畫布上的區段。
1. 輸入欄位的&#x200B;**標籤**&#x200B;和&#x200B;**名稱**。
1. 選取欄位的&#x200B;**格式**。
1. 在&#x200B;**基本API URL**&#x200B;欄位中輸入API URL呼叫。

   * 您可以新增$$QUERY以針對一般使用者實施查詢篩選。

   **範例**
列出所有國家： <https://api.first.org/data/v1/countries>

   允許使用者在下拉式欄位中搜尋任何國家： <https://api.first.org/data/v1/countries?q=$$QUERY>

   允許使用者搜尋區域中的國家： <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * 可用的區域是在Workfront中的獨立自訂欄位中定義。
   * 當使用者在表單上選取區域時，外部查詢欄位只會顯示該區域的國家（在API中定義哪個國家/地區）。 使用者也可以在選取的區域中搜尋國家/地區。

1. 檢閱此查詢欄位在API中參考的欄位的&#x200B;**相依性**。

   相依性欄位可以是物件詳細資訊頁面中的任何自訂或原生欄位。

   在此範例中，`{DE:Region}`將會取代為區域自訂欄位的值。

1. 選取&#x200B;**HTTP方法**。

   這很可能是&#x200B;**Get**。

1. 輸入&#x200B;**JSON路徑**&#x200B;以取得API呼叫的結果。

   此選項允許從API URL傳回的JSON擷取資料。 這可當作選取要讓JSON內的哪些值出現在下拉選項中的方式。

   **範例**
   `$.data[*].country`

1. （選擇性）按一下&#x200B;**新增標題**，然後輸入或貼上使用API驗證所需的金鑰值組。

   >[!NOTE]
   >
   >標題欄位不是儲存認證的安全位置，您應該注意輸入和儲存的內容。

1. （選擇性）選取&#x200B;**多重選取下拉式清單**&#x200B;以允許使用者在下拉式清單中選取多個值。

1. 按一下&#x200B;**套用**。

   ![設定自訂表單中公開API的API呼叫](assets/external-lookup-to-api-for-countries.png)

   將自訂表單新增到Workfront物件（在此範例中為專案）時，它會看起來類似這樣。

   ![具有外部查閱欄位的自訂表單](assets/external-lookup-countries-example1.png)

   根據地區](assets/external-lookup-countries-example2.png)國家/地區的![外部查閱選項

## 外部查詢欄位的其他使用案例

建立外部查詢有許多其他使用案例。

**使用案例：**取代自動提示欄位，因為這些欄位可能會導致報表發生問題。
**解決方案：**&#x200B;使用系統現有物件的API呼叫。

範本的基礎API URL範例，取代預先輸入欄位：
`$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**使用案例：**建立包含更多功能的下拉式欄位（例如，外部eookup欄位中有換行字元）。
**解決方案：**&#x200B;使用系統中現有物件的API呼叫，或建立新物件並使用這個物件的API呼叫。

**使用案例：**定義使用者在自訂表格區域外維護其欄位的方法。 設定「外部查詢」欄位，您可以將使用者指定給組成該欄位的物件。 此選項適合用於高維護欄位和團隊。
**解決方案：**&#x200B;建立新物件並使用這個物件的API呼叫。

**使用案例：**與Workfront外部的物件整合。 例如，存取另一個系統以取得每個使用者的名稱，而不是被限制在預先輸入欄位中。
**解決方案：** Webhook/Fusion Automation連線到其他系統。

