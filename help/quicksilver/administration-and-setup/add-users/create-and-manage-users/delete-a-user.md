---
title: 刪除使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 當使用者離開您的組織時，可以將該使用者從Workfront中移除，不過我們建議您停用使用者，而非刪除使用者。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
TQID: 'https://experienceleague.adobe.com/T5iSq2SOJEQrlvLNiQ5l69OncRMYvEs4uf6QosY9vq8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 6275fff5d615a8db678f16d99c38c96319a57155
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 7%
---
# 刪除使用者

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未上線至Admin Console的組織。 由於您的組織已加入Adobe Admin Console，因此您必須透過Adobe Admin Console執行此動作。
>
>  如需在Adobe Admin Console中刪除使用者的指示，請參閱[個別管理使用者](https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html)一文中的「永久刪除使用者」一節，或連絡您的Adobe Admin Console管理員。

當使用者離開您的組織時，您可以從Adobe Workfront中移除該使用者。

刪除使用者必須透過Adobe Admin Console執行。 如需指示，請參閱文章[個別管理使用者](https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html)中的「永久刪除使用者」一節，或連絡您的Adobe Admin Console管理員。

>[!IMPORTANT]
>
>從系統中刪除使用者也會刪除與您可能想要保留的使用者相關的資訊。 建議您停用使用者，而非刪除使用者。 如需詳細資訊，請參閱[停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p><p>規劃</p></td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>您必須是Adobe Admin Console的管理員。</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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
    >若要深入瞭解，請參閱[為什麼我無法存取停用使用者所擁有的報告？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) [報告常見問題集](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)文章的區段。

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

<!--

     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

-->
* 更新
* 時數

  >[!NOTE]
  >
  >這些物件仍保留在Workfront中，但物件的擁有者現在為空白。

* 如果使用者在「全域導覽列」的「檔案」區域下上傳了任何檔案，也會刪除檔案。
* 如果使用者已出庫他們擁有的檔案，且檔案已上傳到主檔案區域（從主功能表存取），則會隨使用者刪除檔案。 如需簽出檔案的詳細資訊，請參閱[簽出檔案](../../../documents/managing-documents/check-out-documents.md)。

如需停用使用者的詳細資訊，請參閱[停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。


<!--

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.

   -->
