---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: 在「首頁」區域管理工作和團隊請求
description: 將工作任務和問題分配給您後，將列在 [!UICONTROL 工作清單] 在 [!UICONTROL 首頁] 的上界。 您可以查看、重新分配、回復、處理或刪除請求。 在 [!UICONTROL 首頁] 區域不限於與請求隊列相關的問題。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# 在 [!UICONTROL 首頁] 區域

將工作任務和問題分配給您後，將列在 [!UICONTROL 工作清單] 在 [!UICONTROL 首頁] 的上界。 您可以查看、重新分配、回復、處理或刪除請求。 在 [!UICONTROL 首頁] 區域不限於與請求隊列相關的問題。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>[!UICONTROL工作]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL編輯]對任務和問題的訪問</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>將權限或更高版本貢獻給您需要處理的任務和問題</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 查看工作請求

指派給您的工作請求會顯示在 [!UICONTROL 首頁]. 您可以設定要在中顯示的請求 [!UICONTROL 首頁] 使用 [!UICONTROL 工作清單].

您可以選取篩選條件，以顯示可供您使用的項目或您目前正在使用的項目。

本文說明如何在 [!UICONTROL 首頁] 區域來檢視您目前正在處理或可能考慮開始處理的項目。 如需 [!UICONTROL 首頁] 區域，請參閱 [在 [!UICONTROL 首頁] 區域](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 按一下 **[!UICONTROL 篩選]** 下拉式功能表。

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. 按一下以下任務選項之一或兩者：

   **[!UICONTROL 準備開始]:** 僅顯示已準備好開始的任務和問題。 以下兩個陳述必須為true:

   * 這些任務及其父代沒有前任，也沒有任務限制，無法使其工作。
   * 此 [!UICONTROL 計劃開始日期] 過去或將來最多兩週。

   **[!UICONTROL 未就緒]**:僅顯示尚未準備好開始的任務和問題。 以下任一陳述必須為true:

   * 這些任務及其父代可能有前置任務或任務限制，這些限制會阻止他們工作。
   * 任務或問題具有 [!UICONTROL 計劃開始日期] 未來超過兩週。



1. 按一下 **[!UICONTROL 工作]** 在 [!UICONTROL 工作] 或 [!UICONTROL 問題] 以顯示您目前正在處理的任務和問題。
1. 按一下 **[!UICONTROL 已請求]** 在 [!UICONTROL 問題] 顯示已請求（您已分配給這些問題）但您尚未接受處理的問題。

## 存取團隊請求

您可以直接從 [!UICONTROL 首頁] 的上界。 如需團隊請求的詳細資訊，請參閱 [團隊請求概觀](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 在 **[!UICONTROL 工作清單]** 區域，按一下以展開 **[!UICONTROL 團隊請求]** 分組。

   如果沒有指派任何請求給您的團隊，則不會顯示分組。

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. 按一下團隊名稱。\
   此 **[!UICONTROL 團隊請求]** 區段會顯示並顯示指派給您團隊的所有請求。 如需使用團隊請求的詳細資訊，請參閱 [管理工作和團隊請求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## 重新分配請求

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 在 **[!UICONTROL 工作清單]** 區域，選擇要重新分配的請求。

1. 按一下 **[!UICONTROL 分配]** 介面工具集，然後將您自己從請求中移除，然後輸入您要將請求重新指派給的使用者名稱。

   >[!TIP]
   >
   >如果工作請求仍處於「準備開始」或「未準備就緒」狀態，則可以使用 **[!UICONTROL 重新分配]** 按鈕 **[!UICONTROL 更多]** 功能表 [!UICONTROL 工作清單].\
   >![「重新分配」按鈕](assets/reassign-in-left-panel-350x204.png)

1. 如果任務的狀態更改為 [!UICONTROL 新增] 或 [!UICONTROL 進行中] 完成後，必須取消分配用戶，保存任務，然後重新分配用戶，以便該任務在其「主工作清單」中重新出現。

## 回覆請求

您可以回覆要求，以進一步釐清要求或提出新日期。

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 在 **[!UICONTROL 工作清單]** 區域，選擇要回復的請求。
1. 找出指派請求給您的個人。

   您可以在 [!UICONTROL 更新] 頁簽。 請確定 **[!UICONTROL 顯示系統更新]** 啟用。

1. 按一下 **[!UICONTROL 開始新更新]** 然後開始輸入你的回復。
1. 在 **[!UICONTROL 通知]** 框，然後按一下 **[!UICONTROL 更新]**.

   >[!TIP]
   >
   >如果工作請求仍在「準備開始」或 [!UICONTROL 未就緒] 狀態，您可以使用 **[!UICONTROL 回覆]** 按鈕 **[!UICONTROL 更多]** 功能表 [!UICONTROL 工作清單].\
   >![[!UICONTROL 回覆按鈕]](assets/reassign-in-left-panel-350x204.png)   >

## 處理請求

當您按一下 [!UICONTROL 努力] 按鈕，您可以向提交請求的使用者以及指派給您要開始處理請求之請求的任何其他使用者指出。 如需處理請求的詳細資訊，請參閱  [管理工作和團隊請求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 在 **[!UICONTROL 工作清單]** ，選擇要處理的請求，然後按一下 **[!UICONTROL 努力]**.\
   問題的相關資訊會顯示在右側面板中。

## 移除請求

如果您決定不應使用請求，您可以將任務轉換或問題還原為請求，或從清單中移除它。

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 在 **[!UICONTROL 工作清單]**，指向等待處理的項目。
1. 按一下 **[!UICONTROL 分配]** 小工具，把你自己移除。 這會從您的工作清單中刪除工作項。 如果未將請求指派給其他任何人，或指派給其他團隊或工作角色，請求將保留為未指派。

   或

   按一下 **[!UICONTROL 更多]** 功能表圖示 ![](assets/more-icon.png) 中任務或問題名稱的權利 [!UICONTROL 家政] 清單。

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. 從下列選項中選取：

   * **[!UICONTROL 轉換為工作請求]:** 選擇此選項可將工作項轉換為工作請求。\

      工作項目會轉換回請求，而您仍會被指派給請求。\
      您稍後可以按一下「 」，以接受請求 **[!UICONTROL 努力]** 。

   * **[!UICONTROL 移除]:** 選取此選項，即可從 [!UICONTROL 工作清單].\

      系統從請求中取消指派您，且請求不再與您的名稱關聯於 [!DNL Adobe Workfront].\
      如果未將請求指派給其他任何人，或指派給其他團隊或工作角色，請求將保留為未指派。
