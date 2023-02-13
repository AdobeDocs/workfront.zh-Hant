---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 設定問題的「完成」按鈕
description: 「完成」按鈕可自動設定任務或問題的狀態。 依預設，當受託人按一下其工作項目的「完成」時，Adobe Workfront會將問題標示為「已解決」。
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 1%

---

# 設定 [!UICONTROL 完成] 問題按鈕

此 [!UICONTROL 完成] 按鈕可以自動設定任務或問題的狀態。 依預設， [!DNL Adobe Workfront] 將問題標示為 [!UICONTROL 已解決] 受託人點按 [!UICONTROL 完成] 工作項目上。

## 總覽

具有特定權限的使用者可以設定 [!UICONTROL 完成] 按鈕來反映系統中的某些狀態。 有3種不同的方式 [!UICONTROL 完成] 按鈕適用於 [!DNL Workfront]:

* 如果使用者已指派 [!UICONTROL 主隊], [!DNL Workfront] 管理員或使用 [!UICONTROL 計畫] 授權可設定 [!UICONTROL 完成] 按鈕來反映團隊成員的某些狀態。 請參閱 [設定 [!UICONTROL 完成] 按鈕](#configure-the-uicontrol-done-button-for-a-team) 這篇文章。
* 如果使用者沒有 [!UICONTROL 主隊] 指派， [!UICONTROL 完成] 問題按鈕會系結至系統產生的 [!UICONTROL 已解決] 具有三字母代碼的狀態 [!UICONTROL RLV]. 此情境中沒有可用的配置選項。 此 [!UICONTROL 完成] 按鈕自動預設為此狀態。
* 若 [!UICONTROL 已解決] ([!UICONTROL RLV])狀態，並將問題標示為 [!UICONTROL 完成] 無 [!UICONTROL 主隊]，則預設問題狀態會系結至設為的預設狀態 [!UICONTROL 已關閉] 針對指派給該問題所屬專案的群組。 Workfront管理員可以為群組設定全系統的預設設定。 請參閱 [設定 [!UICONTROL 完成] 按鈕 [!UICONTROL 已解決] 已刪除狀態](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) 這篇文章。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td>刪除[!UICONTROL已解析]狀態時，需要系統管理員訪問權限才能配置[!UICONTROL完成]按鈕</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 設定 [!UICONTROL 完成] 按鈕

您可以使用 [!UICONTROL 完成] 按鈕。 您也可以設定多個狀態，並允許使用者選擇適當的狀態。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 交換組]** 表徵圖，然後從下拉菜單中選擇新團隊，或在搜索欄中搜索團隊。
1. 按一下 **[!UICONTROL 更多]** ，然後按一下 **[!UICONTROL 編輯]**.
1. 尋找 **[!UICONTROL 完成按鈕]** 區段 **[!UICONTROL 團隊設定]** 頁面。

1. 為每個工作項類型選擇一個或多個狀態。

   >[!NOTE]
   >
   >為任務或問題選擇狀態時，請考慮以下事項：
   >
   >* 當您為每種類型的工作項目選擇一個狀態時，當用戶按一下時，任務或問題狀態將設定為該狀態 [!UICONTROL 完成] 在他們的項目上。 如果您為每種類型的工作項目設定多個狀態，則下拉式功能表會新增至 [!UICONTROL 完成] 按鈕和用戶必須選擇狀態才能更改工作項的狀態。
   >* 您只能將系統層級狀態與 [!UICONTROL 完成] 按鈕。 您不能將特定組狀態與工作項狀態關聯。
   >* 當被指派給項目的使用者將項目置於與 [!UICONTROL 完成] 按鈕，項目顯示為 [!UICONTROL 完成] 無論您選取的狀態是否為 [!UICONTROL 已完成] 或 [!UICONTROL 已關閉] 狀態或工作狀態。

   >   
   >   
   >  例如，將 [!UICONTROL 完成] 按鈕中的「 」將使工作項顯示為 [!UICONTROL 完成] 對於狀態從「新」更改為「正在」的用戶。
   >   
   >* 問題類型可自訂，其名稱可能與您環境中列出的名稱不同。\
      >  預設任務和問題類型如下：
      >     
      >   * [!UICONTROL 任務]
      >   * [!UICONTROL 問題]
      >   * [!UICONTROL 請求]
      >   * [!UICONTROL 變更順序]
      >   * [!UICONTROL 錯誤報告]


   如果將任務或問題分配給多個用戶，您會看到「[!UICONTROL 完成我的任務]」選項，以及為您的團隊選擇的多個狀態。

1. 按一下 **[!UICONTROL 儲存變更]**.

## 將使用者與首頁團隊關聯

若要變更 [!UICONTROL 完成] 按鈕功能對用戶可見，您可以讓您的設定更改了用戶的「主團隊」的團隊。

將用戶與主團隊關聯：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront].

1. 按一下 **[!UICONTROL 使用者]**，然後選擇要與主團隊關聯的用戶或組。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 在 **[!UICONTROL 組織]** 區段，選取 **[!UICONTROL 主隊]** 欄位。 開始鍵入要與用戶關聯的團隊的名稱。 在清單中看到團隊的名稱時，按一下該團隊的名稱。

1. 按一下 **[!UICONTROL 儲存變更]**.\
   您選取的使用者現在與首頁團隊相關聯。
任何團隊設定，包括與 [!UICONTROL 完成] 按鈕，則這些使用者現在可以看到。

## 設定 [!UICONTROL 完成] 按鈕 [!UICONTROL 已解決] 已刪除狀態

如果使用者沒有首頁團隊，且 [!UICONTROL 已解決] ([!UICONTROL RLV])已刪除， [!DNL Workfront] 管理員可以 [!UICONTROL 已關閉] 項目上的組的狀態。 [!DNL Workfront] 當使用者按一下 [!DNL Done] 按鈕。

### 查找與項目關聯的組

使用者建立專案時，其「首頁群組」會自動指派給專案。 具有 [!UICONTROL 管理] 專案的存取權可在 [!UICONTROL 專案詳細資料] 區段。 了解狀態 [!DNL Workfront] 在此情況下，您必須了解與問題所在的項目關聯的組以及的預設狀態 [!UICONTROL 已關閉] 此組有問題。

要查找與項目關聯的組，請執行以下操作：

1. 前往專案。
1. 在頁面左側，按一下 **[!UICONTROL 專案詳細資料]**.
1. 找出 **[!UICONTROL 專案關聯]** 部分，然後查找 **[!UICONTROL 群組]**.\
   這是您在「設定」區域中檢查狀態時需要使用的群組名稱。 請參閱下節，了解如何更新特定群組的預設狀態。

### 更新特定組的預設狀態

As a [!UICONTROL Workfront] 管理員，您可以更新特定群組的狀態：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 在左側面板中，按一下 **[!UICONTROL 專案偏好設定]**，然後 **[!UICONTROL 狀態]**.

1. 按一下 **[!UICONTROL 問題]**，然後在 **[!UICONTROL 系統狀態]** 搜尋方塊。

1. 選取群組。
1. 按一下 **[!UICONTROL 設定預設狀態]** 下拉式功能表，然後選擇的預設狀態 [!UICONTROL 已關閉]. [!DNL Workfront] 使用者按一下 [!UICONTROL 完成] 按鈕。

   >[!IMPORTANT]
   >
   >只有在用戶未分配主團隊和 [!UICONTROL RLV] 狀態已刪除。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
