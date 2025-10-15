---
product-area: projects
navigation-topic: convert-issues
title: 將問題與其解決物件取消連結
description: 當您透過將問題轉換為專案或任務來建立專案或任務時，您有選項可保留原始問題。 您的Adobe Workfront管理員必須啟用此偏好設定，您才能在轉換問題期間擁有此選項。 如需將問題轉換為專案和任務的詳細資訊，請參閱在Adobe Workfront中轉換問題的總覽。
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 將問題與其解析物件取消連結

<!--Audited: 08/2025-->

當您透過將問題轉換為專案或任務來建立專案或任務時，您有選項可保留原始問題。 您的Adobe Workfront管理員必須啟用此偏好設定，您才能在轉換問題期間擁有此選項。\
如需將問題轉換為專案和任務的詳細資訊，請參閱[在Adobe Workfront中轉換問題的總覽](../../../manage-work/issues/convert-issues/convert-issues.md)。

當您決定保留已轉換為專案或任務的問題時，問題的解決方案會與專案或任務繫結。 問題會成為專案或任務的可解析物件。 專案或任務是問題的解決物件。

您也可以手動將問題連結至另一個問題。 在這種情況下，第二個問題會成為第一個問題的解決物件。\
如需有關解析物件的詳細資訊，請參閱[解析和可解析物件的概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

>[!TIP]
>
>問題狀態無法變更，因為它會自動變更解析物件的狀態。

您可以從問題中移除專案、任務或問題，藉此取消問題解決方案與專案、任務或問題解決方案的連結。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>投稿人或以上</p>
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題的存取權</p> <p>檢視任務與專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理問題的許可權</p> <p>檢視任務或專案的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 從專案、任務或問題中取消問題連結

1. 移至連結至專案、任務或問題的問題。
1. 按一下&#x200B;**問題詳細資料**&#x200B;區段。
1. 移至&#x200B;**問題詳細資訊**&#x200B;區段的&#x200B;**總覽**&#x200B;區域。
1. 在&#x200B;**解析者**&#x200B;欄位中，移除可解析物件型別。\
   問題可由專案、任務或問題解決。

   這會將解析物件從問題中移除。

1. 按一下&#x200B;**儲存** **變更**。\
   問題不再連結至專案、任務或問題，您現在可以獨立解決問題。
