---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: SDL管理翻譯模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以將SDL Managed Translation帳戶連線至多個協力廠商的應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] 模組

在 [!DNL Adobe Workfront Fusion] 情境，您可以連線至 [!DNL SDL Managed Translation] 帳戶至多個協力廠商應用程式和服務。

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

## [!DNL SDL Managed Translation] 模組

>[!NOTE]
>
>對的呼叫的作業逾時 [!DNL SDL Managed Translation] 是 **120秒**.

### 檔案

#### [!UICONTROL 下載翻譯的檔案]

此模組會擷取指定專案中包含之單一翻譯檔案的內容。 如果請求的檔案尚未處於下載狀態，則檔案的內容可能尚未完全翻譯。 如果檔案處於下載狀態，而且您已成功擷取它，請務必使用 `Cancel or Complete File` 方法。

#### [!UICONTROL 上傳檔案]

此模組允許上傳要翻譯的檔案或包含在翻譯專案中作為參考資料。 上傳必須使用多部分/表單資料提交，並且可以包含多個檔案。 您指定 `ProjectOptionId` 應該用於評估已上傳的檔案。 這會決定您上傳的每個檔案是可能的候選翻譯，還是必須作為參考資料處理。 若是封存(`zip `， `rar`， `7z`， `tar` 檔案)應用程式會檢查封存內容，並指出封存整體是否可以翻譯，或封存是否混合了可翻譯和不可翻譯的檔案。

>[!NOTE]
>
>不建議一次上傳多個檔案，因為這可能會增加任何失敗的影響。

#### [!UICONTROL 新增參考檔案]

此模組會新增參考檔案。

### 專案

#### [!UICONTROL 建立專案]

此模組會建立指定的專案。

#### 取消或完成專案

此模組會取消或完成指定的專案。 如果專案正在等待下載，專案會完成工作流程中的任何最終步驟，並最終移動完成。 如果專案正在等待核准或供應商選擇已取消。 如果專案處於任何其他狀態，請求將失敗。

#### [!UICONTROL 下載專案Zip]

此模組取得 `zip` 指定專案的已翻譯檔案檔案。

#### [!UICONTROL 讀取專案]

此模組取得指定的專案。

#### [!UICONTROL 取得處於狀態的專案]

此模組會取得所有處於指定狀態的可用專案。 此方法可透過指定結果來分頁 `$top`， `$skip`、和 `$orderby` 查詢引數。

#### [!UICONTROL 取得專案清單]

取得所有專案的簡單清單，提供有關每個專案的一般資訊。 此方法可讓結果成為頁面，方法是指定 `$top`， `$skip`、和 `$orderby` 查詢引數。

#### [!UICONTROL 搜尋專案建立選項]

此模組會取得專案建立選項。

### 其他

#### [!UICONTROL 進行API呼叫]

此模組會執行任意授權的API呼叫。
