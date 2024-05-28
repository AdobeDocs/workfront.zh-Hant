---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 目前可用的Adobe Workfront Fusion範本
description: Adobe Workfront Fusion目前提供下列公用範本。
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: e569469c2b5e0ba40569ef86043294acae7a6aa8
workflow-type: tm+mt
source-wordcount: '1186'
ht-degree: 0%

---

# 目前可用的Adobe Workfront Fusion範本

Adobe Workfront Fusion目前提供下列公用範本。

您的團隊或組織可能有其他可用的團隊建立範本。

若要檢視可用的範本，請按一下 **範本** 圖示 ![](assets/fusion-template-icon.png) 在Fusion的側邊導覽功能表中。

## Workfront範本

這些範本會自動化Workfront流程和工作流程。

### [!BADGE 最新！]{type=Informative}

此Fusion範本會針對在計時基礎上輸入特定欄位的所有卡片建立標準檢查清單。

### Workfront — 從CSV建立專案

此自動化會根據您在CSV中指定的名稱、Portfolio、狀態、計劃開始日期和範本詳細資訊，在Workfront中建立新專案。

### Workfront — 清理請求，過去30天內未新增附註

使用此範本來強制30天附註更新您的請求。 未在30天內更新的請求其狀態會在60天變更並關閉。

### Workfront — 在100%完成時將專案狀態變更為完成。

此自動化會將具有1005完成時所有任務的專案更新為「完成」狀態。 有未完成問題或未完成任務或專案核准的專案將收到更新，在解決後，專案將移動到「完成」狀態。

### Workfront — 警告並嘗試關閉過時的專案

使用此情境協助針對符合您組織過時專案原則的專案，自動發出警告，並關閉專案。

### Workfront — 將來源問題/請求的新附註和回覆複製到已轉換的專案或任務

使用此範本將問題或請求的附註和回覆複製到已轉換的專案或任務。

### Workfront — 複製計畫自訂Forms和欄位資料至關聯的新專案

此自動化功能會使用自訂表單來監視程式中的新專案。 然後，它會將這些計畫自訂表單和欄位新增到新專案。

### Workfront — 將自訂Forms和欄位資料複製到關聯的新專案Portfolio

此自動化功能會透過自訂表單，監控投資組合中的新專案。 然後，它會將這些產品組合自訂表單和欄位新增到新專案。

### Workfront — 將已核准問題轉換為專案

此範本會將問題轉換為專案。 您可以修改以符合組織的標準。

### Workfront — 將檔案從問題/請求複製到已轉換的專案或任務

此彈性案例會將問題或請求中的檔案複製到先前轉換的專案或任務。

### 根據欄位變更量身打造的通知

此範本會根據某些獨特事件（例如欄位值的變更），為處理Workfront專案的個人建立自訂更新（及相關通知）。 此案例會監視Workfront中特定欄位何時變更任務或問題。 遇到問題時，情境將會評估相關專案中的資訊，並為指派給專案上特定角色的人建立量身打造的更新。

### Workfront — 使用慣例大量附加至專案名稱

此大量更新範本會重新命名符合搜尋條件（屬於某個投資組合）的所有專案，並以標準格式重新命名。

### Workfront — 使用慣例重新命名專案

此範本會找出符合篩選條件（屬於某個投資組合）的所有專案，並以標準格式重新命名。

### Workfront — 建立狀態變更基準線

此範本會在「切換」模組中記錄的任何專案狀態變更時擷取專案基準，並在更新流中建立更新以供記錄。

### Workfront — 每週建立基準線

此範本每週星期一早上6點在依投資組合篩選的專案上擷取專案基準，並在更新流中建立更新以供記錄。

### 尋找原則時間內未使用的專案範本並通知

每月使用您自己的原則來檢閱一次專案範本，這個容易管理的範本會通知違反您原則之範本上的適當使用者。

## Workfront - Workfront Proof範本

