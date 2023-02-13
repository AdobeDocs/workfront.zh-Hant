---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: SDL管理翻譯模組
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以將SDL托管翻譯帳戶連接到多個第三方應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以連結 [!DNL SDL Managed Translation] 帳戶至多個協力廠商應用程式和服務。

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

## [!DNL SDL Managed Translation] 模組

>[!NOTE]
>
>呼叫的作業逾時 [!DNL SDL Managed Translation] is **120秒**.

### 檔案

#### [!UICONTROL 下載翻譯的檔案]

此模組會擷取指定專案中包含之單一翻譯檔案的內容。 如果請求的檔案尚未處於「下載」狀態，則檔案的內容可能尚未完全翻譯。 如果檔案處於「下載」狀態，且您已成功擷取該檔案，請務必使用將檔案標示為已完成 `Cancel or Complete File` 方法。

#### [!UICONTROL 上傳檔案]

此模組允許上傳要翻譯或要作為參考材料包含在翻譯項目中的檔案。 上傳必須使用多部分/表單資料提交，且可包含多個檔案。 您可指定 `ProjectOptionId` 應用來評估上傳的檔案。 這會決定您上傳的每個檔案是否可能是翻譯的候選檔案，還是必須作為參考材料處理。 就檔案而言(`zip `, `rar`, `7z`, `tar` 檔案)應用程式會檢查封存的內容，並指出封存整體是否可翻譯，或是否包含可翻譯和不可翻譯的檔案。

>[!NOTE]
>
>不建議一次上傳多個檔案，因為這可能會增加任何失敗的影響。

#### [!UICONTROL 新增參考檔案]

此模組添加一個參考檔案。

### 專案

#### [!UICONTROL 建立專案]

此模組會建立指定的專案。

#### 取消或完成專案

此模組會取消或完成指定的專案。 如果專案正在等待下載，專案會在工作流程中完成任何最終步驟，並最終移至完成。 如果項目正在等待批准或供應商選擇被取消。 如果專案處於任何其他狀態，要求將會失敗。

#### [!UICONTROL 下載專案Zip]

此模組會取得 `zip` 指定項目的已翻譯檔案檔案。

#### [!UICONTROL 閱讀專案]

此模組會取得指定的專案。

#### [!UICONTROL 以狀態取得專案]

此模組會取得所有處於指定狀態的可用專案。 此方法允許分頁結果，方法是指定 `$top`, `$skip`，和 `$orderby` 查詢參數。

#### [!UICONTROL 取得專案清單]

取得所有專案的簡單清單，提供每個專案的一般資訊。 此方法可讓結果成為頁面，方法是指定 `$top`, `$skip`，和 `$orderby` 查詢參數。

#### [!UICONTROL 搜索項目建立選項]

此模組獲取項目建立選項。

### 其他

#### [!UICONTROL 進行API呼叫]

此模組會執行任意授權的API呼叫。
