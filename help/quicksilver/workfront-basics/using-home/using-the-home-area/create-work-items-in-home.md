---
product-area: projects
navigation-topic: use-the-home-area
title: 從首頁區域建立工作專案
description: 您可以從[!UICONTROL 首頁]區域建立工作專案。 您可以自行建立個人任務、向其他使用者請求工作，或將任務新增到特定專案。
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 從首頁區域建立工作專案

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

您可以從[!UICONTROL 首頁]區域建立工作專案。 您可以自行建立個人任務、向其他使用者請求工作，或將任務新增到特定專案。

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
   <p>如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否已在您的存取層級中設定其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[！UICONTROL Edit]或更新的任務存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 建立個人任務

您可以在[!UICONTROL 首頁]區域中建立僅供您使用的個人工作：

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 按一下&#x200B;**[!UICONTROL 新增工作]** > **[!UICONTROL 個人]**。

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. 在&#x200B;**[!UICONTROL 名稱]**&#x200B;欄位中，指定工作的名稱。
1. （選擇性）按一下&#x200B;**[!UICONTROL 選取日期]**，然後選取工作到期的日期。 這會設定任務的[!UICONTROL 計畫完成日期]。\
   您可以按一下右側面板中的日期或編輯&#x200B;**[!UICONTROL 直接在任務中完成]**&#x200B;日期，以變更&#x200B;**[!UICONTROL 規劃完成日期]**。

1. 按一下&#x200B;**[!UICONTROL 建立]**&#x200B;以儲存工作。\
   工作已指派給您，並可在[!UICONTROL 首頁]區域使用。

>[!NOTE]
>
>* 當您建立個人任務時，它會儲存在[!UICONTROL Workfront]中無法搜尋的「隱藏」專案中。 專案名為「&lt;使用者名稱>的任務」。 「使用者名稱」是建立任務之使用者的全名。 例如，只有在您從任務的階層連結按一下[!UICONTROL 首頁]區域中的個人任務時，才能存取此專案。
>
>* 不同於一般專案任務，個人任務在Workfront介面中可見的欄位集有限，並且不會影響任何專案的時間表或進度。 將個人任務重新指派給另一個使用者，會將所有工作列位新增至個人任務，但該任務仍保留在建立該任務之使用者的個人專案上。
>
>
>* 個人任務只有在記錄時數或將其釘選到時程表時，才會顯示在時程表上。 您只能在為任務記錄小時數時將個人任務釘選到時程表中。 如需詳細資訊，請參閱[記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md)。
> 
>* 如果您想要將個人任務變成一般工作流程的一部分，建議您建立專案，並將任何個人任務移至專案。
>
> ![[!UICONTROL 個人任務的專案]](assets/createworkitems-personal--project-350x105.png)

## 請求其他使用者的工作

您可以直接從「首頁」區域向其他使用者要求工作。 如本節所述，當您向其他使用者要求工作時，在使用者按一下&#x200B;**[!UICONTROL 處理它]**&#x200B;之前，工作會以要求形式顯示在使用者的[首頁]區域。

若要從[!UICONTROL 首頁]區域向其他使用者要求工作：

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 按一下&#x200B;**[!UICONTROL 新增工作]**，然後選取&#x200B;**[!UICONTROL 要求]**。

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. 在&#x200B;**[!UICONTROL 名稱]**&#x200B;欄位中，指定工作的名稱。
1. 在&#x200B;**[!UICONTROL 指派給]**&#x200B;欄位中，開始輸入您要指派的使用者、團隊或角色名稱，然後在其出現在下拉式功能表中時按一下該名稱。
1. 在[!UICONTROL 新增為]下拉式功能表中，選取是否要新增任務或問題。
1. 按一下&#x200B;**[!UICONTROL 選取日期]**，然後選取工作到期的日期和時間。
1. 按一下&#x200B;**[!UICONTROL 建立]**&#x200B;以儲存工作。\
   在您指定之使用者的[!UICONTROL 首頁]區域中，任務會顯示為工作要求。

## 將任務或問題新增至專案

您可以直接從首頁區域將任務或問題新增到現有專案：

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**首頁**。
1. 按一下&#x200B;**[!UICONTROL 新增任務]**，然後選取&#x200B;**[!UICONTROL 專案任務]**。

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. 在&#x200B;**[!UICONTROL 名稱]**&#x200B;欄位中，指定任務或問題的名稱。
1. 在&#x200B;**[!UICONTROL 指派給]**&#x200B;欄位中，開始輸入您要指派的使用者、團隊或角色名稱，然後在其出現在下拉式功能表中時按一下該名稱。
1. 開始輸入您要建立任務或問題的專案名稱，然後在名稱出現在下拉式選單中時按一下該名稱。

   >[!IMPORTANT]
   >
   >只有當專案[!UICONTROL 狀態]設定為[!UICONTROL 目前]時，任務或問題才會出現在[!UICONTROL 工作清單]上。

1. （視條件而定）若要建立問題，請從&#x200B;**[!UICONTROL 新增為]**&#x200B;下拉式功能表中選取&#x200B;**[!UICONTROL 問題]**。 預設會選取&#x200B;**[!UICONTROL 工作]**。

1. 按一下&#x200B;**[!UICONTROL 選取日期]**，然後選取工作到期的日期和時間。
1. 按一下&#x200B;**[!UICONTROL 建立]**&#x200B;以儲存工作。
