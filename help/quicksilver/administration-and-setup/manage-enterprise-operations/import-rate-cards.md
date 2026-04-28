---
user-type: administrator
product-area: system-administration;setup
title: 從範本匯入費率卡
description: 您可以使用範本檔案在Excel中建置您的比率卡，並將其匯入Adobe Workfront。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: debe90e7-08c2-4385-96fb-8d349dec6741
source-git-commit: aa774419e65e9e4a5785382d3cb2b22bdb0389c9
workflow-type: tm+mt
source-wordcount: '1812'
ht-degree: 1%

---

# 從範本匯入費率卡

您可以使用範本檔案在Excel中建立您的費率卡片，並將其匯入Adobe Workfront，而非手動新增所有工作角色和費率。

若要檢視本文中描述的費率卡範例，請下載[範例檔案](assets/rate-cards-sample.zip)。

如需有關費率卡的詳細資訊，請參閱[管理費率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

## 使用範本檔案的重要規則

* 輸入「職務角色」或「非人工資源分類」，但不可同時輸入兩者。
* RATE_RTCRD標籤上的「費率卡順序」必須符合RTCRD標籤上的卡順序（第一為1，第二為2，依此類推）。
* 「開始日期」和「結束日期」必須遵循允許的格式。
* 費率卡片可以在不提供費率的情況下匯入，並稍後更新。
* 自訂屬性（機構、成本中心等） 可能有所不同。 請洽詢您的系統管理員以瞭解確切的需求。
* 在範本中刪除的列將不會刪除系統中的現有記錄。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL標準]</td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>編輯[！UICONTROL費率卡]的存取權</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 填寫範本檔案

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 按一下&#x200B;**新費率卡**，然後按一下&#x200B;**下載Excel範本**。
1. 按照瀏覽器提示將範本檔案儲存到您的電腦。
1. 在Excel中開啟範本檔案。

   >[!TIP]
   >
   > 如果要保留空白的範本檔案，請以新名稱儲存檔案，稍後再使用。

   範本有兩個標籤。 兩個頁標都必須有正確的資訊，才能成功匯入費率卡。

   * RTCRD：定義費率卡（基本資訊）
   * RATE_RTCRD：定義與每個費率卡相關的詳細費率

### 填寫RTCRD （費率卡設定）標籤

建立並列出此標籤上的所有費率卡。 每一列代表一張費率卡。

![RTCRD索引標籤在費率卡匯入範本檔案上](assets/rate-card-import-template-tab1.png)

1. 在每一列輸入費率卡的資訊：

   * **名稱** （必要）：費率卡的名稱，例如「2025年全域帳單」。

     此名稱是費率卡的主要識別碼。 每個費率卡必須有唯一的名稱。

   * **描述** （選擇性）：費率卡的自由格式文字描述。 以此說明目的、範圍或有效性，例如「適用於北美專案」。
   * **公司** （選用）：這可以是公司名稱或公司ID。 匯入將會識別兩者。

     範例： Coffesta，或&#x200B;_68c0234e00000541dd8c0757723daa68_

   * **群組** （選用）：這可以是群組名稱或群組識別碼。 匯入將會識別兩者。

     範例：行銷，或&#x200B;_68c0234e00000541dd8c0757723daa68_

   * **自訂欄位** （選擇性）：如果您的環境有特定要求，您可以新增具有自訂欄位名稱的其他欄。

   >[!NOTE]
   >
   >* 您至少必須輸入每張費率卡的「名稱」。
   >* 系統會根據各費率卡的列位置，自動為每個費率卡指定序號。 例如，您定義的第一個費率卡（在列2中）是序列1，下一個是2，依此類推。 這些序號在RATE_RTCRD頁標中用於附加費率。

### 填寫RATE_RTCRD （匯率設定）頁標

定義屬於此標籤上之費率卡的所有費率。

標籤上的每一列都會定義一個特定比率。 您可以重複費率卡順序，在相同費率卡下建立多個費率。

請確認日期不會重疊，除非是您有意為之。

![費率卡匯入範本檔案上的RATE_RTCRD標籤](assets/rate-card-import-template-tab2.png)

