---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 「Workfront Fusion發行活動： 2021年1月11日起一週」
description: 本頁說明2021年1月11日當週在Adobe Workfront Fusion中所做的所有增強功能。
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Workfront Fusion發行活動： 2021年1月11日起一週

本頁說明2021年1月11日當週在Adobe Workfront Fusion中所做的所有增強功能。

如需所有最近變更的清單，請參閱[Adobe Workfront Fusion發行活動](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)。

如需Workfront Fusion中最近的錯誤修正清單，請參閱[Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)頁面，並檢查任何標示為Workfront Fusion維護更新的更新。

## 現在提供加寬聯結器和模組

您現在可以使用Workfront Fusion連線至您的Widen帳戶。 使用「加寬」模組，您可以：

* 在集合中新增或移除資產
* 下載或上傳檔案
* 讀取或更新資產中繼資料
* 根據您指定的條件搜尋資產
* 擷取集合中的資產清單
* 執行自訂API呼叫。

如需詳細資訊，請參閱[加寬模組](../../../workfront-fusion/apps-and-their-modules/widen-modules.md)。

## Datadog聯結器和模組現已推出

您現在可以使用Workfront Fusion連線至您的Datadog帳戶。

使用Datadog模組，您可以：

* Post時間序列點
* 執行自訂API呼叫

如需Datadog模組的相關資訊，請參閱[Datadog模組](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md)。

## 現已提供事件聯結器和模組

您現在可以使用Workfront Fusion 2.0連線至您的Cvent帳戶。

使用Cvent模組，您可以：

* 建立會議邀請
* 讀取連絡人、活動或受邀者等記錄
* 根據您指定的條件列出記錄
* 註冊或新增受邀者至特定活動
* 更新或刪除連絡人
* 進行自訂API呼叫

如需有關可用Cvent模組的資訊，請參閱[Cvent模組](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md)。

## Microsoft Dynamics 365聯結器和模組現已推出

您現在可以使用Workfront Fusion 2.0連線至您的Microsoft Dynamics 365帳戶。 使用Microsoft Dynamics 365模組，您可以：

* 在Microsoft Dynamics 365中新增或更新記錄時觸發案例
* 建立、讀取、更新或刪除Microsoft Dynamics 365記錄
* 執行自訂API呼叫

如需有關可用Microsoft Dynamics 365模組的資訊，請參閱[Microsoft Dynamics 365模組](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md)。

## DocuSign聯結器和模組現已推出

您現在可以使用Workfront Fusion 2.0連線至您的Docusign帳戶。 使用「檔案」模組，您可以：

* 當信封變更其狀態時觸發案例
* 建立信封
* 讀取、傳送收件者或新增收件者到現有的信封
* 新增或修改檔案中的自訂欄位
* 將檔案下載為已失敗
* 將檔案上傳到信封
* 執行自訂API呼叫

如需詳細資訊，請參閱[DocuSign模組](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md)。

## 搜尋您的案例執行歷史記錄

我們讓您更輕鬆地從先前的案例執行中尋找特定資訊。 Fusion的全文檢索搜尋功能可讓您搜尋套件中包含之任何資料的執行記錄。 例如，若要識別建立特定任務的執行，您可以使用全文搜尋來搜尋該任務ID。

以前，要尋找特定的執行資訊，需要分別檢視每個執行。

如需詳細資訊，請參閱[在Adobe Workfront Fusion中檢視案例的執行歷程記錄](../../../workfront-fusion/scenarios/view-scenario-execution-history.md)。

## Fusion 2.0資料存放區的更新

為了讓您更輕鬆地自訂資料存放區，我們新增了一些新功能。 現在，當您檢視資料存放區時，您可以：

* 拖放以重新排序欄
* 編輯單一儲存格
* 新增多列

如需資料存放區的詳細資訊，請參閱[資料存放區模組](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md)。

## 透過HTTP聯結器發出API金鑰授權請求

為了增加您存取API方式的彈性，我們在HTTP聯結器中新增了一個模組。 現在，當您要存取的Web服務需要使用API金鑰時，您可以使用HTTP聯結器來提出要求。

如需詳細資訊，請參閱[HTTP模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)。

## 對應面板中可用的新函式

為協助您自訂及簡化模組中的公式，我們新增了一些新函式。

* 此

  ```
  omit
  ```

  函式是忽略物件的指定索引鍵並傳回其餘專案的一般函式。
* 此

  ```
  pick
  ```

  函式是僅從物件中挑選指定索引鍵的一般函式。
* 此

  ```
  escapeMarkdown
  ```

  函式為字串函式，可逸出文字中的所有Markdown標籤。

如需省略和挑選函式的詳細資訊，請參閱[Adobe Workfront Fusion中的一般函式](../../../workfront-fusion/functions/general-functions.md)。

如需有關escapeMarkdown函式的詳細資訊，請參閱Adobe Workfront Fusion中的[字串函式](../../../workfront-fusion/functions/string-functions.md)。
