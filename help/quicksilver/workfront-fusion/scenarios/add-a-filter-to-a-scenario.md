---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在 [!DNL Adobe] Workfront Fusion中新增篩選器至案例
description: 在某些情況下，您只需要使用符合特定條件的組合。 篩選可讓您選取這些組合。
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 將篩選器新增至[!DNL Adobe Workfront Fusion]中的案例

在某些情況下，您只需要使用符合特定條件的組合。 篩選可讓您選取這些組合。

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

您可以在兩個模組之間新增篩選器，並檢查從先前模組收到的套件組合是否符合特定的篩選條件：

* 如果是，套件組合會傳遞至案例中的下一個模組。
* 如果沒有，則會終止束的處理。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

您必須先將兩個模組新增至情境，才能在它們之間新增篩選器。

## 在兩個模組之間新增篩選器：

1. 按一下左側面板中的&#x200B;**[!UICONTROL 案例]** ![](assets/scenarios-icon.png)，然後選取案例以開啟它。
1. 按一下視窗右上角的&#x200B;**[!UICONTROL 編輯]**。
1. 按一下模組之間的連線線。
1. 在顯示的方塊中，輸入篩選器的&#x200B;**[!UICONTROL 標籤]**。
1. 定義篩選&#x200B;**[!UICONTROL 條件]**。

   您可以在兩個方塊中輸入一或兩個運算元。 如果您在兩個方塊中輸入運算元，則可以在它們之間的下拉式選單中選取運算元，以指定它們之間的關係。

   >[!TIP]
   >
   >在運算元欄位中，您可以像對應值一樣輸入值，如[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組中所述。

   例如，如果您希望篩選器在[!DNL Adobe Workfront]中尋找以XML結尾的檔案，並將它們傳遞至[!DNL Dropbox]，您應該在第一個方塊和中輸入&#x200B;**[!UICONTROL 檔案名稱]**。第二個方塊中的&#x200B;**[!UICONTROL xml]**。 在它們之間的下拉式功能表中，您可以選取&#x200B;**[!UICONTROL 結尾為（不區分大小寫）]**。 此篩選器將套用至來自第一個模組(Workfront)的傳入組合。 只有包含XML檔案的套件組合會傳遞到下一個模組([!DNL Dropbox])。

   ![](assets/set-up-filter-box-350x368.jpg)

1. 按一下&#x200B;**[!DNL OK]**。

## 複製篩選器

目前，案例編輯器不包含複製篩選器的功能。

>[!NOTE]
>
>如果您複製篩選器兩側的模組，也會複製篩選器。
>
>如需複製模組的詳細資訊，請參閱[複製 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)中的模組或案例

若要複製篩選器而不複製模組，您可以使用[!DNL Google] Chrome來做以下因應措施：

1. 安裝[!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome]擴充功能。
1. 在[!DNL Workfront Fusion]中，開啟情境。
1. 按一下Chrome的三點式功能表，然後按一下**[!UICONTROL 更多工具*]* > **[!UICONTROL 開發人員工具]**。

1. 在顯示的[!UICONTROL Developer tools]面板中，按一下頂端功能表列上的[!UICONTROL Workfront Fusion]標籤。

   ![](assets/copy-a-filter-350x174.png)

1. 按一下左側列中的&#x200B;**[!UICONTROL 工具]**&#x200B;圖示![](assets/devtools-tools-icon.png)。

1. 按一下「複製篩選器」****，然後在右側面板中設定「複製篩選器」****&#x200B;工具：

   1. 將&#x200B;**[!UICONTROL Source模組]**&#x200B;設定為您要複製的篩選器之後的模組。
   1. 將&#x200B;**[!UICONTROL 目標模組]**&#x200B;設定為您要複製的篩選器之前的模組。

1. 按一下&#x200B;**[!UICONTROL 執行]**。
