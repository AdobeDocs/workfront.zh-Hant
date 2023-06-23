---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 設定問題的完成按鈕
description: 完成按鈕可以自動設定任務或問題的狀態。 根據預設，當受指派人在其工作專案上按一下「完成」時，Adobe Workfront會將問題標示為「已解決」。
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 3793f68faf2ec0a8050f8f0c6e06a32579b43879
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 1%

---

# 設定 [!UICONTROL 完成] 問題的按鈕

此 [!UICONTROL 完成] 按鈕可自動設定任務或問題的狀態。 依預設， [!DNL Adobe Workfront] 將問題標籤為 [!UICONTROL 已解決] 當受指派人按一下 [!UICONTROL 完成] 在其工作專案上。

## 總覽

具有特定許可權的使用者可以設定 [!UICONTROL 完成] 按鈕來反映系統中的特定狀態。 有3種不同的方式 [!UICONTROL 完成] 按鈕適用於中的問題 [!DNL Workfront]：

* 如果使用者已指派 [!UICONTROL 主團隊]， a [!DNL Workfront] 具有下列專案的管理員或使用者： [!UICONTROL 計畫] 授權可設定 [!UICONTROL 完成] 按鈕來反映專案團隊成員的特定狀態。 另請參閱 [設定 [!UICONTROL 完成] 團隊按鈕](#configure-the-uicontrol-done-button-for-a-team) 本文章內容。
* 如果使用者沒有 [!UICONTROL 主團隊]，但有[!UICONTROL 其他團隊] Workfront會在其設定檔中搜尋 [!UICONTROL 完成] 任何與使用者相關聯的團隊上的按鈕。 選擇是隨機的，且與任何團隊相關聯的狀態會用於問題。
* 如果使用者沒有 [!UICONTROL 主團隊] 已指派， [!UICONTROL 完成] 問題的按鈕已繫結至系統產生的 [!UICONTROL 已解決] 具有三個字母代碼的狀態 [!UICONTROL RLV]. 此情境中沒有可用的設定選項。 此 [!UICONTROL 完成] 按鈕會自動預設為此狀態。
* 如果 [!UICONTROL 已解決] ([!UICONTROL RLV])狀態已刪除，且使用者將問題標示為 [!UICONTROL 完成] 沒有 [!UICONTROL 主團隊]，預設問題狀態會繫結至設為預設的任何專案 [!UICONTROL 已關閉] 對於指派給問題所屬專案的群組。 Workfront管理員可以為群組設定系統範圍的預設設定。 另請參閱 [設定 [!UICONTROL 完成] 按鈕時 [!UICONTROL 已解決] 已刪除狀態](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) 本文章內容。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>[！UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td>刪除[！UICONTROL已解決]狀態時，需要系統管理員存取權才能設定[！UICONTROL完成]按鈕</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 設定 [!UICONTROL 完成] 團隊按鈕

您可以使用變更將哪個狀態套用到工作專案 [!UICONTROL 完成] 按鈕。 您也可以設定多個狀態，並允許使用者選擇適當的狀態。

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 切換群組]** 圖示，然後從下拉式選單中選取新專案團隊，或在搜尋列中搜尋專案團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後按一下 **[!UICONTROL 編輯]**.
1. 尋找 **[!UICONTROL 完成按鈕]** 底部的 **[!UICONTROL 團隊設定]** 頁面。

1. 為每個工作專案型別選取一個狀態或多個狀態。

   >[!NOTE]
   >
   >選擇任務或問題的狀態時，請考慮以下事項：
   >
   >* 當您為每種型別的工作專案選擇一個狀態時，任務或問題狀態會在使用者點選時設定為該狀態 [!UICONTROL 完成] 在他們的專案上。 如果您為每種型別的工作專案設定了多種狀態，則會將下拉式功能表新增至 [!UICONTROL 完成] 按鈕和使用者必須挑選一個狀態來變更工作專案的狀態。
   >* 您只能將系統層級狀態與 [!UICONTROL 完成] 按鈕。 您無法將群組特定狀態與工作專案狀態建立關聯。
   >* 當指派給專案的使用者將專案置於與關聯的狀態時 [!UICONTROL 完成] 按鈕，專案顯示為 [!UICONTROL 完成] 為該使用者設定，無論您選取的狀態是否為 [!UICONTROL 已完成] 或 [!UICONTROL 已關閉] 狀態或工作狀態。
   >   
   >   
   >  例如，關聯 [!UICONTROL 完成] 具有進行中的按鈕使工作專案顯示為 [!UICONTROL 完成] 適用於將狀態從新變更為進行中的使用者。
   >   
   >* 問題型別是可自訂的，其名稱可能與以下列出的您的環境不同。\
   >  以下是預設任務和問題型別：
   >     
   >   * [!UICONTROL 任務]
   >   * [!UICONTROL 問題]
   >   * [!UICONTROL 請求]
   >   * [!UICONTROL 變更順序]
   >   * [!UICONTROL 錯誤報告]

   如果任務或問題指派給多個使用者，您會看到「[!UICONTROL 完成我的部分]」選項，以及為您的團隊選擇的多種狀態。

1. 按一下 **[!UICONTROL 儲存變更]**.

## 將使用者與主團隊建立關聯

若要變更 [!UICONTROL 完成] 按鈕功能對使用者可見，您可以使變更其設定的團隊成為使用者的主團隊。

若要將使用者與主團隊建立關聯，請執行下列動作：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront].

