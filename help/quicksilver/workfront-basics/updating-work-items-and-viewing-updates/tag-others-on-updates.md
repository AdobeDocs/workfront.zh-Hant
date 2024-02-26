---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 標籤其他人的更新
description: 在Adobe Workfront物件上提供更新註解時，專案上的所有使用者都可以看到提交的資訊。 不過，有時候，不在專案中的使用者可以從檢視此資訊中獲益。 您可以在更新中標籤這些使用者，以便與他們共用，而不將他們包含在專案中。 標籤的使用者會收到事件通知。
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 56ab6fe79fe6e10be2ec61cb16ff48b30856dc0f
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 0%

---

# 標籤其他人的更新

{{highlighted-preview}}

<!--take new commenting and legacy commenting out when we remove the legacy commenting and the new one is the only experience-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 
-->

>[!IMPORTANT]
>
>我們目前正在重新設計Adobe Workfront中的評論體驗。
>
>根據您存取註釋體驗的物件，您可能會在「更新」區段中看到下列功能：
>* 新體驗
>* 舊版體驗
>* 全新和舊版體驗
>
>如需有關新評論體驗及其可用性的詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>新註解體驗僅適用於Workfront物件的「更新」區段，當您從以下區域存取物件時，將無法使用：
>
> * 首頁
> * 清單中的摘要面板
> * 時程表中的摘要面板
> * 工作負載平衡器中的摘要面板
>
><span class="preview">新的評論體驗可在「預覽」環境的清單、時程表和工作負載平衡器的摘要面板中取得。</span>

如果您想要吸引使用者注意某個物件，而他們可能不會關注該物件，則可以在更新物件時標籤使用者。

您不可以透過將使用者指派給物件或讓使用者訂閱物件來將他們包含在物件上，而是在更新時標籤他們，以便與他們共用。 標籤的使用者會收到您輸入之更新的相關通知。

## 在更新中標籤使用者的相關考量事項

* 在更新中被標籤的使用者必須在他們的設定檔中啟用個人通知，以便他們接收電子郵件通知。 如需詳細資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  如需有關將更新新增至Workfront物件的資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* 當問題轉換為專案或任務時，更新會複製到新專案或任務，但標籤的使用者不會。 若要繼續交談，您必須再次標籤參與者。

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
   <td> <p>要求或更高的問題和檔案；檢閱或更高的所有其他物件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>問題和檔案的要求者或以上；所有其他物件的檢閱者或以上</p> 
   <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>檢視物件的存取權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 標籤其他人的更新

在更新中為其他人加上標籤會因您選擇的體驗和物件而異。

### 在新評論體驗中標籤其他人的更新

您可以透過下列方式，在新註解體驗中標籤其他人的更新：

* **自動**：當使用者啟動對話串、新增評論或新增回覆時，會自動標籤他們並新增到標籤人員或團隊區域的評論方塊。 <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

  >[!TIP]
  >
  >當對話串在舊版評論體驗中開始時，不會自動標籤對話串參與者。

* **手動**：手動將使用者新增至評論方塊的「標籤人員」區域時。

您也可以在編輯或回複評論時，移除被錯誤標籤的使用者。

1. 開始更新工作專案，如所述 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 您身為註解擁有者，會自動被標籤並新增至註解方塊的「標籤人員」或「團隊」區域。

   >[!TIP]
   >
   >評論擁有者在評論方塊的「標籤人員」或「團隊」區域中看不到自己的名稱。

