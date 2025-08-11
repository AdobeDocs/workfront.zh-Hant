---
title: 從先前的資料自動填入請求
content-type: reference
description: 您可以使用AI來使用先前請求的資料自動填寫請求欄位。
author: Becky
feature: Get Started with Workfront
source-git-commit: cf2ae77ed27b1dd30144f6de31bec474f53f1efb
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# 從先前的資料自動填入請求

>[!NOTE]
>
>* 此功能將作為開放式測試版在以下排程中提供：
>
>   * 每月發行： 2025年9月11日
>   * 每季發行： 2025年10月16日

AI可協助您根據先前的請求自動填寫請求欄位。 您可以在提交請求之前核准或拒絕這些建議。

自動填寫不會覆寫您已填寫的任何欄位。

使用者不會收到他們無法存取的資料建議。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：投稿人或更高版本</p>
   或
   <p>目前：要求或以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題的存取權</p>  </td> 
  </tr> 
   <td role="rowheader">物件許可權</td> 
   <td><p>將請求新增至請求佇列的存取權</p> <p>檢視現有請求或更高的許可權</p> <p>如需設定要求佇列的資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立要求佇列</a>。 </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 填寫表單時取得建議

自動填寫可在您填寫表單時建議欄位值。 當您在請求欄位中輸入值時，Workfront會將這些值與先前的請求進行比較。 如果輸入的值與先前請求中類似內容中的其他欄位值緊密相關，Workfront會建議這些值。

例如，如果診所一律使用相同的計費代碼，Workfront會在輸入診所名稱時，建議在適當的欄位中輸入計費代碼。

若要根據先前的請求使用建議：

1. 開始建立請求。

   如需指示，請參閱[建立及提交要求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 開始填寫欄位。

   當您填寫欄位時，其他欄位可能會顯示建議。

1. 對於每個欄位建議，請為該欄位選取&#x200B;**接受**&#x200B;或&#x200B;**拒絕**。

   ![接受或拒絕建議](assets/accept-reject-suggestion.png)

   或

   在頁面頂端選取「**全部接受**」或「**全部拒絕**」以接受或拒絕所有建議。

   >[!NOTE]
   >
   >當您提交請求時，任何未稽核的建議都會自動被接受。
