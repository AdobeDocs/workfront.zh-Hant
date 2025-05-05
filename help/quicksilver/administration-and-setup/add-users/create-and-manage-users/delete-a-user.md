---
title: 刪除使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 當使用者離開您的組織時，可以將該使用者從Workfront中移除，不過我們建議您停用使用者，而非刪除使用者。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 1%

---

# 刪除使用者

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未加入「Adobe商業平台」的組織。 如果您已上線Adobe Business Platform，則必須刪除Adobe Admin Console中的使用者。
>
>如需根據貴組織是否已加入Adobe Business Platform而有所差異的程式清單，請參閱[以平台為基礎的管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

當使用者離開您的組織時，您可以從Adobe Workfront中移除該使用者。

>[!IMPORTANT]
>
>從系統中刪除使用者也會刪除與您可能想要保留的使用者相關的資訊。 建議您停用使用者，而非刪除使用者。 如需詳細資訊，請參閱[停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td><p>新增：標準</p><p>或</p><p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 </li> 
     <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">下啟用的兩個<b>使用者管理員</b>選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用<b>使用者管理員（群組使用者）</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除和停用使用者

停用使用者會導致發生下列情況：

* 如果Workfront元件與您的Workfront Proof帳戶相關聯，請移除使用者對Workfront Proof和Workfront的授權。 如需Workfront Proof的詳細資訊，請參閱[Workfront Proof：文章索引](../../../workfront-proof/workfront-proof.md)。
* 無法再將工作指派給使用者。
* 無法再將使用者新增到更新中。
* 無法再將使用者新增到團隊或群組。
* 物件無法再與使用者共用。
* 它們與下列物件的關聯會維持不變：

   * 任務、問題、專案、投資組合
   * 儀表板

     >[!NOTE]
     >
     >如果您停用使用者且無法再檢視與使用者相關聯的報告或儀表板，則可能需要更新&#x200B;**使用**&#x200B;欄位的存取許可權執行此報告。\
     >若要深入瞭解，請參閱[&#128279;](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why)為何無法存取停用使用者所擁有的報告？[報告常見問題集](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)文章的區段。

   * 文件
   * 更新
   * 時數

* 如果使用者已將檔案出庫，當您停用檔案時，檔案仍會保持出庫狀態。 只有Workfront管理員可以重新簽入。 如需簽出檔案的詳細資訊，請參閱[簽出檔案](../../../documents/managing-documents/check-out-documents.md)。

刪除使用者會導致發生下列情況：

* 如果Workfront元件與您的Workfront Proof帳戶相關聯，請移除使用者對Workfront Proof和Workfront的授權。 如需Workfront Proof的詳細資訊，請參閱[Workfront Proof：文章索引](../../../workfront-proof/workfront-proof.md)。
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
     >若要深入瞭解，請參閱[&#128279;](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how)如何存取包含已刪除使用者所擁有之報告的儀表板？[報告常見問題集](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)文章的區段。

   * 更新
   * 時數

     >[!NOTE]
     >
     >這些物件仍保留在Workfront中，但物件的擁有者現在為空白。

* 如果使用者在「全域導覽列」的「檔案」區域下上傳了任何檔案，也會刪除檔案。
* 如果使用者已出庫他們擁有的檔案，且檔案已上傳到主檔案區域（從主功能表存取），則會隨使用者刪除檔案。 如需簽出檔案的詳細資訊，請參閱[簽出檔案](../../../documents/managing-documents/check-out-documents.md)。

如需停用使用者的詳細資訊，請參閱[停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。

您可以一次永久刪除一個使用者，也可以同時永久刪除多個使用者。 當您刪除個別使用者時，必須先等候刪除程式完成，才能繼續前往Workfront中的其他活動。 同時刪除多個使用者的程式會作為背景程式執行，因此您可以在刪除使用者時繼續使用Workfront。

## 刪除一或多個使用者

{{step-1-to-users}}

1. 請至少選取一個要刪除的使用者，按一下[更多]功能表![[更多]圖示](assets/more-icon.png)，然後按一下[刪除]&#x200B;**&#x200B;**。
1. 在出現的方塊中，按一下&#x200B;**刪除**&#x200B;以確認刪除。

   刪除使用者的程式會以背景程式執行，因此您可以在刪除使用者時繼續使用Workfront。

   視您要刪除的使用者數量而定，此程式可能需要幾分鐘甚至幾小時的時間。

   在Workfront中收到使用者已刪除的確認後，您可繼續在系統中看見他們，直到在背景完成刪除程式為止。

   稍後，如果您發現一或多個使用者未成功刪除，請嘗試一次刪除一個。