1. 按一下 **[!UICONTROL 使用者]**，然後選取您要與主團隊建立關聯的一或多位使用者。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後選取 **[!UICONTROL 編輯]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 在 **[!UICONTROL 組織]** 區段，選取 **[!UICONTROL 主團隊]** 欄位。 開始輸入您想要與使用者建立關聯的設定所在團隊的名稱。 當您在清單中看到團隊名稱時，請按一下該團隊名稱。

1. 按一下 **[!UICONTROL 儲存變更]**.\
   您選取的使用者現在與主團隊相關聯。
任何團隊設定，包括和關聯的狀態 [!UICONTROL 完成] 按鈕，現在對這些使用者可見。

## 設定 [!UICONTROL 完成] 按鈕時 [!UICONTROL 已解決] 已刪除狀態

如果使用者沒有主團隊和系統範圍的預設值 [!UICONTROL 已解決] ([!UICONTROL RLV])已刪除，a [!DNL Workfront] 管理員可以設定 [!UICONTROL 已關閉] 專案上的群組狀態。 [!DNL Workfront] 當使用者按一下 [!DNL Done] 按鈕。

### 尋找與專案相關聯的群組

當使用者建立專案時，其主群組會自動指派給專案。 使用者： [!UICONTROL 管理] 存取專案可以在以下位置變更此群組： [!UICONTROL 專案詳細資訊] 區段。 瞭解什麼狀態 [!DNL Workfront] 在此情況下，使用完成的問題時，您必須瞭解問題所在群組和預設狀態為何，並與專案相關聯 [!UICONTROL 已關閉] 此群組遇到問題。

若要尋找與專案相關聯的群組，請執行下列動作：

1. 前往專案。
1. 在頁面左側，按一下 **[!UICONTROL 專案詳細資訊]**.
1. 找到 **[!UICONTROL 專案關聯]** 區段，然後尋找 **[!UICONTROL 群組]**.\
   這是您需要用來檢查「設定」區域中狀態的群組名稱。 如需有關如何更新特定群組預設狀態的指示，請參閱以下章節。

### 更新特定群組的預設狀態

As a [!UICONTROL Workfront] 管理員，您可以更新特定群組的狀態：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 在左側面板中，按一下 **[!UICONTROL 專案偏好設定]**，則 **[!UICONTROL 狀態]**.

1. 按一下 **[!UICONTROL 問題]**，然後輸入群組的名稱 **[!UICONTROL 系統狀態]** 搜尋方塊。

1. 選取群組。
1. 按一下 **[!UICONTROL 設定預設狀態]** 下拉式功能表，然後選擇預設狀態 [!UICONTROL 已關閉]. [!DNL Workfront] 當使用者按一下 [!UICONTROL 完成] 按鈕。

   >[!IMPORTANT]
   >
   >只有當使用者沒有指派的主團隊和 [!UICONTROL RLV] 已刪除狀態。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
