---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新問題狀態
description: 您可以更新問題的狀態，以通知其他人問題的位置及其進展。
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# 更新問題狀態

您可以更新問題的狀態，以通知其他人問題的位置及其進展。

## 存取需求

<!--drafted for P&P;

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
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯問題的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理問題的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 問題狀態

以下是Workfront中問題的預設狀態：

* 新增
* 進行中
* 等待反饋
* 保留
* 不會解決
* 重新打開
* 已關閉
* 已解決

您的Adobe Workfront管理員可針對貴組織的問題新增自訂狀態。 它們也可以根據問題類型提供狀態。

如需自訂狀態和問題類型的詳細資訊，請參閱下列文章：

* [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [建立問題](../../../manage-work/issues/manage-issues/create-issues.md)

您可以手動更新問題狀態，也可以讓Workfront在發生某些動作時自動更新。

## 手動更新問題狀態

在更新問題狀態時，您還可以添加有關新狀態的說明，並更改其他問題資訊，如提交日期。

1. 轉至您要更新狀態的問題。
1. 按一下 **狀態** 欄位，然後選取新狀態。

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. 若要提供問題完成的視覺指示，請拖曳或連按兩下下方的泡泡 **完成百分比** 在問題的標題中。

   或

   按一下問題標題內的泡泡以輸入百分比。

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. （可選）執行下列任一操作以提供有關更新的其他資訊，然後按一下 **更新** 或者，如果問題的狀態等於「完成」，請按一下 **完成：**

   * 若要新增有關更新的附註，請前往 **更新** 區段，按一下 **開始新更新**，然後輸入您的備注。

      ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * 若要通知特定使用者有關更新的資訊，請在 **通知** 框中，此框將在您鍵入有關更新的備注時顯示。 如需詳細資訊，請參閱 [在更新時標籤其他人](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * 若要更新問題的條件，請按一下 **條件**，然後選取最能反映問題目前狀況的條件。 從下列選項中選取：

      * 進展順利
      * 部分關注事項
      * 主要障礙
   * 要更新問題的提交日期，請展開 **提交日期** 下拉式日曆，然後選取新日期。


## 自動更新問題狀態

當下表所列的動作發生時，Workfront會自動將問題的現有狀態更新為不同狀態。

>[!NOTE]
>
>下表中的狀態為預設系統狀態。 您的Workfront管理員或群組管理員可以重新命名Workfront例項中的狀態。 如需在Workfront中建立和管理狀態的相關資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>動作</td> 
   <td>原始狀態</td> 
   <td>新狀態</td> 
  </tr> 
  <tr> 
   <td>將問題完成百分比更新為100%</td> 
   <td>新的或正在進行中</td> 
   <td>已關閉</td> 
  </tr> 
  <tr> 
   <td>將問題完成百分比從100%更新為較低的數字</td> 
   <td>已關閉 </td> 
   <td>進行中</td> 
  </tr> 
  <tr> 
   <td>更新附加到問題的解決對象的狀態</td> 
   <td>各種狀態</td> 
   <td> <p>各種狀態</p> <p>有關解決對象及其如何影響問題狀態的資訊，請參閱文章中的「將可解析對象的狀態與解決對象的狀態同步」一節 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>按一下「開始問題」按鈕以接受處理指派給您的問題</span> </td> 
   <td><span>新增</span> </td> 
   <td> <p>與「首頁團隊」設定中的「開始問題」按鈕相關的任何狀態。 </p> <p>有關用「開始問題」按鈕替換「Work On It」按鈕的資訊，請參閱 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕</a></span><span>.</span> </p> <p>提示：按一下 <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">還原按鈕</span> 按一下「開始問題」後，狀態會回復為「新增」。 </p> </td> 
  </tr> 
 </tbody> 
</table>
