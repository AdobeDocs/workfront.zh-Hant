---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 設定問題的完成按鈕
description: 完成按鈕可以自動設定任務或問題的狀態。 依預設，當受指派人在工作專案上按一下「完成」時，Adobe Workfront會將問題標示為「已解決」。
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 1%

---

# 設定問題的[!UICONTROL 完成]按鈕

[!UICONTROL 完成]按鈕可以自動設定任務或問題的狀態。 依預設，當受指派人按一下其工作專案上的[!UICONTROL 完成]時，[!DNL Adobe Workfront]會將問題標示為[!UICONTROL 已解決]。

## 概觀

具有特定許可權的使用者可以設定[!UICONTROL Done]按鈕，以反映系統中的特定狀態。 針對[!DNL Workfront]中的問題，[!UICONTROL Done]按鈕有3種不同的運作方式：

* 如果使用者擁有指派的[!UICONTROL 主團隊]、[!DNL Workfront]管理員或具有[!UICONTROL 計畫]授權的使用者可以設定[!UICONTROL 完成]按鈕以反映團隊成員的特定狀態。 請參閱本文中的[設定團隊](#configure-the-uicontrol-done-button-for-a-team)的[!UICONTROL 完成]按鈕。
* 如果使用者沒有[!UICONTROL 主團隊]，但他們的設定檔中有[!UICONTROL 其他團隊]，Workfront會搜尋與使用者相關聯之任何團隊上的[!UICONTROL 完成]按鈕設定。 選擇是隨機的，與任何團隊相關聯的狀態會用於問題。
* 如果使用者未指派[!UICONTROL 主團隊]，則問題的[!UICONTROL Done]按鈕會繫結至系統產生的[!UICONTROL Resolved]狀態，該狀態具有三個字母的代碼[!UICONTROL RLV]。 此情境中沒有可用的設定選項。 [!UICONTROL Done]按鈕會自動預設為此狀態。
* 如果刪除[!UICONTROL 已解決] ([!UICONTROL RLV])狀態，且將問題標示為[!UICONTROL 完成]的使用者沒有[!UICONTROL 主團隊]，則預設問題狀態會繫結至指派給問題所屬專案之群組的[!UICONTROL 已關閉]預設值。 Workfront管理員可為群組設定系統範圍的預設設定。 請參閱本文[!UICONTROL 已解決]狀態被刪除時[設定[!UICONTROL 完成]按鈕](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>當刪除已解析狀態時，需要系統管理員存取權才能設定完成按鈕</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定團隊的[!UICONTROL 完成]按鈕

您可以使用[!UICONTROL 完成]按鈕變更套用到工作專案的狀態。 您也可以設定多個狀態，並允許使用者選擇適當的狀態。

{{step1-to-team}}

1. 按一下「**[!UICONTROL 切換群組]**」圖示，然後從下拉式功能表中選取新群組或在搜尋列中搜尋群組。
1. 按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表，然後按一下&#x200B;**[!UICONTROL 編輯]**。
1. 尋找&#x200B;**[!UICONTROL 團隊設定]**&#x200B;頁面底部的&#x200B;**[!UICONTROL 完成按鈕]**&#x200B;區段。

1. 為每個工作專案型別選取一個狀態或多個狀態。

   >[!NOTE]
   >
   >選擇任務或問題的狀態時，請考慮以下事項：
   >
   >* 當您為每種型別的工作專案選擇一個狀態時，當使用者按一下其專案上的[!UICONTROL 完成]時，任務或問題狀態會設定為該狀態。 如果您為每種型別的工作專案設定多個狀態，則會在[!UICONTROL 完成]按鈕中新增下拉式功能表，使用者必須挑選狀態才能變更工作專案的狀態。
   >* 您只能將系統層級狀態與[!UICONTROL 完成]按鈕建立關聯。 您無法將群組特定狀態與工作專案狀態建立關聯。
   >* 當指派給專案的使用者將專案置於與[!UICONTROL 完成]按鈕關聯的狀態時，無論您選取的狀態是[!UICONTROL 已完成]、[!UICONTROL 已關閉]狀態還是工作狀態，該專案都顯示該使用者的[!UICONTROL 完成]。
   >   
   >   
   >  例如，將[!UICONTROL Done]按鈕與In Progress產生關聯，會使工作專案顯示為[!UICONTROL Done] （針對將狀態從New變更為In的使用者）。
   >   
   >* 問題型別可自訂，其名稱可能與您的環境中下列清單不同。\
   >  以下是預設任務和問題型別：
   >     
   >   * [!UICONTROL 任務]
   >   * [!UICONTROL 問題]
   >   * [!UICONTROL 請求]
   >   * [!UICONTROL 變更順序]
   >   * [!UICONTROL 錯誤報告]

   如果任務或問題指派給多個使用者，除了為您的團隊選擇的多個狀態外，您會在下拉式選單中看到「[!UICONTROL 完成我的部分]」選項。

1. 按一下「**[!UICONTROL 儲存變更]**」。

## 將使用者與主團隊建立關聯

若要讓使用者看得見[!UICONTROL 完成]按鈕功能的變更，您可以讓變更使用者主團隊設定的團隊。

若要將使用者與主團隊建立關聯：

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**[!UICONTROL 使用者]**，然後選取您要與主團隊建立關聯的一或多個使用者。
1. 按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表，然後選取&#x200B;**[!UICONTROL 編輯]**。\
   ![](assets/user-settings-nwe-350x291.png)

1. 在&#x200B;**[!UICONTROL 組織]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 主團隊]**&#x200B;欄位。 開始輸入您想要與使用者建立關聯的團隊名稱。 當您在清單中看到團隊名稱時，請按一下該團隊的名稱。

1. 按一下「**[!UICONTROL 儲存變更]**」。\
   您選取的使用者現在與主團隊相關聯。
這些使用者現在可以看到任何團隊設定，包括與[!UICONTROL 完成]按鈕相關聯的狀態。

## 在刪除[!UICONTROL 已解決]狀態時設定[!UICONTROL 完成]按鈕

如果使用者沒有主團隊，而且已刪除[!UICONTROL 已解決] ([!UICONTROL RLV])的全系統預設值，[!DNL Workfront]管理員可以為專案上的群組設定[!UICONTROL 已關閉]狀態。 當使用者按一下[!DNL Done]按鈕時，[!DNL Workfront]會為已關閉的問題選取此狀態。

### 尋找與專案相關聯的群組

當使用者建立專案時，其主群組會自動指派給專案。 擁有專案[!UICONTROL 管理]存取權的使用者可以隨時在[!UICONTROL 專案詳細資料]區段中變更此群組。 若要瞭解此案例中[!DNL Workfront]對已完成問題使用的狀態，您必須瞭解問題所在專案的關聯群組，以及此群組對問題具有的[!UICONTROL 已關閉]預設狀態。

若要尋找與專案相關聯的群組：

1. 前往專案。
1. 在頁面左側，按一下&#x200B;**[!UICONTROL 專案詳細資料]**。
1. 找到&#x200B;**[!UICONTROL 專案關聯]**&#x200B;區段，然後找到&#x200B;**[!UICONTROL 群組]**。\
   這是您需要用來檢查「設定」區域中狀態的群組名稱。 如需有關如何更新特定群組預設狀態的指示，請參閱下節。

### 更新特定群組的預設狀態

作為[!UICONTROL Workfront]管理員，您可以更新特定群組的狀態：

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。
1. 在左側面板中，按一下&#x200B;**[!UICONTROL 專案偏好設定]**，然後按&#x200B;**[!UICONTROL 狀態]**。

1. 按一下&#x200B;**[!UICONTROL 問題]**，然後在右側的&#x200B;**[!UICONTROL 系統狀態]**&#x200B;搜尋方塊中輸入群組名稱。

1. 選取群組。
1. 按一下&#x200B;**[!UICONTROL 設定預設狀態]**&#x200B;下拉式功能表，然後選擇[!UICONTROL 已關閉]的預設狀態。 當使用者按一下[!UICONTROL 完成]按鈕時，[!DNL Workfront]會針對已關閉問題使用此狀態。

   >[!IMPORTANT]
   >
   >只有當使用者未獲指派主團隊且[!UICONTROL RLV]狀態已被刪除時，才會使用此狀態。

1. 按一下「**[!UICONTROL 儲存]**」。