1. 在每一資料列輸入費率資訊：

   * **名稱** （必要）：費率列的標籤。

     最佳實務是重複使用費率卡名稱以清楚明瞭，例如「2025年全球計費 — 開發人員費率」。

   * **費率卡參考** （必要）：此費率所屬的費率卡序號。

     如果費率卡是您在RTCRD標籤（列2）上列出的第一個費率卡，請輸入1。 如果是第二個，請輸入2，依此類推。

   * **工作角色** （若未使用非人工資源分類則為必要）：比率套用的工作角色。 這可以是工作角色名稱或工作角色ID。 匯入將會識別兩者。

     範例： Designer或&#x200B;_68c0234e00000541dd8c0757723daa68_

   * **非人工資源分類** （若未使用工作角色，則為必要）：比率套用的非人工資源分類。 這可以是類別名稱或類別ID。 匯入將會識別兩者。

     範例：相機或&#x200B;_68c0234e00000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >您無法同時在&#x200B;**工作角色**&#x200B;與&#x200B;**非人工資源類別**&#x200B;欄中輸入資料。 需要一個。

   * **開始日期** （選用）：費率生效的日期。

     日期必須符合其中一個支援的格式（視您的位置而定）： MM/dd/yyyy， dd/MM/yyyy， MM/DD/YY， DD/MM/YY， M/d/yy， d/M/yy， yyyy/MM/dd， yyyy/dd/mm， yyyy-MM-dd， yyyyy-MM-dd， yyyyy-dd-MM

     範例： 01/01/2025

     如需詳細資訊，請參閱下方的[日期格式需求](#date-formatting-requirements)。

   * **結束日期** （選用）：費率停止生效的日期。

     此日期必須與開始日期遵循相同的支援格式。

     如需詳細資訊，請參閱下方的[日期格式需求](#date-formatting-requirements)。

   * **值** （選用）：數字比率值，例如150。 預設值為 0。
   * **貨幣** （選用）：匯率的貨幣，例如USD、EUR、GBP。 預設值為系統貨幣。
   * **已鎖定** （選擇性）：指出速率是否已鎖定。 有效值為True或False。
   * **屬性** （選用/自訂）：最後一欄（機構、地點、成本中心等） 是因客戶組態而異的費率屬性。 這些是可自訂的欄位，可能因客戶環境而異。

     範例： Agency = &quot;1： Agency， Location = &quot;Chicago，&quot; Cost Center = &quot;22： Cost Center&quot;

### 填寫RSALS （費率卡別名）標籤

建立並列出此標籤上的所有別名。 每一列代表一個別名。

將費率卡附加至專案時，別名會出現在預留位置指派、費用和報表等資訊中，而不是內部工作角色名稱。 在單一比率卡中，每個工作角色和屬性組合只能有一個別名。

別名會新增至系統，但並未根據此標籤上的資訊連線至工作角色。

費率卡匯入範本檔案上的![RSALS標籤](assets/rsals-tab-rate-card-import.png)

1. 在每一列輸入別名的名稱。

   每列只輸入一個別名：職務角色別名、非人工資源分類別名或費用型別別名。

### 填寫RCRMET_RTCRD_RSALS （費率卡中繼資料）標籤

On this tab you can define the connections between resources and aliases for a specific rate card.

![RCRMET_RTCRD_RSALS tab on rate card import template file](assets/rcrmet-tab-rate-card-import.png)

1. Enter the information on each row:

   * **Rate Card** (required): The name or the sequence number of the rate card that the resource and alias belong to. The rate card must be listed on the RTCRD tab.

     For a sequence number: If the rate card was the first one you listed on the RTCRD tab (row 2), enter 1. 如果是第二個，請輸入2，依此類推。

   * **Job Role** (required if Expense Type and Non-Labor Resource Category are not used): The job role that the alias is connected to. 這可以是工作角色名稱或工作角色ID。 匯入將會識別兩者。

     範例： Designer或&#x200B;_68c0234e00000541dd8c0757723daa68_

   * **Expense Type** (required if Job Role and Non-Labor Resource Category are not used): The expense type that the alias is connected to. This can be either the expense type name or the expense type ID. 匯入將會識別兩者。

     Example: Travel or _68c0234e00000541dd8c0757723daa68_

   * **Non-Labor Resource Category** (required if Job Role and Expense Type are not used): The non-labor resource category that the alias is connected to. 這可以是類別名稱或類別ID。 匯入將會識別兩者。

     範例：相機或&#x200B;_68c0234e00000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >You cannot enter all three of the **Job Role**, **Expense Type**, and **Non-Labor Resource Category** columns. 需要一個。

   * **Resource Alias**: The alias entered on the RSALS tab.

### Date formatting requirements

When preparing rate card data for importing, you must ensure that the date columns are formatted as **General**, not as **Date**.

If the columns are set to Date format, the system may misinterpret values during the import process, leading to errors or failed uploads. 使用一般格式會保留日期的原始數值或文字表示，讓系統正確驗證並套用值。

遵循這些步驟將可避免不必要的問題，並確保順利且準確地匯入比率資料。

1. 在儲存或上傳檔案之前，請選取試算表中的日期欄。
1. 將資料行格式變更為&#x200B;**一般**。
1. 確認值仍正確顯示（例如，01/01/2025或2025-01-01）。

## 匯入範本檔案

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 按一下&#x200B;**新費率卡**，然後按一下&#x200B;**匯入新費率卡**。
1. 將您的檔案拖放到對話方塊中，或按一下&#x200B;**選取Excel檔案**&#x200B;以瀏覽電腦上的檔案。
1. 按一下&#x200B;**開始匯入**。

   如果檔案沒有問題，則會顯示確認訊息，且新費率卡會出現在清單中。

1. 如果檔案包含問題，則會顯示錯誤訊息。 按一下「**檢視問題**」，在個別的熒幕上檢視問題。

   您必須更正Excel檔案中的問題並再次匯入，費率卡才會存在於Workfront中。

## 更新現有的費率卡

您可以使用相同的Excel範本更新現有費率卡中的費率，並將這些變更上傳至Workfront。

更新現有匯率時，只需要RATE_RTCRD （匯率設定）頁標。

>[!NOTE]
>
>上傳現有費率卡的費率會覆寫費率卡上所有目前的工作角色和費率。
>
>例如，如果您現有費率卡上有5個具有費率的工作角色，而Excel檔案有1個工作角色，則上傳後，費率卡會有1個工作角色。 若要將其他5個工作角色及其費率保留在費率卡上，您必須將其納入Excel檔案中。

若要更新現有的費率卡，請執行下列步驟：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 按一下&#x200B;**新費率卡**，然後按一下&#x200B;**匯入費率卡更新**。
1. 將您的檔案拖放到對話方塊中，或按一下&#x200B;**選取Excel檔案**&#x200B;以瀏覽電腦上的檔案。
1. 按一下&#x200B;**開始匯入**。

   如果檔案沒有問題，則會顯示確認訊息，且新費率卡會出現在清單中。

1. 如果檔案包含問題，則會顯示錯誤訊息。 按一下「**檢視問題**」，在個別的熒幕上檢視問題。

   您必須更正Excel檔案中的問題並再次匯入，費率卡更新才會存在於Workfront中。


