---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 選擇觸發程式模組在Adobe Workfront Fusion中的開始位置
description: 某些觸發器模組允許您選擇要從中開始檢索包的第一個包。
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 選擇觸發程式模組的起始位置 [!DNL Adobe Workfront Fusion]

某些觸發器模組允許您選擇要從中開始檢索包的第一個包。

您也可以指定是要從特定日期之後擷取所有套件組合，還是只擷取套件組合。

如需觸發程式模組的詳細資訊，請參閱區段 [觸發模組](../../workfront-fusion/modules/module-types.md#triggers) 在文章中 [模組類型](../../workfront-fusion/modules/module-types.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 選擇觸發程式模組的開始位置

1. 儲存觸發程式模組。

   或

   依照 [在 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   或

   以滑鼠右鍵按一下 [!UICONTROL 藍本編輯器]，如 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 在 **[!UICONTROL 選擇要開始的位置]** 框中。

   ![](assets/choose-where-to-start-350x346.jpg)

   顯示的選項取決於指定服務的可能性。 其中可能包括：

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL從現在開始]（預設）</td>
            <td>從現在開始擷取新增或更新的所有套件組合（視設定而定）</td>
        </tr>
        <tr>
            <td>[!UICONTROL從特定日期之後]</td>
            <td>在指定的日期/時間後，擷取新增或更新的所有套件組合（視設定而定）</td>
        </tr>
        <tr>
            <td>[!UICONTROL ID大於或等於特定值]</td>
            <td>擷取ID大於或等於指定ID的所有套件組合</td> 
        </tr>
        <tr>
            <td>[!UICONTROL所有套件組合]</td>
            <td>擷取所有可用的套件組合</td>
        </tr>
        <tr>
            <td>[!UICONTROL選擇第一個捆綁包]</td>
            <td>允許您選擇要從中開始檢索包的第一個包</td>
        </tr>
   </table>
