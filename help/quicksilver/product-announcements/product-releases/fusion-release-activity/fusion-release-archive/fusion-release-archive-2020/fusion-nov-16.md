---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Workfront Fusion發行活動：《2020年11月16日周》'
description: 本頁說明2020年11月16日當周在Adobe Workfront Fusion中所做的所有增強功能。
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 9221a69e-2482-478b-95a9-f62dd28538d6
hidefromtoc: true
source-git-commit: e18b23e7d58aced4c95c5df51769a6e959fa3d57
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Workfront Fusion發行活動： 2020年11月16日起第一週

本頁說明2020年11月16日當周在Adobe Workfront Fusion中所做的所有增強功能。

如需所有最近變更的清單，請參閱 [Adobe Workfront Fusion發行活動](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

如需Workfront Fusion最近錯誤修正的清單，請參閱 [Workfront維護更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) 並檢查任何標示為「Workfront Fusion維護更新」的更新。

## Jira Cloud連接器更新

為了擴展Jira Cloud連接器的使用方式，我們新增了三個新模組：

* 向衝刺添加問題
* 清單記錄
* 搜索記錄

我們還更新了現有模組以支援「Sprint」對象類型。 過去，「Sprint」物件只能透過自訂API呼叫模組存取。

如需詳細資訊，請參閱 [Jira軟體模組](../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md).

## 執行ID現在可用於藍本的對應

藍本的執行ID現在可在對應面板中使用。 此ID代表案例的特定執行，可作為中繼資料使用。 例如，執行ID可與Fusion建立的記錄一起儲存，以便您稍後可以確定建立該記錄的Fusion執行。 您可以在「一般函式」下的「映射」面板中找到「執行ID」。

如需執行情境的詳細資訊，請參閱 [Adobe Workfront Fusion中的情境執行、週期和階段](../../../../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Workfront Fusion 2.0案例的鍵盤快速鍵

為了讓建立情境更方便，我們新增了一些鍵盤快速鍵：

* Ctrl/Cmd+Shift+Enter:執行一次方案
* Ctrl/Cmd + Shift + S:儲存案例

如需有關建立Workfront Fusion 2.0案例的詳細資訊，請參閱 [在Adobe Workfront Fusion中建立案例](../../../../../workfront-fusion/scenarios/create-a-scenario.md).

## 更新Office 365 Excel連接器

為了擴展使用Office 365 Excel連接器的方式，我們添加了一些新模組。 現在您可以：

* 從活頁簿的變更觸發模組
* 搜尋或下載活頁簿
* 列出工作表、工作表行、表或表行
* 更新表或工作表行
* 刪除表或工作表行
* 檢索表的元資料
* 進行自訂API呼叫

應用程式中仍會顯示先前可用的模組。

如需詳細資訊，請參閱 [Microsoft Office 365 Excel模組](../../../../../workfront-fusion/apps-and-their-modules/microsoft-365-excel-modules.md).

## 在Workfront應用程式連線中使用OAuth 2.0

我們已更新Workfront連接器以使用OAuth 2.0。此更新表示在您的Workfront應用程式連線中進行變更會更輕鬆。 例如，如果連線的相關資訊發生變更（例如密碼），您就不需要在案例中更新每個個別連線。 此外，OAuth2還提供其他優點，例如改善安全性，以及使用單一登入(SSO)的功能。

現有連線目前不需要任何變更。 不過，如果您想善用OAuth 2.0的優點，可以重新授權現有連線。

如需詳細資訊，請參閱 [Adobe Workfront模組](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).
