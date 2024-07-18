---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 複製 [!DNL Adobe Workfront Fusion]中的模組或案例
description: 複製 [!DNL Adobe Workfront Fusion]中的模組或案例
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# 複製[!DNL Adobe Workfront Fusion]中的模組或案例

您可以在[!DNL Adobe Workfront Fusion]中複製模組、模組群組或整個案例。 此功能可讓您重複使用案例或部分案例，而無需再次建置

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

您必須先將模組新增至情境，才能複製模組。

## 複製模組或模組群組

當您複製模組時，副本會保留原始模組的所有欄位值和設定。

您可以將一個或多個模組貼到相同情境的另一個區域或不同情境中。

將模組貼到不同情境時，請考量下列事項。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* 從您未複製的其他模組提取資訊的任何欄位值，都無法再存取該資訊。 您必須設定這些欄位，才能從新情境中提取資訊。
* 如果您將模組貼到另一個團隊或組織所擁有的情境中，所有連線都必須更新為擁有新情境的群組或組織所擁有的連線。

### 複製模組

複製模組群組類似於複製單一模組。

1. 以滑鼠右鍵按一下要複製的模組。

   >[!NOTE]
   >
   >按住[!UICONTROL Shift]並按一下您要複製的模組，即可選取多個模組。 複製模組群組也會複製它們之間的任何連線線、篩選器或路由邏輯。

1. 選取&#x200B;**[!UICONTROL 複製模組]**。
1. 將游標移至您要複製情境的情境區域。
1. 按一下滑鼠右鍵，然後選取&#x200B;**[!UICONTROL 貼上]**。
1. 將貼上的模組拖曳至情境中的適當位置，以將模組連結至情境。

   您也可以使用鍵盤快速鍵來複製和貼上。

## 複製情境

複製情境會建立情境的復本，然後您可以進行編輯。

1. 開啟案例詳細資訊頁面：

   1. 按一下左側面板中的&#x200B;**[!UICONTROL 案例]**&#x200B;索引標籤，然後按一下您想要瞭解詳細資訊的案例。

      或

      如果您正在[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)中處理案例編輯器，請按一下視窗左上角附近的向左箭頭![](assets/exit-editing-arrow.png)。

1. 以滑鼠右鍵按一下頁面右上角的&#x200B;**[!UICONTROL 選項]**。
1. 選取&#x200B;**[!UICONTROL 複製]**。
1. （選擇性）輸入新情境的名稱。
1. （選擇性）啟用&#x200B;**[!UICONTROL 保持任何新模組的狀態與要複製的模組的狀態相同]**，以確保複製的案例也包含原始案例所處理之最近記錄的資訊。
1. 按一下&#x200B;**[!UICONTROL 儲存]**&#x200B;以建立情境。

## 使用藍圖複製案例

情境Blueprint代表指定情境在指定時間點的排列、對應和欄位值。 您可以將情境Blueprint匯出至電腦上的JSON檔案，然後在建立新情境時匯入它。 可以編輯從情境Blueprint匯入的情境。

情境藍圖代表整個情境。 若您只想從案例中複製某些模組，請參閱本文中的[複製模組或模組群組](#copy-a-module-or-a-group-of-modules)。

>[!NOTE]
>
>有關[!DNL Adobe Workfront]內容中藍圖的資訊，請參閱[藍圖概觀](../../administration-and-setup/blueprints/blueprints-overview.md)。

### 匯出情境藍圖

1. 在案例中，按一下案例設定區域中的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表。
1. 按一下&#x200B;**[!UICONTROL 匯出Blueprint]**。

   會建立JSON檔案並下載至您的電腦。 您可以在[!DNL Downloads]資料夾中找到此檔案。

### 匯入Blueprint

>[!IMPORTANT]
>
>如果您將藍圖匯入現有情境，情境藍圖會取代現有情境。 您無法將藍圖附加至現有情境。

1. 開始建立新情境。
1. 在案例中，按一下案例設定區域中的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表。
1. 按一下&#x200B;**[!UICONTROL 匯入Blueprint]**。
1. 在出現的對話方塊中，按一下&#x200B;**[!UICONTROL 瀏覽]**
1. 導覽至您要匯入的藍圖，然後按一下&#x200B;**[!UICONTROL 開啟]**。
1. 按一下「**[!UICONTROL 儲存]**」。

   會建立JSON檔案並下載至您的電腦。 您可以在[!UICONTROL 下載]資料夾中找到此檔案。

## 使用範本複製和重複使用案例

您可以建立範本作為[!DNL Workfront Fusion]案例的起點。 當您從範本建立案例時，可以修改案例而不修改範本。 欄位值未儲存在範本中。

如需建立及使用範本的詳細資訊，請參閱[情境範本](../../workfront-fusion/scenarios/templates/fusion-templates.md)。