1. 在 **標籤人員或團隊** 欄位，開始輸入您要包含的使用者或團隊名稱，然後在名稱出現在下拉式清單中時按一下該名稱。

   或

   在「 」中輸入@符號 **撰寫評論** 區域，開始輸入您要在更新中包含的使用者或團隊名稱，然後按一下該名稱（當它出現在下拉式清單中時）。

   >[!TIP]
   > 
   >當存在具有類似或相同名稱的使用者時，若要識別正確的使用者，請注意顯示圖片、使用者的主要角色或其電子郵件地址。
   > 
   >使用者必須至少與一個工作角色相關聯，才能在更新中標籤他們時檢視該工作角色。
   > 
   >您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱 [授予使用者存取許可權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   <div class="preview">

   預覽環境中的標籤範例：
   ![標籤使用者](assets/tag-others-unified-commenting-with-all-tab.png)

   </div>

   生產環境中的標籤範例：
   ![](assets/tag-others-unified-commenting.png)

1. （選用）若要設為私人更新，請啟用 **我的公司私有** 位於更新方塊的右下角。 這可讓貴公司的使用者看到更新。 此 **我的公司私有** 只有在Workfront設定檔中指定了公司時，才可使用選項。

   >[!NOTE]
   >
   >* 只有在使用者與公司相關聯時，才會顯示此選項。
   >* 公司外部的已標籤使用者仍可收到應用程式內通知或電子郵件，即使他們不會在更新索引標籤上看到私人評論。 如果您不想與外部使用者共用資訊，建議不要在更新時標籤這些使用者。

1. （可選）若要新增多個使用者和團隊，請重複步驟2。 <!--insure this stays accurate-->

   >[!NOTE]
   >
   >「標籤人員或團隊」欄位中列出的所有使用者和團隊成員都會收到更新的應用程式內通知，且可能會收到電子郵件，具體取決於其電子郵件通知設定的設定。 在評論或回覆中標籤自己的使用者會收到該評論或回覆的通知，並可以在中看到他們的名稱被列為對話串剩餘部分的成員，但他們不會收到另一個通知，除非他們再次標籤自己。 如需詳細資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [為系統中的每個人設定事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 按一下 **提交**.\
   更新中包含的使用者會自動被授予物件的檢視許可權，而且可以檢視和回應對物件所做的更新。

   標籤實體的名稱會顯示在其頭像旁，最多兩個實體。 如果標籤了兩個以上的實體，除了會標籤多少個其他實體外，還會顯示第一個實體的名稱。

   ![](assets/members-icons-expanded-unshimmed.png)

   有關更新工作專案時可用的其他功能的資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. （可選）按一下 **更多** 功能表 ![](assets/more-menu.png) 在註解的右上角，然後按一下 **編輯**. 移除任何已標籤的使用者，然後按一下 **提交**. 您只能在輸入註解後15分鐘內進行編輯。 您只能編輯您新增的註解。

   >[!TIP]
   >
   >使用舊版評論體驗新增評論和回覆時，未特別標籤的評論擁有者無法由使用新評論體驗的人員手動移除。


### 在舊版更新區段中標籤其他人的更新

您可以在舊版更新區段中手動標籤使用者。

1. 開始更新工作專案，如所述 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 在 **通知** 欄位，開始輸入您要包含的使用者或團隊名稱，然後在名稱出現在下拉式清單中時按一下該名稱。

   或

   在「 」中輸入@符號 **開始新的更新** 區域，開始輸入您要在更新中包含的使用者或團隊名稱，然後按一下該名稱（當它出現在下拉式清單中時）。

   >[!TIP]
   >
   >當存在具有類似或相同名稱的使用者時，若要識別正確的使用者，請注意顯示圖片、使用者的主要角色或其電子郵件地址。
   >
   >使用者必須至少與一個工作角色相關聯，才能在更新中標籤他們時檢視該工作角色。
   >
   >您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱 [授予使用者存取許可權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. （選用）若要設為私人更新，請啟用 **我的公司私有** 位於更新方塊的右下角。 這可讓貴公司的使用者看到更新。 此 **我的公司私有** 只有在Workfront設定檔中指定了公司時，才可使用選項。

   >[!NOTE]
   >
   >公司外部的已標籤使用者仍可收到應用程式內通知或電子郵件，即使他們不會在更新索引標籤上看到私人評論。 如果您不想與外部使用者共用資訊，建議不要在更新時標籤這些使用者。

1. （可選）若要新增多個使用者和團隊，請重複步驟2。

   >[!NOTE]
   >
   >列在「通知」欄位中的所有使用者和團隊成員都會收到更新的應用程式內通知，且可能會收到電子郵件，具體取決於其電子郵件通知設定的設定。 在評論或回覆中標籤自己的使用者會收到該評論或回覆的通知，並可在其餘對話的「通知」欄位中看到其名稱，但除非他們再次標籤自己，否則不會收到其他通知。 如需詳細資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [為系統中的每個人設定事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 按一下 **更新**.\
   更新中包含的使用者會自動被授予物件的檢視許可權，而且可以檢視和回應對物件所做的更新。

   您可以在更新對話串頂端檢視每個回覆中已標籤的訪客。 這些使用者以及訂閱物件的任何使用者會在物件進行更新或回覆時收到通知。

   ![](assets/tagging-transparency-350x192.png)

   有關更新工作專案時可用的其他功能的資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



