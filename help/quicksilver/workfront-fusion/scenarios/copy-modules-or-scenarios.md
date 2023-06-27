---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 複製模組或情境於 [!DNL Adobe Workfront Fusion]
description: 複製模組或情境於 [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# 複製模組或情境於 [!DNL Adobe Workfront Fusion]

您可以複製模組、模組群組或整個情境，在 [!DNL Adobe Workfront Fusion]. 此功能可讓您重複使用案例或案例的一部分，而無需重新建置它們

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

您必須先將模組新增至情境，才能複製模組。

## 複製模組或模組群組

當您複製模組時，副本會保留原始模組的所有欄位值和設定。

您可以將一個或多個模組貼到相同情境的另一個區域或不同情境中。

將模組貼入不同情境時，請考量下列事項。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* 從您未複製的其他模組提取資訊的任何欄位值，都無法再存取該資訊。 您必須設定這些欄位，才能從新案例中提取資訊。
* 如果您將模組貼到另一個團隊或組織所擁有的情境中，所有連線都必須更新為擁有新情境的群組或組織所擁有的連線。

### 複製模組

複製模組群組類似於複製單一模組。

1. 以滑鼠右鍵按一下您要複製的模組。

   >[!NOTE]
   >
   >您可以按住以選取多個模組 [!UICONTROL shift] 並按一下您要複製的模組。 複製模組群組時，也會複製模組之間的任何連線線、篩選器或路由邏輯。

1. 選取 **[!UICONTROL 複製模組]**.
1. 將游標移至您要複製情境的情境區域。
1. 按一下滑鼠右鍵，然後選取 **[!UICONTROL 貼上]**.
1. 將貼上的模組拖曳至情境中的適當位置，以將模組連結至情境。

   您也可以使用鍵盤快速鍵來複製和貼上。

## 複製情境

複製情境會建立情境的復本，然後您可以進行編輯。

1. 開啟案例詳細資訊頁面：

   1. 按一下 **[!UICONTROL 情境]** 索引標籤中，然後按一下您要瞭解詳細資訊的情境。

      或

      如果您使用的情境在 [中的案例編輯器 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)，按一下向左鍵 ![](assets/exit-editing-arrow.png) 靠近視窗的左上角。

1. 按一下右鍵 **[!UICONTROL 選項]** 頁面右上角的。
1. 選取 **[!UICONTROL 原地複製]**.
1. （選擇性）輸入新情境的名稱。
1. （選用）啟用 **[!UICONTROL 使任何新模組的狀態與複製時相同]** 以確保複製的案例也包含原始案例處理之最近記錄的相關資訊。
1. 按一下 **[!UICONTROL 儲存]** 以建立情境。

## 使用藍圖複製案例

案例Blueprint代表指定案例在指定時間點的排列、對應和欄位值。 您可以將情境Blueprint匯出至電腦上的JSON檔案中，然後在建立新情境時匯入該情境。 可以編輯從案例Blueprint匯入的案例。

情境藍圖代表整個情境。 如果您只想從案例中複製特定模組，請參閱 [複製模組或模組群組](#copy-a-module-or-a-group-of-modules) 本文章內容。

>[!NOTE]
>
>有關以下專案內容中的藍圖資訊： [!DNL Adobe Workfront]，請參閱 [藍圖概觀](../../administration-and-setup/blueprints/blueprints-overview.md).

### 匯出案例Blueprint

1. 在情境中，按一下 **[!UICONTROL 更多]** 情境設定區域中的功能表。
1. 按一下 **[!UICONTROL 匯出Blueprint]**.

   會建立JSON檔案並下載至您的電腦。 您可以在下列位置找到此檔案： [!DNL Downloads] 資料夾。

### 匯入Blueprint

>[!IMPORTANT]
>
>如果您將Blueprint匯入至現有案例，案例Blueprint會取代現有案例。 您無法將藍圖附加至現有情境。

1. 開始建立新情境。
1. 在情境中，按一下 **[!UICONTROL 更多]** 情境設定區域中的功能表。
1. 按一下 **[!UICONTROL 匯入Blueprint]**.
1. 在出現的對話方塊中，按一下 **[!UICONTROL 瀏覽]**
1. 導覽至您要匯入的藍圖，然後按一下 **[!UICONTROL 開啟]**.
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   會建立JSON檔案並下載至您的電腦。 您可以在下列位置找到此檔案： [!UICONTROL 下載] 資料夾。

## 使用範本複製和重複使用案例

您可以將範本建立為 [!DNL Workfront Fusion] 情境。 當您從範本建立案例時，無需修改範本即可修改案例。 欄位值不會儲存在範本中。

如需建立和使用範本的詳細資訊，請參閱 [案例範本](../../workfront-fusion/scenarios/templates/fusion-templates.md).
