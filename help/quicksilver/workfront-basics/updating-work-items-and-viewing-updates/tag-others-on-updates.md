---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 標籤其他更新的專案
description: 在Adobe Workfront物件上提供更新註解時，專案上的所有使用者都可以看到提交的資訊。 不過，有時候，不在專案中的使用者可以從檢視此資訊中獲益。 您可以在更新中標籤這些使用者，以便與他們共用，而不需將這些使用者包含在專案中。 標籤的使用者會收到事件通知。
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: e1411ce49d8668ba50bcb9b80d4a4b47d0dd00fc
workflow-type: tm+mt
source-wordcount: '1436'
ht-degree: 0%

---

# 標籤其他更新的專案

<!--take "Beta" references out when we remove the beta-->


<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在「預覽」環境中可用。

>[!NOTE]
>
>我們目前正在重新設計Adobe Workfront中的評論體驗。
>
>如需有關新評論體驗的詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>您可以存取下列物件的新體驗：
> * 問題， <span class="preview">專案</span>， <span class="preview">任務</span>、和 <span class="preview">檔案</span>，即可開始評論Beta版。
   >
   >     此功能僅適用於「更新」區段，不適用於以下區域：
   >
   >     * 首頁
   >     * 清單中的摘要面板
   >     * 時程表中的摘要面板
>
> * 目標

   >
   >   新的註解體驗是目標的預設值。 您必須有其他授權才能存取Workfront目標。 如需詳細資訊，請參閱 [使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    如需有關對目標發表註解的資訊，請參閱 [在Adobe Workfront目標中管理目標註解](../../workfront-goals/goal-management/manage-goal-comments.md).



如果您想要吸引使用者注意他們可能未關注的物件，則可以在更新物件時標籤使用者。
您可以在更新中標籤這些使用者，以便與他們共用，而不需透過將他們指派給或讓他們訂閱來將他們包含在物件上。 標籤的使用者會收到您輸入之更新的相關通知。

>[!NOTE]
>
>使用者必須在他們的設定檔中啟用個人通知，以便他們接收電子郵件通知。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

如需新增更新至Workfront物件的詳細資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>當問題轉換為專案或任務時，更新將會複製到新專案或任務，但標籤的使用者不會。 若要繼續交談，您必須再次標籤參與者。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>請求或更高版本以處理問題和檔案；檢閱或更高版本以處理所有其他物件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>問題和檔案的要求者或以上；所有其他物件的檢閱者或以上</p> 
   <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>檢視物件的存取權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡Workfront管理員。

## 標籤其他更新的專案

在更新中為其他人加上標籤會因您選擇的體驗和物件而異。

### 在目前的更新區段中標籤其他人的更新

1. 開始更新工作專案，如所述 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 在 **通知** 欄位，開始輸入您要包含的使用者或團隊名稱，然後按一下該名稱（當它出現在下拉式清單中時）。

   或

   在「 」中輸入@符號 **開始新的更新** 區域，開始輸入您要在更新中包含的使用者或團隊名稱，然後在其出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   >
   >當存在具有類似或相同名稱的使用者時，若要識別正確的使用者，請注意頭像、使用者的主要角色或其電子郵件地址。 使用者必須至少與一個工作角色相關聯，才能在更新中標籤他們時檢視該工作角色。

   ![](assets/tag-users-in-update.png)

1. （選用）若要將更新設為私人，請啟用 **我的公司私有** 更新方塊的右下角。 這會使更新僅對您公司中的使用者可見。 此 **我的公司私有** 選項僅適用於在Workfront設定檔中指定了公司的情況。

   >[!NOTE]
   >
   >公司外部的標籤使用者仍可收到應用程式內通知或電子郵件，即使他們看不到更新索引標籤上的私人評論。 如果您不想與外部使用者共用資訊，建議不要在更新時標籤外部使用者。

1. （可選）若要新增多個使用者和團隊，請重複步驟2。

   >[!NOTE]
   >
   >「通知」欄位中列出的所有使用者和團隊成員都會收到更新的應用程式內通知，且可能會收到電子郵件，具體取決於其電子郵件通知設定的設定。 在評論或回覆中標籤自己的使用者會收到該評論或回覆的通知，並可在其餘對話的「通知」欄位中看到其名稱，但除非他們再次標籤自己，否則不會收到其他通知。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [為系統中的每個人設定事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 按一下 **更新**.\
   更新中包含的使用者會自動被授予物件的檢視許可權，並可以檢視和回應物件的更新。

   您可以在更新對話串頂端檢視每個回覆中已標籤的使用者。 這些使用者以及訂閱物件的任何使用者會在物件更新或回覆時收到通知。

   ![](assets/tagging-transparency-350x192.png)

   有關更新工作專案時可用的其他功能的資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### 標籤其他人在評論Beta版體驗中的更新

您可以在評論Beta版體驗中標籤其他人的更新。 您也可以在編輯評論時，移除被錯誤標籤的使用者。

1. 開始更新工作專案，如所述 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 在 **標籤人員或團隊** 欄位，開始輸入您要包含的使用者或團隊名稱，然後按一下該名稱（當它出現在下拉式清單中時）。

   或

   在「 」中輸入@符號 **撰寫評論** 區域，開始輸入您要在更新中包含的使用者或團隊名稱，然後在其出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   >
   >當存在具有類似或相同名稱的使用者時，若要識別正確的使用者，請注意頭像、使用者的主要角色或其電子郵件地址。 使用者必須至少與一個工作角色相關聯，才能在更新中標籤他們時檢視該工作角色。

   ![](assets/tag-others-unified-commenting.png)

1. （選用）若要將更新設為私人，請啟用 **我的公司私有** 更新方塊的右下角。 這會使更新僅對您公司中的使用者可見。 此 **我的公司私有** 選項僅適用於在Workfront設定檔中指定了公司的情況。

   >[!NOTE]
   >
   >* 此選項僅在使用者與公司相關聯時顯示。
   >* 公司外部的標籤使用者仍可收到應用程式內通知或電子郵件，即使他們看不到更新索引標籤上的私人評論。 如果您不想與外部使用者共用資訊，建議不要在更新時標籤外部使用者。


1. （可選）若要新增多個使用者和團隊，請重複步驟2。 <!--insure this stays accurate-->

   >[!NOTE]
   >
   >「標籤人員或團隊」欄位中列出的所有使用者和團隊成員都會收到更新的應用程式內通知，且可能會收到電子郵件，具體取決於其電子郵件通知設定的設定。 在評論或回覆中標籤自己的使用者會收到該評論或回覆的通知，並且可以在中看到其名稱被列為對話串剩餘部分的成員，但他們不會收到另一個通知，除非他們再次標籤自己。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [為系統中的每個人設定事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 按一下 **提交**.\
   更新中包含的使用者會自動被授予物件的檢視許可權，並可以檢視和回應物件的更新。

   您可以在「成員」區域的更新文字下檢視每個回覆中已標籤的人員。 這些使用者以及訂閱物件的任何使用者會在物件更新或回覆時收到通知。
1. （可選）按一下 **成員** 包含在更新中，以顯示您輸入的更新與其共用的實體清單。

   ![](assets/members-icons-expanded-unshimmed.png)

   有關更新工作專案時可用的其他功能的資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. （可選）按一下 **更多** 功能表 ![](assets/more-menu.png) 按一下「讚」圖示右側，然後按一下 **編輯**. 移除任何已標籤的使用者，然後按一下 **提交**. 您只能在輸入註解後15分鐘內對其進行編輯。 您只能編輯您新增的註解。