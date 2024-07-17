---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境提升常見問題集
description: 探索關於Workfront環境升級的常見問題。
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: e2150f344ddc8626389afaaccc7c394f61c2dbc9
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 3%

---

# 環境提升常見問題集

以下是有關環境升級的常見問題集：

## 是否支援跨網域促銷活動？

### 解答

目前不支援跨網域環境升級。 您必須在相同網域中的環境之間升級。

## Adobe商業平台/IMS是進行環境促銷的先決條件嗎？

### 解答

否。環境升級適用於啟用IMS和非IMSorkfront的執行個體。

## 如何知道我們的Workfront執行個體是否位於Prime或Ultimate授權上？

### 解答

* Workfront管理員可找出您組織的授權。

   1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
   1. 按一下左側面板中的&#x200B;**系統**
   1. 若要檢視您的Workfront計畫，請選取&#x200B;**授權**。
您的計畫會顯示在頁面右上角附近。
      ![](assets/locate-plan.png)

  或
* 請聯絡您的Workfront客戶代表。

## 環境促銷活動是否為雙向的？

### 解答

是。例如，您可以從Sandox提升至生產環境，或從Production提升至沙箱。

## 是否支援共用？

### 解答

否，目前不支援共用。

## 何時可以使用倒回功能？

### 解答

復原是首要任務，目前正在開發中。 我們預計於2024年第3季或第4季發佈復原功能。

## 是否可選擇略過個別元件的促銷活動？ 在選項`Use Existing`、`Overwrite`和`Save with a new Name`存在的地方，可以新增`Skip`以跳過個別引數的升級？

### 解答


* 「使用現有」等同於「略過」或忽略部署，因為它對應到目標環境中的現有物件，而且不會進行任何變更。
* 若要略過物件，建議移除
不想從推進套件或直接從來源環境安裝的任何物件。 移除物件後，重新組裝封裝。

