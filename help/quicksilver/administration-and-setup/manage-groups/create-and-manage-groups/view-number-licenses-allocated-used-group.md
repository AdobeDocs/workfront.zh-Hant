---
title: 查看組中分配和使用的許可證數
description: 作為Adobe Workfront管理員，您可以查看組及其子組中當前使用的各種許可證類型的計數。 當您需要評估是否重新分發許可證時，此功能非常有用。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: 0e8f8973ad4c1310b973bae4e6fe3578c05db204
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# 查看組中分配和使用的許可證數

作為Adobe Workfront管理員，您可以查看組及其子組中當前使用的各種許可證類型的計數。 當您需要評估是否重新分發許可證時，此功能非常有用。

如果您管理的組上有任何組，則其管理員也可以為您的組執行此操作。 對於Workfront管理員（對於任何組）也是如此。

>[!IMPORTANT]
>
>只有當用戶的家庭組是用戶的家庭組時，才會在特定組中計算用戶的許可證。

## 訪問要求

要執行本文中的步驟，必須具備以下條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>計劃 </p> <p>您必須是組的組管理員或Workfront管理員。 有關詳細資訊，請參見 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用戶完全管理訪問權限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要瞭解您擁有的計畫或許可證類型，請與Workfront管理員聯繫。

## 查看組中使用的許可證數

1. 按一下 **主菜單** 表徵圖 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png)。

1. 在左面板中，按一下 **組** ![](assets/groups-icon.png)。

1. 按一下組的名稱。
1. 在顯示的頁面上，在靠近右上角的標題區域中查看 **使用中的許可證** 表徵圖 **計畫** 和 **工作** 當前正在使用的許可證。

   如果您正在查看頂級組，而Workfront管理員為該組定義了每個許可證類型的最大數量，則還會顯示這些數字。 例如，在下面的組中，最多10個用戶可以擁有計畫許可證，15個用戶可以擁有工作許可證：

   ![](assets/licenses-used-allocated.png)

   有關Workfront管理員如何為組定義最大數量的已分配許可證的資訊，請參閱一節 [設定家庭組的最大許可證計數](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) 在文章中 [管理系統中的可用許可證](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)。

   >[!NOTE]
   >
   >如果您正在查看的組是子組，則只能查看正在使用的許可證數，而不能查看為組分配的最大許可證數。 這是因為Workfront管理員沒有為子組定義最大許可證計數。
   >
   >![](assets/subgroup-used-licenses-only.png)

1. 對於組中當前使用的每種類型許可證（包括審閱和請求）的單獨計數，請按一下正下方的文本區域 **正在使用的許可證：**

   ![](assets/click-text-to-see-more.png)

   該顯示框為所有四種Workfront許可證類型提供了相同的資訊：計畫、工作、複查和請求。 在框的底部，您可以看到此組成員或其子組成員使用的許可證總數：

   ![](assets/more-license-info.png)

   對於「審閱」和「請求」許可證，「最大」列始終顯示「無限制」。
