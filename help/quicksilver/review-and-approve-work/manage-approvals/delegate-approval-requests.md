---
product-area: projects
navigation-topic: approvals
title: 委派核准請求
description: 委派核准請求可讓您指派另一個使用者來核准您的請求一段時間，例如，假期您將不在辦公室時。
author: Courtney
feature: Work Management
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: d04afc0cc55a71e48c357af2ed4446c22dab1ba4
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 0%

---

# 委派核准請求

您可以在外出時暫時委派指派給的工作。 您可以委派任務和發放分配，也可以委派批准請求。 本文說明如何委派核准請求。 有關委派任務和問題分配的資訊，請參見 [管理任務和問題委派](../../manage-work/delegate-work/how-to-delegate-work.md).

>[!NOTE]
>
>為確保您為委派核准所排程的日期不會不一致，我們建議您的使用者設定檔的時區符合您排程的時區。 如需詳細資訊，請參閱下列文章：
>
>* [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>


## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請聯絡您的Workfront管理員。

## 了解委派核准的使用者存取權

在指定的核准期間，您委派核准請求的使用者具備下列功能：

* 可以在未作出任何決定時批准或拒絕現有批准請求
* 可以批准和拒絕在指定時段內接收的新批准請求
* 已授予對等待批准的對象的查看訪問權限

   >[!NOTE]
   >
   > Adobe Workfront管理員可限制使用者存取特定物件類型。 當用戶沒有對對象類型的訪問權限，並且將該類型的批准委託給用戶時，用戶沒有對該對象的「查看」訪問權限。 不過，使用者仍可以核准或拒絕 **首頁** 頁面，如 [核准工作](../../review-and-approve-work/manage-approvals/approving-work.md).\
   例如，使用者A屬於群組A。Workfront管理員已限制群組A的存取權限，因此此群組中的使用者無法檢視Workfront中的工作。 如果將任務批准請求委派給用戶A，則用戶A無法查看與批准關聯的任務。 但是，用戶A可以從首頁批准或拒絕批准請求。

   有關Workfront管理員如何限制對安裝程式中對象類型的訪問權限的資訊，請參見  [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

在批准委派停止或取消後，指定為批准者的用戶：

* 無法再為需要核准的項目核准工作
* 繼續具有工作項的「查看」訪問權\
   通過批准委派獲得對對象的查看訪問權限的用戶，即使在批准委派停止或被撤回後，仍保留該查看訪問權限。 要刪除在委派批准期間用戶有權訪問的任何對象的查看訪問權限，您必須轉到該對象並直接從該對象中刪除訪問權限。

## 在「首頁」區域中委派核准請求

* [將您的核准委派給其他使用者](#delegate-your-approvals-to-another-user)
* [更新或停止核准委派](#update-or-stop-an-approval-delegation)
* [查看委派的批准](#view-delegated-approvals)

### 將您的核准委派給其他使用者 {#delegate-your-approvals-to-another-user}

無論如何將核准指派給您（無論是直接指派給您、指派給您所屬的團隊，還是指派給您的工作角色），您都可以委派下列核准類型：

* 專案核准
* 任務批准
* 核准

不能委派工時單和文檔批准。 

委派核準時，請考量下列事項：

* 委派核準時，會委派所有核准。 您無法委派個別的核准請求。
* 您只能將核准委派給一個使用者；您無法同時將核准委派給多個使用者。\
   所有項目、任務和問題的所有批准都委託給您指定的用戶。
* 最多5個使用者可以同時委派核准給同一位使用者。 換言之，不能將單一使用者同時指定為超過5個使用者的暫時核准者。
* 「更新」索引標籤上會顯示有關核准的活動。 必須啟用「顯示系統更新」。 委派核准的使用者和委派核准的使用者，都會收到關於核准活動的電子郵件通知。

要將批准委託給其他用戶，請執行以下操作：

1. 按一下 **首頁** 圖示 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   您的Workfront管理員可能會對環境中的「首頁」圖示進行下列變更：
   * 以自訂的影像取代，以說明您的組織。 在此情況下，圖示看起來會與本文所顯示的不同。
   * 將連結至該頁面的頁面取代為其他頁面。 在此情況下，按一下 **主菜單** ![](assets/main-menu-icon.png) 在頁面的右上角，然後按一下 **首頁**.


   或

   按一下 **主菜單** 圖示> **您的姓名** > **關閉時間** 中。

1. （選用和條件性）在「首頁」區域中，按一下 **篩選** 下拉式功能表，然後按一下 **核准**.

1. （有條件）按一下 **委派我的核准**

   或

   如果您的系統或組管理員啟用了任務和問題委派，請按一下 **委派**，然後按一下 **委派核准**.

   ![](assets/delegate-approvals-nwe.png)

1. 在「委派我的核准」區段中指定下列資訊：

   * **名稱**:開始輸入要委派核准的使用者名稱，然後在下拉式功能表中顯示名稱時按一下名稱。
   * **開始日期**:選擇開始轉發批准的日期。 轉送從您選取的日期凌晨12:00開始。\
      開始日期必須是目前日期或未來日期。
   * **結束日期**：執行下列其中一項操作：

      * 選擇停止轉發的批准日期。 轉送將於您選取的日期晚上11時59分結束。
      * 選擇 **無結束日期** 設定Workfront以無限期委派核准。

1. 按一下&#x200B;**儲存**。

### 更新或停止核准委派 {#update-or-stop-an-approval-delegation}

1. 按一下 **首頁** 圖示 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   您的Workfront管理員可能會對環境中的「首頁」圖示進行下列變更：
   * 以自訂的影像取代，以說明您的組織。 在此情況下，圖示看起來會與本文所顯示的不同。
   * 將連結至該頁面的頁面取代為其他頁面。 在此情況下，按一下 **主菜單** ![](assets/main-menu-icon.png) 在頁面的右上角，然後按一下 **首頁**.


1. 按一下 **篩選** 下拉式功能表，然後按一下 **核准**.

1. （有條件）按一下 **編輯委派**

   或

   如果系統或組管理員啟用了任務和問題委派，請按一下 **編輯委派**，然後按一下 **委派核准**.

1. （條件性）執行下列任一操作：

   * 要更新現有批准委派，請執行以下操作：變更顯示的資訊，然後按一下 **儲存**.

   * 要停止現有委派：按一下 **停止委派**，然後按一下 **停止委派** 確認。

      ![](assets/stop-delegation-nwe.png)

### 查看委派的批准 {#view-delegated-approvals}

您只能在「工作清單」中查看以下類型的批准委託：

* 專案核准
* 任務批准
* 核准

要查看委託批准，請執行以下操作：

1. 按一下 **首頁** 圖示 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   您的Workfront管理員可能會對環境中的「首頁」圖示進行下列變更：
   * 以自訂的影像取代，以說明您的組織。 在此情況下，圖示看起來會與本文所顯示的不同。
   * 將連結至該頁面的頁面取代為其他頁面。 在此情況下，按一下 **主菜單** ![](assets/main-menu-icon.png) 在頁面的右上角，然後按一下 **首頁**.


1. 按一下 **篩選** 下拉式功能表，然後按一下 **核准**.\
   依預設，所有核准都會顯示在清單中，包括指派給您的核准和委派給您的核准。

   ![](assets/delegated-to-me-nwe-350x93.png)
