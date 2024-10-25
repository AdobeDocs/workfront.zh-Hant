---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 設定任務的「完成」按鈕
description: 完成按鈕可以自動設定任務或問題的狀態。 依預設，當受指派人按一下其工作專案上的「完成」時，Adobe Workfront會將任務標示為「已完成」。
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# 設定任務的[!UICONTROL 完成]按鈕

[!UICONTROL 完成]按鈕可以自動設定任務或問題的狀態。 依預設，當受指派人在工作專案上按一下「標籤為完成」時，[!UICONTROL Adobe Workfront]會將工作標籤為[!UICONTROL 已完成]。

>[!NOTE]
>
>「完成」按鈕在Workfront的所有區域顯示為「標示為完成」 。

## 概觀

具有特定許可權的使用者可以設定[!UICONTROL Done]按鈕，使其與系統中的特定狀態產生關聯。 在[!UICONTROL Workfront]中，[!UICONTROL Done]按鈕有兩種不同的工作方式：

* 如果使用者擁有指派的主團隊，[!DNL Workfront]管理員或具有[!UICONTROL 計畫]授權的使用者可以設定[!UICONTROL 完成]按鈕以反映團隊成員的特定狀態。 請參閱本文中的[設定團隊](#configure-the-uicontrol-done-button-for-a-team)的[!UICONTROL 完成]按鈕。
* 如果使用者沒有[!UICONTROL 主團隊]，但他們的設定檔中有[!UICONTROL 其他團隊]，Workfront會搜尋與使用者相關聯之任何團隊上的[!UICONTROL 完成]按鈕設定。 選擇是隨機的，與任何團隊關聯的狀態用於任務。
* 如果使用者沒有指派主團隊，則任務的[!UICONTROL 完成]按鈕會繫結到完成狀態。 此情境中沒有可用的設定選項。 [!UICONTROL Done]按鈕會自動預設為此狀態。

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
   >  例如，將[!UICONTROL Done]按鈕與[!UICONTROL In Progress]建立關聯，會讓狀態從[!UICONTROL New]變更為[!UICONTROL In progress]的使用者，將工作專案顯示為[!UICONTROL Done]。
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
1. 按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表，然後按一下&#x200B;**[!UICONTROL 編輯]**。\
   ![](assets/user-settings-nwe-350x291.png)

1. 在&#x200B;**[!UICONTROL 組織]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 主團隊]**&#x200B;欄位。 開始輸入您想要與使用者建立關聯的團隊名稱。 當您在清單中看到團隊名稱時，請按一下該團隊的名稱。

1. 按一下「**[!UICONTROL 儲存變更]**」。\
   您選取的使用者現在與主團隊相關聯。
這些使用者現在可以看到任何團隊設定，包括與[!UICONTROL 完成]按鈕相關聯的狀態。
