---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中建立新範本 [!DNL Adobe Workfront Fusion]
description: 您可以在 [!DNL Adobe] Workfront聚變。
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 在中建立新範本 [!DNL Adobe Workfront Fusion]

您可以在 [!DNL Adobe] Workfront聚變。

>[!TIP]
>
>建立新範本之前，您可以檢查 [!UICONTROL 公用範本] 頁簽，確保您要建立的模板尚未可用。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

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
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化） </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 建立新範本

1. 按一下 **[!UICONTROL 範本]** ![](assets/fusion-template-icon.png) ，即可取得Advertising Cloud的說明。
1. 按一下 **[!UICONTROL 建立新範本]** 在右上角。
1. （選用）取代預設值，重新命名範本 **[!UICONTROL 新範本名稱]** 在左上角。
1. （可選）若要變更範本的語言，請按一下 **[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png) 並從「語言」下拉式清單中選取語言。

   >[!IMPORTANT]
   >
   >「語言」選項與系統設定中可用的語言相對應，只涉及公共模板的名稱及其說明。 儲存範本後，就無法變更範本語言。

1. （可選）若要輸入範本說明，請按一下 **[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png) 並輸入說明。
1. 以與建立標準案例相同的方式新增應用程式、模組和工具。

   若要將內容說明新增至模組，請參閱 [設定 [!UICONTROL 精靈] 功能](#set-up-wizard-functionality) 這篇文章。

   如需建立案例的詳細資訊，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >如果您的範本包含需要新增連線、認證或其他隱私權相關資訊的模組，則此資訊不會與範本使用者共用。

1. （選用）按一下 **[!UICONTROL 執行一次]** 來測試範本。
1. 按一下 **[!UICONTROL 儲存]** 圖示 ![](assets/save-icon.png).

>[!NOTE]
>
>通過保存模板，可使所有團隊成員都可見。 如果您希望範本可在團隊外部存取，則需要發佈該範本，然後使用共用連結，或要求管理員核准並發佈範本。

## 設定 [!UICONTROL 精靈] 功能 {#set-up-wizard-functionality}

此 [!DNL Workfront Fusion template] [!UICONTROL 精靈] 可讓您為未來的範本使用者提供與模組中使用的特定欄位相關的指示或資訊。

1. 按一下新增至範本的模組，以查看模組的欄位。
1. 找出您要新增的欄位 [!UICONTROL 精靈] 資訊，並啟用 **[!UICONTROL 在嚮導中使用]** 那塊地。
1. 在 [!UICONTROL 說明] 欄位。
1. （可選）若要讓使用者在使用範本時看到此文字，請啟用 **[!UICONTROL 使用作為預設值]**.
1. 對要提供資訊的每個欄位重複步驟2-4。
1. 按一下 **[!UICONTROL 確定]** 儲存變更並關閉模組。
