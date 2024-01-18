---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 「Workfront Fusion發行活動： 2021年5月3日當週」
description: 本頁說明2021年5月3日當週在Adobe Workfront Fusion中所做的所有增強功能。
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Workfront Fusion發行活動： 2021年5月3日起一週

本頁說明2021年5月3日當週在Adobe Workfront Fusion中所做的所有增強功能。

如需所有最近變更的清單，請參閱 [Adobe Workfront Fusion發行活動](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

如需Workfront Fusion中近期的錯誤修正清單，請參閱 [Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) 頁面，並檢查是否有任何標示為Workfront Fusion維護更新的更新。

## Salesforce聯結器現在可以使用SOQL進行搜尋

Salesforce > Search for records模組現在可選擇使用SOQL （Salesforce物件查詢語言）進行搜尋。 您也可以使用先前可用的選項（SOSL和簡單搜尋）進行搜尋。

如需詳細資訊，請參閱 [Salesforce模組](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Azure DevOps聯結器中的新連線型別需要較少的領域

為了增強安全性，我們已將一個新的聯結器型別新增到Workfront Fusion Azure DevOps Connector。 現在，當您在Azure DevOps模組中建立連線時，可以從兩種連線型別中進行選取：

* Azure DevOps

  這個新的連線型別將範圍限製為Workfront Fusion特別需要的範圍。

* Azure DevOps （要求所有領域）

  這是舊版連線型別，會要求與Azure DevOps連線中可用的所有範圍。

建議您在使用Azure DevOps的所有新情境中使用Azure DevOps連線型別。 我們也建議您變更現有案例中的任何Azure DevOps模組，以使用新的連線型別。 舊版Azure DevOps （要求所有範圍）連線型別不久將會被取代。

如需詳細資訊，請參閱 [Azure DevOps模組](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
