---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 將篩選器新增至案例，於 [!DNL Adobe] Workfront融合
description: 在某些情況下，您只需使用符合特定條件的套件組合。 篩選器可讓您選取這些套件組合。
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# 將篩選器新增至案例，於 [!DNL Adobe Workfront Fusion]

在某些情況下，您只需使用符合特定條件的套件組合。 篩選器可讓您選取這些套件組合。

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

您可以在兩個模組之間添加篩選器，並檢查從前面的模組接收的套件組合是否滿足特定篩選條件：

* 若有，則套件組合會傳遞至案例中的下一個模組。
* 如果沒有，套件組合的處理將終止。

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

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

您必須先將兩個模組新增至案例，才能在它們之間新增篩選器。

## 在兩個模組之間新增篩選器：

1. 按一下 **[!UICONTROL 藍本]** ![](assets/scenarios-icon.png) 在左側面板中，選取要開啟的藍本。
1. 在視窗的右上角，按一下 **[!UICONTROL 編輯]**.
1. 按一下模組之間的連接線。
1. 在顯示的方塊中，輸入 **[!UICONTROL 標籤]** 的下界。
1. 定義篩選 **[!UICONTROL 條件]**.

   您可以在兩個方塊中輸入一或兩個運算元。 如果在兩個框中輸入操作數，則可以在它們之間的下拉菜單中選擇一個運算子，以指定它們之間的關係。

   >[!TIP]
   >
   >在操作數欄位中，您可以以映射值的相同方式輸入值，如 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   例如，如果您想讓篩選器在 [!DNL Adobe Workfront] 以XML結尾，並傳遞至 [!DNL Dropbox]，您可以輸入 **[!UICONTROL 檔案名]** 和。**[!UICONTROL xml]** 在第二個方塊中。 在它們之間的下拉式功能表中，您可選取 **[!UICONTROL 結尾為（不區分大小寫）]**. 此篩選器會套用至來自第一個模組(Workfront)的傳入套件組合。 只有包含XML檔案的套件組合才會傳遞至下一個模組([!DNL Dropbox])。

   ![](assets/set-up-filter-box-350x368.jpg)

1. 按一下 **[!DNL OK]**.

## 複製篩選器

目前，案例編輯器不包含複製篩選器的功能。

>[!NOTE]
>
>如果您複製篩選器兩側的模組，也會複製篩選器。
>
>有關複製模組的詳細資訊，請參閱 [複製中的模組或方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

若要複製篩選器而不複製模組，您可以使用 [!DNL Google] Chrome提供下列因應措施：

1. 安裝 [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] 擴充功能。
1. 在 [!DNL Workfront Fusion]，開啟案例。
1. 按一下Chrome三點功能表，然後按一下**[!UICONTROL 更多工具*]* > **[!UICONTROL 開發人員工具]**.

1. 在 [!UICONTROL 開發人員工具] 面板，按一下頂端的功能表列 [!UICONTROL Workfront融合] 標籤。

   ![](assets/copy-a-filter-350x174.png)

1. 按一下 **[!UICONTROL 工具]** 圖示 ![](assets/devtools-tools-icon.png) 在左側欄。

1. 按一下 **[!UICONTROL 複製篩選]**，然後設定 **[!UICONTROL 複製篩選]** 工具的右側面板：

   1. 設定 **[!UICONTROL 來源模組]** 作為模組，緊接在您要複製的篩選器之後。
   1. 設定 **[!UICONTROL 目標模組]** 作為模組，緊接在您要複製的篩選器之前。

1. 按一下 **[!UICONTROL 執行]**.
