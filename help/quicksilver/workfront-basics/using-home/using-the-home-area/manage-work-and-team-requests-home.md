---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: 管理首頁區域的工作和團隊請求
description: 當工作任務和問題指派給您時，它們會列在[!UICONTROL 首頁]區域的[!UICONTROL 工作清單]中。 您可以檢視、重新指派、回覆、處理或移除請求。 [!UICONTROL 首頁]區域中的工作請求不限於與請求佇列關聯的問題。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# 管理[!UICONTROL 首頁]區域的工作和團隊請求

當工作任務和問題指派給您時，它們會列在[!UICONTROL 首頁]區域的[!UICONTROL 工作清單]中。 您可以檢視、重新指派、回覆、處理或移除請求。 [!UICONTROL 首頁]區域中的工作請求不限於與請求佇列關聯的問題。

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

## 檢視工作要求

指派給您的工作請求會顯示在[!UICONTROL 首頁]的左側面板中。 您可以使用[!UICONTROL 工作清單]頂端的篩選器，設定在[!UICONTROL 首頁]中顯示哪些要求。

您可以選取篩選器，以顯示準備好要處理的專案或您目前處理的專案。

本文說明如何使用[!UICONTROL 首頁]區域中的篩選器，以檢視您目前正在處理或可能考慮開始處理的專案。 如需[!UICONTROL 首頁]區域中所有篩選器的相關資訊，請參閱[在[!UICONTROL 首頁]區域](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)的工作清單中顯示專案。

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 按一下&#x200B;**[!UICONTROL 篩選器]**&#x200B;下拉式功能表。

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. 按一下以下任一或兩個選項以取得工作：

   **[!UICONTROL 準備開始]：**&#x200B;僅顯示準備開始的任務和問題。 下列兩個陳述式都必須為true：

   * 任務及其父項沒有前置任務或任務限制而無法處理。
   * 任務或問題的[!UICONTROL 規劃開始日期]是過去或最多未來兩週。

   **[!UICONTROL 未就緒]**：僅顯示尚未準備開始的任務和問題。 下列其中一個陳述式必須為true：

   * 任務及其父項可能具有前置任務或任務限制，使其無法處理。
   * 任務或問題的[!UICONTROL 規劃開始日期]在未來的兩週以上。


1. 按一下「[!UICONTROL 任務]」或「[!UICONTROL 問題]」下的「**[!UICONTROL 處理]**」以顯示您目前正在處理的任務和問題。
1. 按一下「[!UICONTROL 問題]」下的「**[!UICONTROL 已要求]**」以顯示您已經要求（指派給您）但尚未接受處理的問題。

## 存取團隊請求

您可以直接從[!UICONTROL 首頁]區域存取指派給您團隊的要求。 如需有關團隊請求的詳細資訊，請參閱[團隊請求概觀](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md)。

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 在&#x200B;**[!UICONTROL 工作清單]**&#x200B;區域中，按一下以展開&#x200B;**[!UICONTROL 團隊請求]**&#x200B;群組。

   如果沒有指派給團隊的請求，則不會顯示分組。

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. 按一下專案團隊名稱。\
   **[!UICONTROL 團隊請求]**&#x200B;區段會顯示並顯示指派給您團隊的所有請求。 如需有關處理團隊要求的詳細資訊，請參閱[管理工作和團隊要求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)。

## 重新指派請求

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 在&#x200B;**[!UICONTROL 工作清單]**&#x200B;區域中，選取您要重新指派的要求。

1. 按一下&#x200B;**[!UICONTROL 指派]** Widget並將您自己從要求中移除，然後輸入您要重新指派要求的使用者名稱。

   >[!TIP]
   >
   >如果工作要求仍處於[準備開始]或[未就緒]狀態，您可以使用[!UICONTROL 工作清單]的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表中的&#x200B;**[!UICONTROL 重新指派]**&#x200B;按鈕。\
   >![重新指派按鈕](assets/reassign-in-left-panel-350x204.png)

1. 如果任務的狀態在完成後變更為[!UICONTROL 新增]或[!UICONTROL 進行中]，您必須取消指派使用者、儲存任務，然後重新指派使用者，任務才能重新出現在他們的首頁工作清單中。

## 回覆要求

您可以回覆要求以進一步釐清要求或建議新日期。

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 在&#x200B;**[!UICONTROL 工作清單]**&#x200B;區域中，選取您要回覆的要求。
1. 找出將請求指派給您的個人。

   您可以在任務的[!UICONTROL 更新]標籤上找到此資訊。 確定已啟用&#x200B;**[!UICONTROL 顯示系統更新]**&#x200B;的選項。

1. 按一下&#x200B;**[!UICONTROL 開始新的更新]**&#x200B;並開始輸入您的回覆。
1. 在&#x200B;**[!UICONTROL 通知]**&#x200B;方塊中輸入收件者名稱，然後按一下&#x200B;**[!UICONTROL 更新]**。

   >[!TIP]
   >
   >如果工作要求仍處於[準備開始]或[!UICONTROL 未就緒]狀態，您可以使用[!UICONTROL 工作清單]的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表中的&#x200B;**[!UICONTROL 回覆]**&#x200B;按鈕。\
   >![[!UICONTROL 回覆按鈕]](assets/reassign-in-left-panel-350x204.png)   >

## 處理請求

當您按一下[!UICONTROL 處理它]按鈕時，您將向提交請求的使用者以及可能指派給請求的任何其他使用者指示您將開始處理請求。 如需有關處理請求的詳細資訊，請參閱[管理工作和團隊請求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)。

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 在&#x200B;**[!UICONTROL 工作清單]**&#x200B;區域中，選取您要處理的請求，然後按一下&#x200B;**[!UICONTROL 處理它]**。\
   問題的相關資訊會顯示在右側面板中。

## 移除請求

如果您決定不應該處理請求，您可以將任務或問題轉換回請求，或從清單中移除它。

1. 按一下右上角的&#x200B;**[!UICONTROL 主要功能表]** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 在&#x200B;**[!UICONTROL 工作清單]**&#x200B;中，指向等待處理的專案。
1. 按一下&#x200B;**[!UICONTROL 指派]** Widget並移除您自己。 這會從您的工作清單移除工作專案。 如果請求未指派給其他人或其他團隊或工作角色，請求將保持未指派狀態。

   或

   按一下[!UICONTROL 首頁工作]清單中任務或問題名稱右側的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表圖示![](assets/more-icon.png)。

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. 從下列選項中選取：

   * **[!UICONTROL 轉換至工作要求]：**&#x200B;選取此選項可將工作專案轉換回工作要求。\

     工作專案會轉換回請求，而您仍會獲指派給請求。\
      您稍後可以再按一下[處理請求] ****&#x200B;來接受請求。

   * **[!UICONTROL 移除]：**&#x200B;選取此選項以從您的[!UICONTROL 工作清單]移除請求。\

     您已從請求中取消指派，且請求不再與您在[!DNL Adobe Workfront]中的名稱相關聯。\
      如果請求未指派給其他人或其他團隊或工作角色，請求將保持未指派狀態。
