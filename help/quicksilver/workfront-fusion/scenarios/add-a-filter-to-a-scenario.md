---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 將篩選器新增至中的情境 [!DNL Adobe] Workfront Fusion
description: 在某些情況下，您只需要使用符合特定條件的套件組合。 篩選可讓您選取這些組合。
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 將篩選器新增至中的情境 [!DNL Adobe Workfront Fusion]

在某些情況下，您只需要使用符合特定條件的套件組合。 篩選可讓您選取這些組合。

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

您可以在兩個模組之間新增篩選器，並檢查從先前模組收到的套件組合是否符合特定的篩選條件：

* 如果有的話，套件組合會傳遞至案例中的下一個模組。
* 如果失敗，則會終止束的處理。

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
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 若為工作自動化與整合]，[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

您必須先將兩個模組新增至情境，才能在它們之間新增篩選器。

## 在兩個模組之間新增篩選器：

1. 按一下 **[!UICONTROL 情境]** ![](assets/scenarios-icon.png) 在左側面板中，然後選取要開啟的情境。
1. 在視窗的右上角，按一下 **[!UICONTROL 編輯]**.
1. 按一下模組之間的連線線。
1. 在顯示的方塊中，輸入 **[!UICONTROL 標籤]** 用於篩選。
1. 定義篩選器 **[!UICONTROL 條件]**.

   您可以在兩個方塊中輸入一或兩個運算元。 如果在這兩個方塊中輸入運算元，則可在它們之間的下拉式選單中選取運運算元，以指定它們之間的關係。

   >[!TIP]
   >
   >在運算元欄位中，您可以像對應值一樣輸入值，如中所述 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   例如，如果您希望篩選器在中尋找檔案 [!DNL Adobe Workfront] 以XML結尾，然後將其傳遞至 [!DNL Dropbox]，您可以輸入 **[!UICONTROL 檔案名稱]** 在第一個方塊和中。**[!UICONTROL xml]** 在第二個方塊中。 在兩者之間的下拉式功能表中，您可以選取 **[!UICONTROL 結尾為（不區分大小寫）]**. 此篩選器將套用至來自第一個模組(Workfront)的傳入組合。 只有包含XML檔案的套件組合會傳遞至下一個模組([!DNL Dropbox])。

   ![](assets/set-up-filter-box-350x368.jpg)

1. 按一下 **[!DNL OK]**.

## 複製篩選器

目前，案例編輯器不包含複製篩選器的功能。

>[!NOTE]
>
>如果您複製篩選器兩側的模組，也會複製篩選器。
>
>如需複製模組的詳細資訊，請參閱 [複製模組或情境於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

若要複製篩選器而不複製模組，您可以使用 [!DNL Google] 使用Chrome進行下列因應措施：

1. 安裝 [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] 副檔名。
1. 在 [!DNL Workfront Fusion]，開啟情境。
1. 按一下Chrome三點選單，然後按一下**[!UICONTROL 更多工具*]* > **[!UICONTROL 開發人員工具]**.

1. 在 [!UICONTROL 開發人員工具] 面板，在頂端選單列上，按一下 [!UICONTROL Workfront Fusion] 標籤。

   ![](assets/copy-a-filter-350x174.png)

1. 按一下 **[!UICONTROL 工具]** 圖示 ![](assets/devtools-tools-icon.png) 在左側列中。

1. 按一下 **[!UICONTROL 複製篩選器]**，然後設定 **[!UICONTROL 複製篩選器]** 工具在右側面板中：

   1. 設定 **[!UICONTROL 來源模組]** 作為模組，緊接在您要複製的篩選之後。
   1. 設定 **[!UICONTROL 目標模組]** 作為模組，位於您要複製的篩選器之前。

1. 按一下 **[!UICONTROL 執行]**.
