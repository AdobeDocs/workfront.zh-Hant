---
content-type: reference
navigation-topic: search
title: 使用對象的參考編號
description: 在 [!DNL Adobe Workfront]，項目會識別為物件。 對象與資料庫對應，用於將資料與項關聯。 在區分兩個其他類似對象時（例如具有相同名稱的任務），參考編號很有用。 您可以搜尋參考編號並將其納入報表中。
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 使用對象的參考編號

在 [!DNL Adobe Workfront]，項目會識別為物件。 對象與資料庫對應，用於將資料與項關聯。

Workfront會在建立物件時，自動為下列每個物件指派一個唯一的參考編號：

* 專案
* 任務
* 問題
* 文件

在區分兩個其他類似對象時（例如具有相同名稱的任務），參考編號很有用。 您可以搜尋參考編號並將其納入報表中。

>[!IMPORTANT]
>
>* [!DNL Workfront] 連續分配所有客戶和所有對象的引用編號。 例如，建立任務時， [!DNL Workfront] 可能會為它指定一個參考號00005。 如果另一個客戶在下一個建立專案，則其專案可能會收到下一個可用的參考編號，例如00006。 如果您接下來建立問題，您的問題可能會收到參考編號00007，以此類推。
>* 不能控制中任何對象的引用編號順序 [!DNL Workfront]. 序列總是由我們的資料庫控制。
>




## 查看對象的參考編號

預設會顯示任務和問題的參考編號。 您也可以輕鬆配置 [!DNL Workfront] 顯示其他類型對象的參考編號。

* [查看任務和問題的參考編號](#view-reference-numbers-for-tasks-and-issues)
* [查看其他對象的參考編號](#view-reference-numbers-for-other-objects)
* [在報表中檢視參考編號](#view-reference-numbers-in-reports)

### 查看任務和問題的參考編號

在查看任務或問題時，預設會顯示參考編號。  若要查看參考編號，請按一下 **[!UICONTROL 任務詳細資訊]** 或 **[!UICONTROL 問題詳細資訊]** 在左側面板中，找到 **[!UICONTROL 基本資訊]** 一節。

![](assets/reference-number-nwe-350x184.png)

### 查看其他對象的參考編號

要查看對象的參考編號，可以建立自定義視圖或修改現有視圖並添加 [!UICONTROL 參考編號] 欄。 例如，您可以修改 [!UICONTROL 專案] 檢視以顯示所有專案的參考編號。

有關如何建立或修改視圖的資訊，請參見 [檢視概觀，於 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### 在報表中檢視參考編號

您可以新增 [!UICONTROL 參考編號] 欄。

如需如何將欄新增至報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 按參考編號搜索對象

[!DNL Workfront] 允許您按參考編號搜索對象。

在 **[!UICONTROL 搜尋]** 欄位，然後按 **[!UICONTROL 輸入]**.

如需在Workfront中搜尋的詳細資訊，請參閱 [搜尋 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
