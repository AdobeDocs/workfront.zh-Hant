---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 複製中的模組或方案 [!DNL Adobe Workfront Fusion]
description: 複製中的模組或方案 [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# 複製中的模組或方案 [!DNL Adobe Workfront Fusion]

您可以在 [!DNL Adobe Workfront Fusion]. 此功能可讓您重複使用方案或部分方案，而無須再次建置

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

您必須先將模組新增至案例，才能加以複製。

## 複製模組或一組模組

複製模組時，復本會保留原始模組的所有欄位值和設定。

您可以將模組或模組貼到相同案例的其他區域，或貼到不同案例。

將模組貼入不同案例時，請考量下列事項。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* 從您未複製的其他模組提取資訊的任何欄位值，都無法再存取該資訊。 您必須設定這些欄位，才能從新情境中提取資訊。
* 如果將模組貼入另一個團隊或組織擁有的藍本中，所有連線都必須更新為擁有新藍本的群組或組織擁有的連線。

### 複製模組

複製一組模組類似於複製單一模組。

1. 以滑鼠右鍵按一下您要複製的模組。

   >[!NOTE]
   >
   >您可以按住 [!UICONTROL shift] 並按一下要複製的模組。 複製一組模組也會複製它們之間的任何連接線、篩選器或路由邏輯。

1. 選擇 **[!UICONTROL 複製模組]**.
1. 將游標移至您要複製方案的方案區域。
1. 按一下右鍵，然後選擇 **[!UICONTROL 貼上]**.
1. 將貼上的模組拖曳至案例中的適當位置，將其連結至案例。

   您也可以使用鍵盤快速鍵來複製和貼上。

## 複製方案，方法是複製

複製藍本會建立藍本的復本，然後您可以編輯該副本。

1. 開啟方案詳細資訊頁面：

   1. 按一下 **[!UICONTROL 藍本]** 標籤，然後按一下您要詳細資訊的案例。

      或

      若您正在處理 [中的案例編輯器 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)，按一下左箭頭 ![](assets/exit-editing-arrow.png) 靠近窗口的左上角。

1. 按一下右鍵 **[!UICONTROL 選項]** 在頁面的右上角。
1. 選擇 **[!UICONTROL 原地複製]**.
1. （可選）輸入新方案的名稱。
1. （可選）啟用 **[!UICONTROL 將任何新模組的狀態與重複模組的狀態保持相同]** 以確保複製的方案也包含有關原始方案處理的最新記錄的資訊。
1. 按一下 **[!UICONTROL 儲存]** 來建立藍本。

## 使用藍圖複製方案

方案藍圖表示給定方案在給定時間點的安排、映射和欄位值。 您可以將藍圖匯出至電腦上的JSON檔案，然後在建立新藍圖時匯入。 可以編輯從藍本導入的藍本。

藍圖代表整個藍圖。 如果您只想從案例中複製特定模組，請參閱 [複製模組或一組模組](#copy-a-module-or-a-group-of-modules) 這篇文章。

>[!NOTE]
>
>關於 [!DNL Adobe Workfront]，請參閱 [藍圖概述](../../administration-and-setup/blueprints/blueprints-overview.md).

### 匯出藍圖

1. 在案例中，按一下 **[!UICONTROL 更多]** 功能表。
1. 按一下 **[!UICONTROL 匯出Blueprint]**.

   系統會建立JSON檔案，並下載至您的電腦。 您可以在 [!DNL Downloads] 檔案夾。

### 匯入Blueprint

>[!IMPORTANT]
>
>如果您將Blueprint匯入現有藍本，藍本會取代現有藍本。 您無法將Blueprint附加至現有案例。

1. 開始建立新藍本。
1. 在案例中，按一下 **[!UICONTROL 更多]** 功能表。
1. 按一下 **[!UICONTROL 匯入Blueprint]**.
1. 在顯示的對話方塊中，按一下 **[!UICONTROL 瀏覽]**
1. 導覽至您要匯入的Blueprint，然後按一下 **[!UICONTROL 開啟]**.
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   系統會建立JSON檔案，並下載至您的電腦。 您可以在 [!UICONTROL 下載] 檔案夾。

## 使用模板複製和重複使用方案

您可以建立範本，作為您 [!DNL Workfront Fusion] 方案。 從模板建立方案時，可以修改方案而不修改模板。 欄位值不會儲存在範本中。

如需建立和使用範本的詳細資訊，請參閱 [方案範本](../../workfront-fusion/scenarios/templates/fusion-templates.md).
