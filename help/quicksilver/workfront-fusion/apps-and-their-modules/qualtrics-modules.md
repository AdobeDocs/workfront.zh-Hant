---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Qualtrics模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Qualtrics的工作流程，並將其連線至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Qualtrics模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Qualtrics]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
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

若要使用[!DNL Qualtrics]模組，您必須有[!UICONTROL Qualtrics]帳戶。

## 正在連線[!DNL Qualtrics]至[!DNL Workfront Fusion]

您可以直接從[!UICONTROL Qualtrics]模組內建立與您的[!DNL Qualtrics]帳戶的連線。

1. 在任何[!UICONTROL Qualtrics]模組中，按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
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
      <td>使用格式<code>&lt;Data Center ID>.qualtrics.com</code>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL API Key]</td> 
      <td>若要尋找您的API金鑰，請參閱[!DNL Qualtrics]檔案。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以建立連線並返回模組。

## [!DNL Qualtrics]模組及其欄位

[!DNL Qualtrics]聯結器可使用下列模組：

* [!UICONTROL 觀看新的問卷回應]
* [!UICONTROL 建立目錄連絡人]
* [!UICONTROL 刪除目錄連絡人]
* [!UICONTROL 取得目錄連絡人]
* [!UICONTROL 更新目錄連絡人]
* [!UICONTROL 透過SMS建立新的意見調查發佈]
* [!UICONTROL 透過電子郵件散發問卷]
* [!UICONTROL 進行API呼叫]
* [!UICONTROL 列出目錄連絡人]
