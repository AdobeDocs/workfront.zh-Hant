---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 重新排序組狀態
description: 作為組管理員，您可以更改項目、任務的順序，並為您管理的組發出狀態。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 6%

---

# 重新排序組狀態

作為組管理員，您可以更改項目、任務的順序，並為您管理的組發出狀態。

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。

>[!NOTE]
>
>* Workfront管理員可重新排序系統層級的狀態。 這不會影響群組內的狀態順序。
>
>  但是，新建立的頂層組中的狀態將繼承系統層狀態的順序。 （新子組將繼承組中狀態的順序，向上一層。）
>
>* 您可以重新排序鎖定的狀態。 有關鎖定狀態的資訊，請參閱 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>


## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫* </td> 
   <td>任何</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 狀態的預設順序

依預設，狀態會依下列順序顯示：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">專案</th> 
   <th width="33.33%">任務</th> 
   <th width="33.33%">問題</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>目前</p> 
     <p>廢棄</p> 
     <p> 保留 </p> 
     <p> 計畫 </p> 
     <p> 已完成 </p> 
     <p> 已請求 </p> 
     <p> 已核准 </p> 
     <p> 已拒絕 </p> 
     <p> 構想 </p> 
   </td> 
   <td> 
     <p>新增</p> 
     <p>進行中</p> 
     <p>已完成</p> 
   </td> 
   <td> 
     <p>新增</p> 
     <p>進行中</p> 
     <p>重新打開</p> 
     <p>等待反饋</p> 
     <p>保留</p> 
     <p>無法複製</p> 
     <p>已關閉</p> 
     <p>已解決</p> 
     <p>確認完成</p> 
     <p>不會解決</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## 重新排序您管理之群組中任務和專案的狀態

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組**，然後按一下群組的名稱。
1. 在左側面板中，按一下 **狀態**.
1. 在顯示的狀態清單上方，按一下 **專案** 或 **工作** 標籤。

1. 依您想要的順序拖放狀態。

   新狀態順序會自動保存。

1. 要測試新狀態順序，請轉至與組關聯的任務或項目，按一下右上角的狀態，並確保顯示的狀態按您配置的順序。

## 重新排序問題的狀態

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組**，然後按一下群組的名稱。
1. 在左側面板中，按一下 **狀態**.
1. 按一下 **問題** 標籤。
1. （選用）選取問題類型(**錯誤報告**, **變更順序**, **問題**，或 **要求**)。

   >[!NOTE]
   >
   >* 不能自定義主清單的狀態順序。
   >* 建議您以相同方式，為每個問題類型排序狀態。 如需問題類型的詳細資訊，請參閱 [設定請求類型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. 依您想要的順序拖放狀態。

   新狀態順序會自動保存。

1. 要測試新狀態順序，請轉至與組關聯的問題，按一下右上角的狀態，並確保顯示的狀態按照您配置的順序。
