---
product-area: projects
navigation-topic: use-the-home-area
title: 在首頁區域將專案標示為完成
description: 如果您是任務或問題受指派人，可將任務或問題標示為已完成。 將任務或問題標籤為「完成」時，任務或問題的狀態會變更為「完成」。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# 在[!UICONTROL 首頁]區域將專案標示為[!UICONTROL 完成]

如果您是任務或問題受指派人，可將任務或問題標示為已完成。 將任務或問題標籤為[!UICONTROL 完成]時，任務或問題的狀態會變更為[!UICONTROL 完成]。

>[!NOTE]
>
>除非您是指派給任務或問題的資源之一，否則您不會看到[!UICONTROL 完成]按鈕。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>[！UICONTROL編輯]對任務和問題的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>您需要處理的任務和問題的Contribute許可權或更高版本</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 將任務或問題標示為[!UICONTROL 完成]

只有指派給任務或問題的使用者可以將其標籤為[!UICONTROL 完成]。

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 在&#x200B;**[!UICONTROL 工作清單]**&#x200B;中，找出任何等待處理的專案。
1. 執行下列任一項作業：

* 在工作專案上按一下&#x200B;**[!UICONTROL 完成]**。\
   請參閱[瞭解[!UICONTROL 完成]按鈕的選項](#understand-the-options-of-the-done-button)，以取得此按鈕可能如何出現的詳細資訊。

* 選取您要標示為完成的專案，然後在右側面板中按一下&#x200B;**[!UICONTROL 更新狀態]**，然後將專案的狀態變更為等於[!UICONTROL 完成]或[!UICONTROL 已關閉]的狀態。

## 瞭解[!UICONTROL 完成]按鈕的選項

依預設，按一下工作專案上的[!UICONTROL 完成]按鈕會將該專案的狀態變更為[!UICONTROL 完成] （工作）或[!UICONTROL 已解決] （問題）。

您的[!DNL Adobe Workfront]管理員可以自訂與[!UICONTROL 完成]按鈕關聯的狀態，並將這些自訂套用至您的主團隊。

視與[!UICONTROL 完成]按鈕關聯的狀態數，或指派給任務或問題的資源數而定，[!UICONTROL 完成]按鈕的外觀可能會變更。

* [與一個狀態關聯的[!UICONTROL 完成]按鈕](#done-button-associated-with-one-status)
* [與多個狀態關聯的[!UICONTROL 完成]按鈕](#done-button-associated-with-multiple-statuses)
* [指派給多個資源的專案的[!UICONTROL 完成]按鈕](#done-button-for-items-assigned-to-multiple-resources)

### 與一個狀態關聯的[!UICONTROL 完成]按鈕

當[!UICONTROL Done]按鈕與一個狀態相關聯，且工作專案僅指派給您時，按鈕會顯示&#x200B;**[!UICONTROL Done]**。 按一下後，任務或問題的狀態會變更為與[!UICONTROL 完成]按鈕相關的狀態。

![完成按鈕](assets/Done.png)

若要瞭解哪個狀態與[!UICONTROL 完成]按鈕相關聯，請檢查[!UICONTROL 完成按鈕]區段您主團隊的[!UICONTROL 團隊設定]，如[編輯團隊設定](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)中所述。

如果您未指派給主團隊，按一下[!UICONTROL 完成]時會選擇預設狀態，如上所述[瞭解[!UICONTROL 完成]按鈕](#understand-the-options-of-the-done-button)的選項。

### 與多個狀態關聯的[!UICONTROL 完成]按鈕

當[!UICONTROL Done]按鈕與多個狀態關聯時，按鈕會顯示單字&#x200B;**[!UICONTROL Done]**，後面接著下拉式功能表。 在此案例中，您無法按一下[!UICONTROL 完成]。 您必須從下拉式選單中選取狀態。 選取最適合工作專案完成的狀態。 這樣做會變更工作專案的狀態。

若要瞭解如何將多個狀態與[!UICONTROL Done]按鈕相關聯，請參閱[設定任務的[!UICONTROL Done]按鈕](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)和[設定問題的[!UICONTROL Done]按鈕](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)。

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### 指派給多個資源的專案的[!UICONTROL 完成]按鈕

將任務或問題指派給多個資源時，按鈕會顯示單字&#x200B;**[!UICONTROL 完成]**，後面接著下拉式功能表。 在下拉式功能表中，您可以選擇在&#x200B;**[!UICONTROL 完成我的部分]** （讓團隊成員知道您已完成您的一部份工作）或與[!UICONTROL 完成]按鈕（完成專案）相關的狀態之間選擇。 選取&#x200B;**[!UICONTROL 完成我的零件]**&#x200B;後，工作專案會從您的工作清單中移除，但會保留在那些仍指派給工作專案的工作清單中。\
如果「完成」按鈕與多個狀態相關聯，它們會列在「完成我的零件」****&#x200B;下。

>[!NOTE]
>
>在具有多個受指派人的任務或問題上，每個使用者負責指出其在任務或問題上的指派實際上已完成。 因此，每個受指派人都必須按一下「[!UICONTROL 完成]」才能顯示他們已完成指派給專案上的工作。

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
