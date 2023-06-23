---
product-area: projects
navigation-topic: use-the-home-area
title: 從首頁區域建立工作專案
description: 從首頁區域建立工作專案
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 3793f68faf2ec0a8050f8f0c6e06a32579b43879
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 從首頁區域建立工作專案

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

您可以從以下位置建立工作專案： [!UICONTROL 首頁] 區域。 您可以自行建立個人任務、向其他使用者請求工作，或向特定專案新增任務。

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
   <td> <p>[！UICONTROL Worker]</p> <p>注意：如果您仍然沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需如何進行 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[！UICONTROL Edit]或更新的工作存取權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立個人任務

您可以建立只有您才能使用的個人任務，位於 [!UICONTROL 首頁] 區域：

1. 按一下 **[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png) 然後按一下 **[!UICONTROL 首頁]**.
1. 按一下 **[!UICONTROL 新增任務]** > **[!UICONTROL 個人]**.

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. 在 **[!UICONTROL 名稱]** 欄位中，指定工作的名稱。
1. （可選）按一下 **[!UICONTROL 選取日期]**，然後選取任務的到期日。 這會設定 [!UICONTROL 計畫完成日期] 用於任務。\
   您可以變更 **[!UICONTROL 計畫完成日期]** 按一下右側面板中的日期或編輯 **[!UICONTROL 完成日期為]** 日期直接在任務中。

1. 按一下 **[!UICONTROL 建立]** 以儲存任務。\
   任務已指派給您，並可在以下位置找到： [!UICONTROL 首頁] 區域。

>[!NOTE]
>
>* 當您建立個人任務時，它會儲存在無法搜尋的「隱藏」專案中 [!UICONTROL Workfront]. 專案名為「&lt;使用者名稱>的任務」。 「使用者名稱」是建立任務之使用者的全名。 只有當您按一下中的個人任務時，才能存取此專案 [!UICONTROL 首頁] 區域，例如任務的階層連結。
>
>* 與一般專案任務不同，個人任務在Workfront介面中可見的欄位集有限，並且不會影響任何專案的時間表或進度。 將個人任務重新指派給另一個使用者，會將所有工作列位新增至個人任務，但任務仍會保留在建立任務之使用者的個人專案上。
>
>* 如果您想要將個人任務變成一般工作流程的一部分，建議您建立專案，並將任何個人任務移動至專案。
>
> ![[!UICONTROL 個人任務的專案]](assets/createworkitems-personal--project-350x105.png)

## 請求其他使用者的工作

您可以直接從「首頁」區域向其他使用者要求工作。 如本節所述，當您向其他使用者請求工作時，任務會作為請求顯示在使用者的「首頁」區域中，直到使用者點按為止 **[!UICONTROL 處理它]**.

若要向其他使用者要求工作，請 [!UICONTROL 首頁] 區域：

1. 按一下 **[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png) 然後按一下 **[!UICONTROL 首頁]**.
1. 按一下 **[!UICONTROL 新增任務]**，然後選取 **[!UICONTROL 請求]**.

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. 在 **[!UICONTROL 名稱]** 欄位中，指定工作的名稱。
1. 在 **[!UICONTROL 指派給]** 欄位，開始輸入您要指派的使用者、專案團隊或角色名稱，然後在其出現在下拉式選單中時按一下該名稱。
1. 在 [!UICONTROL 新增為] 下拉式功能表，選取是否要新增任務或問題。
1. 按一下 **[!UICONTROL 選取日期]**，然後選取任務到期的日期和時間。
1. 按一下 **[!UICONTROL 建立]** 以儲存任務。\
   任務會顯示為工作請求，位於 [!UICONTROL 首頁] 您所指定使用者的區域。

## 將任務或問題新增至專案

您可以直接從首頁區域將任務或問題新增到現有專案：

1. 按一下 **[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png) 然後按一下 **首頁**.
1. 按一下 **[!UICONTROL 新增任務]**，然後選取 **[!UICONTROL 專案任務]**.

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. 在 **[!UICONTROL 名稱]** 欄位中，指定任務或問題的名稱。
1. 在 **[!UICONTROL 指派給]** 欄位，開始輸入您要指派的使用者、專案團隊或角色名稱，然後在其出現在下拉式選單中時按一下該名稱。
1. 開始輸入您要建立任務或問題的專案名稱，然後在名稱出現在下拉式選單中時按一下該名稱。

   >[!IMPORTANT]
   >
   >任務或問題會顯示在 [!UICONTROL 工作清單] 僅當專案時 [!UICONTROL 狀態] 設為 [!UICONTROL 目前].

1. （視條件而定）若要建立問題，請選取 **[!UICONTROL 問題]** 從 **[!UICONTROL 新增為]** 下拉式功能表。 依預設， **[!UICONTROL 任務]** 「 」已選取。

1. 按一下 **[!UICONTROL 選取日期]**，然後選取任務到期的日期和時間。
1. 按一下 **[!UICONTROL 建立]** 以儲存任務。