這些範本可自動化結合Workfront與Workfront Proof的工作流程。

### Workfront Proof > Workfront — 校訂決定時的專案更新

當對直接新增到專案的校訂做出決定時，此自動化會收集關於校訂決定的資訊（例如誰做出了決定），然後將這個進度反映在對應Workfront專案作為更新。

### Workfront Proof > Workfront — 在校訂決定上任務更新和完成（如果核准）

當個別校訂繫結至個別任務時，此情境會在對校訂做出核准決定時關閉相關任務。 如果核准，它將會完成任務並更新專案。

## http - Workfront範本

這些範本會從Web服務擷取資訊，並將該資訊帶入Workfront。

>[!NOTE]
>
> 您必須擁有Workfront Fusion for Work Automation and Integration授權，才能在此區段使用範本。

### 使用JWT （JSON Web權杖）建立連線

為使用者端API建立JWT授權。

### APILayer > Workfront — 每日匯率更新(EUR)

此範本會建立自動在設定時間點更新匯率的情境。 此情境會從APIlayers.com API提取歐元(EUR)對美元(USD)的匯率，並更新Workfront中的匯率。

## Workfront-Marketo範本

這些範本支援Workfront-Marketo整合。

>[!NOTE]
>
> 您必須擁有Workfront Fusion for Work Automation and Integration授權，才能在此區段使用範本。

### 透過Workfront核准工作流程核准您的Marketo Engage電子郵件草稿

這是Workfront與Marketo Engage之間檢閱和核准整合的一部分。 此範本會偵測Workfront中的電子郵件校訂是否已核准，然後更新Marketo Engage中已核准的對應電子郵件。

### 在Workfront中接收行銷活動請求，並在Marketo Engage中自動建立行銷活動

此情境提供了一種程式化方式，可讓您根據在Workfront中提出的請求，在Marketo Engage中建立電子郵件和網路研討會行銷活動。 透過使用自動化來建立、組織和設定行銷活動，團隊能夠提高效率。

### 在Workfront中檢閱您Marketo Engage電子郵件草稿的電子郵件校樣

此範本會偵測Workfront任務是否已設定為準備好檢閱狀態，然後從Marketo Engage匯出電子郵件草稿以將其儲存為Workfront中的校訂。

## Workfront-SharePoint範本

這些範本可連線Workfront和SharePoint。

>[!NOTE]
>
> 您必須擁有Workfront Fusion for Work Automation and Integration授權，才能在此區段使用範本。

### 監視SharePoint資料夾的變更

此範本可讓您檢視SharePoint資料夾中是否有變更。


## Workfront-Anaplan範本

這些範本支援Workfront-Anaplan整合，並且預期Workfront中的Anaplan會有特定設定。 如需這些範本及其所需設定的詳細資訊，請參閱各範本的相關文章。

如需Workfront-Anaplan整合的詳細資訊，請參閱 [Adobe Workfront與Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

>[!NOTE]
>
> 您必須擁有Workfront Fusion for Work Automation and Integration授權，才能在此區段使用範本。

### 支出最佳化工作流程

* [傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單專案](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [傳送 [!DNL Adobe Workfront] 費用至 [!DNL Anaplan] 清單專案](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
* [傳送 [!DNL Adobe Workfront] 實際小時更新至 [!DNL Anaplan] 清單專案](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

### 連結預算請求的工作流程

* [建立 [!DNL Anaplan] 清單專案來自 [!DNL Adobe Workfront] 預算請求](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [套用 [!DNL Anaplan] 預算分配至 [!DNL Adobe Workfront] 專案](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

### 連結行銷活動請求的工作流程

* [建立 [!DNL Anaplan] 清單專案來自 [!DNL Adobe Workfront] 行銷活動請求](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [套用 [!DNL Anaplan] 預算分配至 [!DNL Adobe Workfront] 行銷活動請求或行銷活動專案](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)


<!--[!BADGE New!]{type=Informative} -->