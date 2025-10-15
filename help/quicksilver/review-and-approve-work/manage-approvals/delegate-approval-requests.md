---
product-area: projects
navigation-topic: approvals
title: 委派核准請求
description: 委派核准請求可讓您指派另一名使用者，在一段時間核心准您的請求，例如，當您休假時。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: 14360a82b0de65587a9413b58d9c69abb55fa29d
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 0%

---

# 委派核准請求

您不在辦公室時，可以暫時委派指派給您的工作。 您可以委派任務和問題指派，也可以委派核准請求。 本文會說明如何委派核准請求。 有關委派任務和問題指派的資訊，請參閱[委派任務和問題](../../manage-work/delegate-work/how-to-delegate-work.md)。

無論核准如何指派給您（無論是直接指派給您、您所屬的團隊或您的工作角色），您都可以委派下列型別的核准：

* 專案核准
* 任務核准
* 問題核准

您無法委派時程表、檔案或校訂核准。

>[!NOTE]
>
>為確保與您排程委派核准的日期不會有任何不一致，我們建議您的使用者設定檔的時區與排程的時區相符。 如需詳細資訊，請參閱下列文章：
>
>* [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td>
   <p>Contribute或更高版本</p>
   <p>評論或以上</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 瞭解受委派核准的使用者存取權

在指定的核准期間，您委派核准請求的使用者具有下列能力：

* 可以核准或拒絕未做出決定的現有核准請求
* 可以核准和拒絕在指定時段內收到的新核准要求
* 被授與等待核准之物件的檢視存取權

  >[!NOTE]
  >
  > Adobe Workfront管理員可以限制使用者存取某些物件型別。 當使用者無權存取物件型別並且該型別的核准委派給使用者時，使用者無權檢視物件。 但是，使用者仍然可以核准或拒絕來自&#x200B;**首頁**&#x200B;頁面的核准要求，如[核准工作](../../review-and-approve-work/manage-approvals/approving-work.md)中所述。\
  >例如，使用者A屬於群組A。Workfront管理員已限制群組A的存取權，因此該群組中的使用者無法在Workfront中檢視任務。 如果任務核准請求被委派給使用者A，則使用者A無法檢視與核准相關聯的任務。 但是，使用者A可以從首頁核准或拒絕核准請求。

  如需Workfront管理員如何在「設定」中限制物件型別存取權的相關資訊，請參閱  [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。 

核准委派停止或取消後，指定為核准者的使用者：

* 不再具有核准需要核准之專案工作的存取權
* 繼續擁有工作專案的檢視存取權\
  透過核准委派而被授予物件檢視存取許可權的使用者，即使在核准委派停止或被撤回後，仍保留該檢視存取許可權。 若要移除核准委派期間使用者有權存取之任何物件的「檢視」存取權，您必須移至物件，並直接從物件移除存取權。

## 將您的核准委派給其他使用者 {#delegate-your-approvals-to-another-user}

無論核准如何指派給您（無論是直接指派給您、您所屬的團隊或您的工作角色），您都可以委派下列型別的核准：

* 專案核准
* 任務核准
* 問題核准

您無法委派時程表、檔案或校訂核准。

委派核準時，請考量下列事項：

* 當您委派核準時，您的所有核准都會被委派。 您無法委派個別核准請求。
* 您只能將核准委派給一個使用者；您不能同時將核准委派給多個使用者。\
  所有專案、任務和問題的所有核准都會委派給您指定的使用者。
* 最多5名使用者可同時委派核准給相同使用者。 換言之，一個使用者無法同時被指定為5個以上使用者的暫時核准者。
* 有關核准的活動會顯示在更新索引標籤上。 您必須啟用[顯示系統更新]。 委派核准的使用者和受委派核准的使用者都會收到有關核准活動的電子郵件通知。

### 從首頁區域委派核准


若要將核准委派給其他使用者：

1. 按一下右上角的&#x200B;**[!UICONTROL 主功能表]** ![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）按一下&#x200B;**自訂**&#x200B;以新增&#x200B;**我的核准** Widget。
1. 移至[我的核准]Widget，然後按一下[委派我的核准] **。**

   >[!NOTE]
   >
   >Workfront管理員可以從設定區域停用核准委派。 如果核准委派被停用，您將不會看到「委派核准」按鈕。

   ![在首頁](assets/delegate-approvals-home.png)委派核准

1. 在委派我的核准區段中指定下列資訊：

   * **名稱**：開始輸入您要委派核准的使用者名稱，然後在名稱出現在下拉式功能表中時按一下該名稱。
   * **開始日期**：選取核准開始轉送的日期。 轉送從您選取的日期凌晨12:00開始。\
     開始日期必須是目前日期或是未來日期。
   * **結束日期**：執行下列任一項作業：
      * 選取核准停止轉送的日期。 轉送在您選取的日期晚上11:59結束。
      * 選取&#x200B;**無結束日期**&#x200B;以設定Workfront無限期委派核准。

1. 按一下「**儲存**」。

### 從您的使用者設定檔委派核准

1. 按一下左側面板中的&#x200B;**主要功能表**&#x200B;圖示> **您的名稱** > **休假**。
1. 按一下&#x200B;**委派核准**。

   >[!NOTE]
   >
   >Workfront管理員可以從設定區域停用核准委派。 如果核准委派被停用，您將不會看到「委派核准」按鈕。

1. 在委派我的核准區段中指定下列資訊：

   * **名稱**：開始輸入您要委派核准的使用者名稱，然後在名稱出現在下拉式功能表中時按一下該名稱。
   * **開始日期**：選取核准開始轉送的日期。 轉送從您選取的日期凌晨12:00開始。\
     開始日期必須是目前日期或是未來日期。
   * **結束日期**：執行下列任一項作業：
      * 選取核准停止轉送的日期。 轉送在您選取的日期晚上11:59結束。
      * 選取&#x200B;**無結束日期**&#x200B;以設定Workfront無限期委派核准。

## 更新或停止核准委派 {#update-or-stop-an-approval-delegation}

1. 按一下右上角的&#x200B;**[!UICONTROL 主功能表]** ![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）按一下&#x200B;**自訂**&#x200B;以新增&#x200B;**我的核准** Widget。

1. 前往「我的核准」Widget，然後按一下「**編輯委派**」。
   ![編輯委派](assets/edit-delegations.png)
<!--
   Or

   If your system or group administrator enabled task and issue delegation, click **Edit delegation**, then click **Delegate approvals**.   -->

1. （視條件而定）執行下列任一項作業：

   * 若要更新現有的核准委派：變更顯示的資訊，然後按一下[儲存]。**&#x200B;**

   * 若要停止現有的委派：按一下[停止委派]&#x200B;**&#x200B;**，然後按一下[停止委派]&#x200B;**確認。**

## 檢視受委派的核准 {#view-delegated-approvals}

您只能在「我的核准」Widget中檢視下列型別的核准委派：

* 專案核准
* 任務核准
* 問題核准

若要檢視受委派的核准：

1. 按一下右上角的&#x200B;**[!UICONTROL 主功能表]** ![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）按一下&#x200B;**自訂**&#x200B;以新增&#x200B;**我的核准** Widget。
1. 在&#x200B;**我的核准** Widget中，按一下&#x200B;**篩選器**&#x200B;下拉式功能表，然後按一下&#x200B;**委派核准**。\
   委派給您的所有核准都會顯示在清單中。
