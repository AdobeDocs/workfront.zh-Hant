---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: SDL管理翻譯模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以將SDL Managed Translation帳戶連線至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# [!DNL SDL Managed Translation]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以將[!DNL SDL Managed Translation]帳戶連線至多個協力廠商應用程式和服務。

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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，貴組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## SDL Managed Translation API資訊

SDL Managed Translation聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td>https://languagecloud.sdl.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.4.26</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL SDL Managed Translation]模組

>[!NOTE]
>
>呼叫[!DNL SDL Managed Translation]的作業逾時為&#x200B;**120秒**。

### 檔案

#### [!UICONTROL 下載翻譯的檔案]

此模組會擷取指定專案中包含之單一翻譯檔案的內容。 如果請求的檔案尚未處於下載狀態，則檔案的內容可能尚未完全翻譯。 如果檔案處於下載狀態，而且您已成功擷取檔案，請務必使用`Cancel or Complete File`方法將檔案標示為完成。

#### [!UICONTROL 上傳檔案]

此模組允許上傳要翻譯或包含在翻譯專案中作為參考資料的檔案。 上傳必須使用多部分/表單資料提交，並且可以包含多個檔案。 您指定用於評估已上傳檔案的`ProjectOptionId`。 這會決定您上傳的每個檔案是可能的候選翻譯，還是必須作為參考資料處理。 若是封存（`zip `、`rar`、`7z`、`tar`個檔案），應用程式會檢查封存的內容，並指出封存整體是否可以翻譯，或封存是否包含可翻譯與不可翻譯檔案的混合。

>[!NOTE]
>
>不建議一次上傳多個檔案，因為這可能會增加任何失敗的影響。

#### [!UICONTROL 新增參考檔案]

此模組會新增參考檔案。

### 專案

#### [!UICONTROL 建立專案]

此模組會建立指定的專案。

#### 取消或完成專案

此模組會取消或完成指定的專案。 如果專案正在等待下載，專案會透過工作流程中的任何最終步驟進行轉換，並最終移動以完成。 如果專案正在等待核准或供應商選擇已取消。 如果專案處於任何其他狀態，請求將失敗。

#### [!UICONTROL 下載專案Zip]

此模組取得指定專案的`zip`轉譯檔案。

#### [!UICONTROL 讀取專案]

此模組取得指定的專案。

#### [!UICONTROL 取得狀態為]的專案

此模組取得所有處於指定狀態的可用專案。 此方法可透過指定`$top`、`$skip`和`$orderby`查詢引數來允許分頁結果。

#### [!UICONTROL 取得專案清單]

取得所有專案的簡單清單，提供有關每個專案的一般資訊。 此方法可透過指定`$top`、`$skip`和`$orderby`查詢引數來允許結果為頁面。

#### [!UICONTROL 搜尋專案建立選項]

此模組取得專案建立選項。

### 其他

#### [!UICONTROL 進行API呼叫]

此模組會執行任意授權的API呼叫。
