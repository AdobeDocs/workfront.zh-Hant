---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Qualtrics模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用Qualtrics的工作流程，並將其連線到多個第三方應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Qualtrics模組

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Qualtrics]，以及將其連線到多個協力廠商應用程式和服務。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
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

使用 [!DNL Qualtrics] 模組，您必須擁有 [!UICONTROL Qualtrics] 帳戶。

## 正在連線 [!DNL Qualtrics] 至 [!DNL Workfront Fusion]

您可以建立與的連線 [!DNL Qualtrics] 直接從a內的帳戶 [!UICONTROL Qualtrics] 模組。

1. 在任何 [!UICONTROL Qualtrics] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 輸入下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL連線名稱]</p> </td> 
      <td> <p>輸入新連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL資料中心ID] </td> 
      <td>使用格式 <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL API金鑰]</td> 
      <td>若要尋找您的API金鑰，請參閱 [!DNL Qualtrics] 說明檔案。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。

## [!DNL Qualtrics] 模組及其欄位

下列模組適用於 [!DNL Qualtrics] 聯結器：

* [!UICONTROL 觀看新的調查回應]
* [!UICONTROL 建立目錄連絡人]
* [!UICONTROL 刪除目錄連絡人]
* [!UICONTROL 取得目錄連絡人]
* [!UICONTROL 更新目錄連絡人]
* [!UICONTROL 透過簡訊建立新的調查分佈]
* [!UICONTROL 透過電子郵件發佈意見調查]
* [!UICONTROL 進行API呼叫]
* [!UICONTROL 列出目錄連絡人]
