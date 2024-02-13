---
title: 刪除使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 當使用者離開您的組織時，可以將該使用者從Workfront中移除，不過我們建議您停用使用者，而非刪除使用者。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: b3717fc89e45983b80471fdd629c79b82086c6ff
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# 刪除使用者

當使用者離開您的組織時，您可以從Adobe Workfront中移除該使用者。

>[!IMPORTANT]
>
>從系統中刪除使用者也會刪除與您可能想要保留的使用者相關的資訊。 建議您停用使用者，而非刪除使用者。 如需詳細資訊，請參閱 [停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>. </p> </li> 
     <li> <p><b>使用者</b> 將存取層級中的設定設為 <b>編輯</b> 存取，使用 <b>建立</b> 以及兩者中的至少一個 <b>使用者管理員</b> 選項已啟用於 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>這兩個選項中，如果使用者 <b>管理員（群組使用者）</b> 已啟用，您必須是使用者所屬群組的群組管理員。</p> <p>如需關於的詳細資訊 <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 刪除和停用使用者

停用使用者會導致發生下列情況：

* 如果Workfront Proof元件與您的Workfront帳戶相關聯，請移除使用者的Workfront和Workfront Proof授權。 如需Workfront Proof的詳細資訊，請參閱 [Workfront Proof：文章索引](../../../workfront-proof/workfront-proof.md).
* 無法再將工作指派給使用者。
* 無法再將使用者新增到更新中。
* 無法再將使用者新增到團隊或群組。
* 物件無法再與使用者共用。
* 它們與下列物件的關聯會維持不變：

   * 任務、問題、專案、投資組合
   * 儀表板

     >[!NOTE]
     >
     >如果您停用使用者且無法再檢視與使用者相關聯的報告或儀表板，則可能需要更新 **透過以下存取許可權運行此報告：** 欄位。\
     >若要進一步瞭解，請參閱 [為何無法存取已停用使用者所擁有的報表？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) 的區段 [報表常見問題集](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 文章。

   * 文件
   * 更新
   * 時數

* 如果使用者已將檔案出庫，當您停用檔案時，檔案仍會保持出庫狀態。 只有Workfront管理員可以重新簽入。 如需出庫檔案的詳細資訊，請參閱 [簽出檔案](../../../documents/managing-documents/check-out-documents.md).

刪除使用者會導致發生下列情況：

* 如果Workfront校訂元件與您的Workfront帳戶相關聯，請移除使用者的Workfront和Workfront Proof授權。 如需Workfront Proof的詳細資訊，請參閱 [Workfront Proof：文章索引](../../../workfront-proof/workfront-proof.md).
* 無法再將工作指派給使用者。
* 無法再將使用者新增到更新中。
* 無法再將使用者新增到團隊或群組。
* 物件無法再與使用者共用。
* 刪除該使用者與下列物件的關聯：

   * 任務、問題、專案、投資組合
   * 儀表板

     >[!NOTE]
     >
     >您也會失去對包含與已刪除使用者相關聯之控制面板的自訂區段的存取權。\
     >若要進一步瞭解，請參閱 [如何存取包含已刪除使用者所擁有報表的儀表板？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) 的區段 [報表常見問題集](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 文章。

   * 更新
   * 時數

     >[!NOTE]
     >
     >這些物件仍保留在Workfront中，但物件的擁有者現在為空白。

* 如果使用者在「全域導覽列」的「檔案」區域下上傳了任何檔案，也會刪除檔案。
* 如果使用者已出庫他們擁有的檔案，且檔案已上傳到主檔案區域（從主功能表存取），則會隨使用者刪除檔案。 如需出庫檔案的詳細資訊，請參閱 [簽出檔案](../../../documents/managing-documents/check-out-documents.md).

如需停用使用者的詳細資訊，請參閱 [停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

您可以一次永久刪除一個使用者，也可以同時永久刪除多個使用者。 當您刪除個別使用者時，必須先等候刪除程式完成，才能繼續前往Workfront中的其他活動。 同時刪除多個使用者的程式會作為背景程式執行，因此您可以在刪除使用者時繼續使用Workfront。

## 刪除一或多個使用者

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **使用者**.
1. 請至少選取一個要刪除的使用者，然後按一下「更多」功能表 ![](assets/more-icon.png)，然後按一下 **刪除**.
1. 在出現的方塊中，按一下 **刪除** 以確認刪除。

   刪除使用者的程式會以背景程式執行，因此您可以在刪除使用者時繼續使用Workfront。

   視您要刪除的使用者數量而定，此程式可能需要幾分鐘甚至幾小時的時間。

   在Workfront中收到使用者已刪除的確認後，您可繼續在系統中看見他們，直到在背景完成刪除程式為止。

   稍後，如果您發現一或多個使用者未成功刪除，請嘗試一次刪除一個。
