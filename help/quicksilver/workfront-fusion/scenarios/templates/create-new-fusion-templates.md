---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中建立新範本 [!DNL Adobe Workfront Fusion]
description: 您可以在中建立新的情境範本 [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: f3f34e807228b299c0570e63bdf329f4e20e0340
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 在中建立新範本 [!DNL Adobe Workfront Fusion]

您可以在中建立新的情境範本 [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>建立新範本之前，您可以檢查 [!UICONTROL 公用範本] 索引標籤來確保您想要建立的範本尚無法使用。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 工作自動化與整合]，請參閱[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 建立新範本

您可以使用與建立情境類似的程式來建立範本。 Fusion管理員也可以從現有的案例建立範本。

* [建立範本](#build-a-template)
* [從情境建立範本](#create-a-template-from-a-scenario)

### 建立範本

1. 按一下 **[!UICONTROL 範本]** ![](assets/fusion-template-icon.png) ，位於左側導覽面板中。
1. 按一下 **[!UICONTROL 建立新範本]** 位於右上角。
1. （可選）取代預設值來重新命名範本 **[!UICONTROL 新範本名稱]** 左上角。
1. （可選）若要變更範本的語言，請按一下 **[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png) 並從語言下拉式清單中選取語言。

   >[!IMPORTANT]
   >
   >「語言」選項對應於系統設定中可用的語言，並且只與公用範本的名稱及其說明有關。 一旦範本已儲存，您就無法變更範本語言。

1. （選擇性）若要輸入範本的說明，請按一下 **[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png) 並輸入說明。
1. 以建立標準情境時的相同方式新增應用程式、模組和工具。

   若要將內容說明新增至模組，請參閱 [設定 [!UICONTROL 精靈] 功能](#set-up-wizard-functionality) 本文章內容。

   如需建立情境的詳細資訊，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >如果您的範本包含需要新增連線、憑證或其他隱私權敏感資訊的模組，則此資訊不會與範本使用者共用。

1. （選用）按一下 **[!UICONTROL 執行一次]** 以測試您的範本。
1. 按一下 **[!UICONTROL 儲存]** 圖示 ![](assets/save-icon.png).

>[!NOTE]
>
>儲存您的範本後，您便可讓所有專案團隊成員看到該範本。 如果您希望範本可在團隊外部存取，您必須提交請求以核准並發佈。 請求會進入Adobe Workfront進行核准，並在獲得核准後，團隊以外的其他人即可存取範本。
>
>如需有關發佈範本的資訊，請參閱 [發佈和共用 [!DNL Adobe Workfront Fusion] 範本](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### 從情境建立範本

>[!NOTE]
>
>您必須是Fusion管理員才能從案例建立範本。

1. 針對您要建立案例的案例，開啟案例詳細資訊頁面。
1. 按一下 **管理員** 下拉式選單，靠近頁面的右上角。
1. 選取 **復製為範本**.

   情境會複製到新範本頁面中。
1. （可選）取代預設值來重新命名範本 **[!UICONTROL 新範本名稱]** 左上角。
1. （可選）若要變更範本的語言，請按一下 **[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png) 並從語言下拉式清單中選取語言。

   >[!IMPORTANT]
   >
   >「語言」選項對應於系統設定中可用的語言，並且只與公用範本的名稱及其說明有關。 一旦範本已儲存，您就無法變更範本語言。

1. （選擇性）若要輸入範本的說明，請按一下 **[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png) 並輸入說明。
1. 使用與編輯標準案例相同的方式來編輯應用程式、模組和工具。

   若要將內容說明新增至模組，請參閱 [設定 [!UICONTROL 精靈] 功能](#set-up-wizard-functionality) 本文章內容。

   >[!NOTE]
   >
   >如果您的範本包含需要新增連線、憑證或其他隱私權敏感資訊的模組，則此資訊不會與範本使用者共用。

1. （選用）按一下 **[!UICONTROL 執行一次]** 以測試您的範本。
1. 按一下 **[!UICONTROL 儲存]** 圖示 ![](assets/save-icon.png).

## 設定 [!UICONTROL 精靈] 功能 {#set-up-wizard-functionality}

此 [!DNL Workfront Fusion template] [!UICONTROL 精靈] 可讓您為範本的未來使用者提供與模組中所使用特定欄位相關的指示或資訊。

1. 按一下新增至範本的模組，以檢視模組的欄位。
1. 找到您要新增的欄位 [!UICONTROL 精靈] 資訊，並啟用 **[!UICONTROL 在精靈中使用]** 用於該欄位。
1. 在中，輸入您希望讓使用者可見的資訊 [!UICONTROL 說明] 欄位。
1. （選用）若要讓使用者能在使用範本時看到此文字，請啟用 **[!UICONTROL 使用作為預設值]**.
1. 針對您想要提供資訊的每個欄位，重複步驟2至4。
1. 按一下 **[!UICONTROL 確定]** 以儲存變更並關閉模組。
