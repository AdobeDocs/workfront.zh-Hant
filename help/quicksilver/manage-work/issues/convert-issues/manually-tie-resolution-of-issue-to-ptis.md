---
product-area: projects
navigation-topic: convert-issues
title: 手動將問題的解決連結至其他問題、任務或專案
description: 您可以手動將問題的解決連結至專案、任務或問題的解決，而不轉換問題。 問題會成為您選取之專案、任務或問題的可解析物件之一。 當您這樣做時，專案、任務或問題狀態的變更會觸發原始問題狀態的變更。
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 1%

---

# 手動將問題的解決連結至其他問題、任務或專案

<!--Audited: 08/2025-->

您可以手動將問題的解決連結至專案、任務或問題的解決，而不轉換問題。 問題會成為您選取之專案、任務或問題的可解析物件之一。 當您這樣做時，專案、任務或問題狀態的變更會觸發原始問題狀態的變更。

>[!TIP]
>
>當您將問題的解決繫結到另一個物件的解決時，您無法再手動編輯原始問題的狀態。

如需有關解析和可解析物件的詳細資訊，請參閱[解析和可解析物件概觀](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

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
   <td><p>投稿人或以上</p> 
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題、任務、專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理您連結至其他問題、任務或專案之問題的許可權</p> <p>檢視或授予您新增至現有問題的問題、任務或專案的更高許可權</p>  </td> 
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
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues,&nbsp;Tasks, Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 先決條件

開始之前，您必須：

* 有您想要將其解決方案連結至其他問題、任務或專案解決方案的問題

* 有其他問題、任務或專案

## 將問題的解決連結至另一個問題、任務或專案的解決

1. 瀏覽至您想要將其解決方案連結至另一個問題的解決方案，或是任務或專案的解決方案的問題。
1. 按一下左側面板中的&#x200B;**問題詳細資訊**，然後展開&#x200B;**概觀**&#x200B;區域。

   ![問題詳細資訊圖示](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. 按一下&#x200B;**解析者**&#x200B;欄位，然後從下列解析物件型別中選取：

   * **專案**
   * **任務**
   * **問題**

   根據您選取的物件，會顯示下列欄位：

   * **解析專案**
   * **解析任務**
   * **正在解決問題**

1. 在&#x200B;**解決專案**、**任務**&#x200B;或&#x200B;**問題**&#x200B;欄位中開始輸入特定專案、任務或問題的名稱，然後當它出現在清單中時按一下它。

   >[!NOTE]
   >
   >您無法將問題的解決連結至問題所在的任務或專案。 問題的任務或專案未顯示在解決任務或解決工作列位中。


1. 按一下「**儲存變更**」。

   原始問題會變成您在步驟4和步驟5中選取的專案、任務或問題的可解析物件。 這表示解析物件（您連結至的專案、任務或問題）完成時，原始問題就會完成。

   >[!NOTE]
   >
   >一個專案、任務或問題可能具有多個問題作為可解析物件。
