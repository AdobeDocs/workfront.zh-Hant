---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Workfront Fusion發行活動：《2021年1月11日周》'
description: 本頁說明2021年1月11日當周在Adobe Workfront Fusion中所做的所有增強功能。
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# Workfront Fusion發行活動： 2021年1月11日起第一週

本頁說明2021年1月11日當周在Adobe Workfront Fusion中所做的所有增強功能。

如需所有最近變更的清單，請參閱 [Adobe Workfront Fusion發行活動](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

如需Workfront Fusion最近錯誤修正的清單，請參閱 [Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) 並檢查任何標示為「Workfront Fusion維護更新」的更新。

## 現已可擴展連接器和模組

您現在可以使用Workfront Fusion連線至您的Widen帳戶。 使用「擴展」模組，您可以：

* 新增資產至集合或從集合中移除資產
* 下載或上傳檔案
* 讀取或更新資產中繼資料
* 根據您指定的條件搜尋資產
* 擷取集合中的資產清單
* 執行自訂API呼叫。

如需詳細資訊，請參閱 [擴展模組](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## Datagog連接器和模組現已可用

您現在可以使用Workfront Fusion連線至您的Datadog帳戶。

透過Datadog模組，您可以：

* 後置時間點
* 執行自訂API呼叫

如需Datadog模組的相關資訊，請參閱 [Datadog模組](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## 現在提供Cvent連接器和模組

您現在可以使用Workfront Fusion 2.0連線至Cevent帳戶。

使用「事件」模組，您可以：

* 建立會議請求
* 閱讀記錄，如聯繫人、事件或被邀請者
* 根據您指定的條件列出記錄
* 註冊或添加被邀請者到特定事件
* 更新或刪除聯繫人
* 進行自訂API呼叫

如需可用Cevent模組的相關資訊，請參閱 [事件模組](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## Microsoft Dynamics 365連接器和模組現已推出

您現在可以使用Workfront Fusion 2.0連線至您的Microsoft Dynamics 365帳戶。 有了Microsoft Dynamics 365模組，您可以：

* 在Microsoft Dynamics 365中新增或更新記錄時觸發案例
* 建立、讀取、更新或刪除Microsoft Dynamics 365記錄
* 執行自訂API呼叫

如需可用Microsoft Dynamics 365模組的相關資訊，請參閱 [Microsoft Dynamics 365模組](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## DocuSign連接器和模組現已可用

您現在可以使用Workfront Fusion 2.0連線至您的Document帳戶。 使用「文檔」模組，您可以：

* 信封更改其狀態時觸發情境
* 建立信封
* 讀取、發送或將收件者添加到現有信封
* 添加或修改文檔中的自定義欄位
* 以歸檔方式下載文檔
* 將檔案上傳至信封
* 執行自訂API呼叫

如需詳細資訊，請參閱 [DocuSign模組](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## 搜尋您的藍本執行歷史記錄

我們讓您更輕鬆地從先前的方案執行中找到特定資訊。 Fusion的全文搜索使搜索捆綁包中包含的任何資料的執行歷史記錄成為可能。 例如，要標識建立了特定任務的執行，可以使用全文搜索來搜索該任務ID。

以前，需要分別檢視每個執行來尋找特定的執行資訊。

如需詳細資訊，請參閱 [在Adobe Workfront Fusion中檢視案例的執行歷史記錄](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Fusion 2.0資料儲存的更新

為了讓您更輕鬆自訂資料存放區，我們新增了一些新功能。 現在，當您檢視資料存放區時，可以：

* 拖放以重新排序欄
* 編輯單一儲存格
* 新增多列

如需資料存放區的詳細資訊，請參閱 [資料儲存模組](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## 透過HTTP連接器提出API金鑰授權要求

為了提高存取API的方式彈性，我們已在HTTP連接器中新增模組。 現在，當您存取的Web服務需要使用API金鑰時，可以使用HTTP連接器提出要求。

如需詳細資訊，請參閱 [HTTP模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## 映射面板中提供的新功能

為協助您自訂和簡化模組中的公式，我們新增了一些新函式。

* 此

   ```
   omit
   ```

   函式是一般函式，可省略物件的指定鍵值並傳回其餘。
* 此

   ```
   pick
   ```

   函式是只從物件中挑選指定索引鍵的一般函式。
* 此

   ```
   escapeMarkdown
   ```

   函式是字串函式，可逸出文字中的所有Markdown標籤。

有關省略和挑選功能的詳細資訊，請參閱 [Adobe Workfront Fusion的一般功能](../../../workfront-fusion/functions/general-functions.md).

如需escapeMarkdown函式的詳細資訊，請參閱 [Adobe Workfront Fusion中的字串函式](../../../workfront-fusion/functions/string-functions.md).
