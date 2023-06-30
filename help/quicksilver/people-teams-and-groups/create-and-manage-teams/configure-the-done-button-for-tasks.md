---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 設定任務的「完成」按鈕
description: 完成按鈕可以自動設定任務或問題的狀態。 根據預設，當受指派人在其工作專案上按一下「完成」時，Adobe Workfront會將任務標示為「已完成」。
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# 設定 [!UICONTROL 完成] 任務按鈕

此 [!UICONTROL 完成] 按鈕可自動設定任務或問題的狀態。 依預設， [!UICONTROL Adobe Workfront] 將任務標籤為 [!UICONTROL 已完成] 當受指派人按一下其工作專案上的「完成」時。

## 總覽

具有特定許可權的使用者可以設定 [!UICONTROL 完成] 按鈕來反映系統中的特定狀態。 有兩種不同的方式 [!UICONTROL 完成] 按鈕適用於中的任務 [!UICONTROL Workfront]：

* 如果使用者擁有指派的主團隊， [!DNL Workfront] 具有下列專案的管理員或使用者： [!UICONTROL 計畫] 授權可設定 [!UICONTROL 完成] 按鈕來反映專案團隊成員的特定狀態。 另請參閱 [設定 [!UICONTROL 完成] 團隊按鈕](#configure-the-uicontrol-done-button-for-a-team) 本文章內容。
* 如果使用者沒有 [!UICONTROL 主團隊]，但有 [!UICONTROL 其他團隊] Workfront會在其設定檔中搜尋 [!UICONTROL 完成] 任何與使用者相關聯的團隊上的按鈕。 選擇是隨機的，且與任何團隊關聯的狀態用於任務。
* 如果使用者沒有指派主團隊， [!UICONTROL 完成] 任務的按鈕會繫結到完成狀態。 此情境中沒有可用的設定選項。 此 [!UICONTROL 完成] 按鈕會自動預設為此狀態。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] 計劃*</strong></p></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] 授權*</strong></p></td> 
   <td> <p>[！UICONTROL計畫] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫或授權型別，請連絡 [!DNL Workfront] 管理員。

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
   >  例如，關聯 [!UICONTROL 完成] 按鈕與 [!UICONTROL 進行中] 導致工作專案顯示為 [!UICONTROL 完成] 適用於變更狀態的使用者 [!UICONTROL 新增] 至 [!UICONTROL 進行中].
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
任何團隊設定，包括和關聯的狀態 [!UICONTROL 完成] 按鈕現在對這些使用者可見。
