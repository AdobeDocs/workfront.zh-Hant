---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Qualtrics模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Qualtrics的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Qualtrics模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Qualtrics]，並將其連接至多個協力廠商應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
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

使用 [!DNL Qualtrics] 模組，您必須 [!UICONTROL Qualtrics] 帳戶。

## 連接 [!DNL Qualtrics] to [!DNL Workfront Fusion]

您可以建立與 [!DNL Qualtrics] 直接從內部 [!UICONTROL Qualtrics] 模組。

1. 在任何 [!UICONTROL Qualtrics] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 輸入以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL連接名]</p> </td> 
      <td> <p>輸入新連接的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL資料中心ID] </td> 
      <td>使用格式 <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API密鑰]</td> 
      <td>若要尋找您的API金鑰，請參閱 <a href="https://api.qualtrics.com/instructions/docs/Instructions/api-key-authentication.md">API Token驗證</a> 在 [!DNL Qualtrics] 檔案。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL Qualtrics] 模組及其欄位

下列模組適用於 [!DNL Qualtrics] 連接器：

* [!UICONTROL 觀看新的調查回應]
* [!UICONTROL 建立目錄聯繫人]
* [!UICONTROL 刪除目錄聯繫人]
* [!UICONTROL 獲取目錄聯繫人]
* [!UICONTROL 更新目錄聯繫人]
* [!UICONTROL 透過簡訊建立新的調查分送]
* [!UICONTROL 透過電子郵件發佈調查]
* [!UICONTROL 進行API呼叫]
* [!UICONTROL 清單目錄聯繫人]
