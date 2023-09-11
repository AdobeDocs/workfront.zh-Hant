---
product-area: projects
navigation-topic: use-the-home-area
title: 從首頁區域建立工作專案
description: 從首頁區域建立工作專案
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: ecbba9b1da674328df866ec30e48fe44dd02cb86
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 0%

---

# 從首頁區域建立工作專案

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

您可以從以下位置建立工作專案： [!UICONTROL 首頁] 區域。 您可以自行建立個人任務、向其他使用者請求工作，或將任務新增到特定專案。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[！UICONTROL Worker]</p> <p><b>附註</b></p> 
   <p>如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[！UICONTROL Edit]或更新的任務存取權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立個人任務

您可以在「 」中建立您只能使用的個人工作 [!UICONTROL 首頁] 區域：

1. 按一下 **[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png) 按一下「 」 **[!UICONTROL 首頁]**.
1. 按一下 **[!UICONTROL 建立任務]** > **[!UICONTROL 個人]**.

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. 在 **[!UICONTROL 名稱]** 欄位，指定工作的名稱。
1. （選用）按一下 **[!UICONTROL 選取日期]**，然後選取任務到期的日期。 這會設定 [!UICONTROL 計畫完成日期] 用於任務。\
   您可以變更 **[!UICONTROL 計畫完成日期]** 按一下右側面板中的日期或編輯 **[!UICONTROL 此工作的完成日期為]** 日期直接在任務中。

1. 按一下 **[!UICONTROL 建立]** 以儲存任務。\
   任務已指派給您，並可在以下位置使用： [!UICONTROL 首頁] 區域。

>[!NOTE]
>
>* 當您建立個人任務時，該任務會儲存在「隱藏」的專案中，無法在中搜尋 [!UICONTROL Workfront]. 專案名為「&lt;使用者名稱>的任務」。 「使用者名稱」是建立任務之使用者的全名。 只有當您按一下中的個人任務時，才能存取此專案 [!UICONTROL 首頁] 區域，例如任務的階層連結。
>
>* 不同於一般專案任務，個人任務在Workfront介面中可見的欄位集有限，並且不會影響任何專案的時間表或進度。 將個人任務重新指派給另一個使用者，會將所有工作列位新增至個人任務，但該任務仍保留在建立該任務之使用者的個人專案上。
>
>
>* 個人任務只有在記錄時數或將其釘選到時程表時，才會顯示在時程表上。 您只能在為任務記錄小時數時將個人任務釘選到時程表中。 如需詳細資訊，請參閱 [記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md).
> 
>* 如果您想要將個人任務變成一般工作流程的一部分，建議您建立專案，並將任何個人任務移至專案。
>
> ![[!UICONTROL 個人任務的專案]](assets/createworkitems-personal--project-350x105.png)

## 請求其他使用者的工作

您可以直接從「首頁」區域向其他使用者要求工作。 如本節所述，當您向其他使用者請求工作時，在使用者點按之前，任務會作為請求顯示在使用者的首頁區域中 **[!UICONTROL 處理它]**.

若要向其他使用者要求工作，請執行下列步驟： [!UICONTROL 首頁] 區域：

1. 按一下 **[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png) 按一下「 」 **[!UICONTROL 首頁]**.
1. 按一下 **[!UICONTROL 建立任務]**，然後選取 **[!UICONTROL 請求]**.

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. 在 **[!UICONTROL 名稱]** 欄位，指定工作的名稱。
1. 在 **[!UICONTROL 指派給]** 欄位，開始輸入您要指派的使用者、專案團隊或角色名稱，然後按一下該名稱（當它出現在下拉式功能表中時）。
1. 在 [!UICONTROL 新增為] 下拉式選單，選擇是否要新增任務或問題。
1. 按一下 **[!UICONTROL 選取日期]**，然後選取任務到期的日期和時間。
1. 按一下 **[!UICONTROL 建立]** 以儲存任務。\
   任務會顯示為中的工作請求 [!UICONTROL 首頁] 您所指定使用者的區域。

## 將任務或問題新增至專案

您可以直接從首頁區域將任務或問題新增到現有專案：

1. 按一下 **[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png) 按一下「 」 **首頁**.
1. 按一下 **[!UICONTROL 建立任務]**，然後選取 **[!UICONTROL 專案任務]**.

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. 在 **[!UICONTROL 名稱]** 欄位，指定任務或問題的名稱。
1. 在 **[!UICONTROL 指派給]** 欄位，開始輸入您要指派的使用者、專案團隊或角色名稱，然後按一下該名稱（當它出現在下拉式功能表中時）。
1. 開始輸入您要建立任務或問題的專案名稱，然後在名稱出現在下拉式選單中時按一下該名稱。

   >[!IMPORTANT]
   >
   >任務或問題會顯示在 [!UICONTROL 工作清單] 僅限專案時 [!UICONTROL 狀態] 設為 [!UICONTROL 目前].

1. （視條件而定）若要建立問題，請選取 **[!UICONTROL 問題]** 從 **[!UICONTROL 新增為]** 下拉式功能表。 根據預設， **[!UICONTROL 任務]** 已選取。

1. 按一下 **[!UICONTROL 選取日期]**，然後選取任務到期的日期和時間。
1. 按一下 **[!UICONTROL 建立]** 以儲存任務。
