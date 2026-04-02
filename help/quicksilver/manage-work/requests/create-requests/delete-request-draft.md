---
product-area: requests
navigation-topic: create-requests
title: 刪除提交的請求或請求草稿
description: 您可以在Adobe Workfront中刪除已提交的請求或請求草稿。
author: Alina
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# 刪除提交的請求或請求草稿

您可以刪除Adobe Workfront或Adobe Workfront Planning已提交的請求，或是您已建立或擁有其管理許可權的請求草稿。

Workfront管理員和Workfront Planning工作區管理員也可以刪除未建立的請求和請求草稿。

您無法在舊版請求體驗中檢視Planning請求。

本文說明如何在新請求體驗中刪除請求草稿。 刪除Workfront和Planning請求或其草稿是相同的。

如需詳細資訊，請參閱：

* [建立並提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [從草稿建立請求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)
* [提交Adobe Workfront Planning請求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何Workfront或Workflow套件</p>

<p>用於管理Planning請求的任何Workfront Planning套件 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>投稿人或以上</p>
   <p>要求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員或Planning工作區管理員，才能刪除未建立的請求。</p><p>您必須擁有問題的編輯存取權。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>您必須先建立請求或草稿，才能在新的請求體驗中刪除該請求或草稿，或者您必須是Workfront管理員或Planning工作區管理員，才能刪除未提交的請求草稿。
   </p><p>您必須擁有您要刪除問題的編輯許可權。</p>  </td> 
  </tr>

</tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除新請求體驗中的請求或請求草稿

您可以刪除下列區域中的請求與草稿：

* 在Workfront的要求區域中
* 在首頁我的請求Widget中
* 從請求頁面

下列使用者可以刪除請求草稿：

* Workfront管理員可以刪除他們或其他人提交的請求和草稿。
* Workfront Planning工作區管理員可以刪除Planning工作區中由其管理的請求和草稿。
* 使用者可以刪除他們提交的請求和草稿。

### 從「首頁」的「請求」區域或「我的請求」Widget中刪除請求或草稿

{{step1-to-requests}}

1. 若要存取&#x200B;**首頁**&#x200B;中的&#x200B;**我的請求** Widget：

   {{step1-to-home}}

   1. 找到&#x200B;**我的請求** Widget。

      如需&#x200B;**我的要求**&#x200B;介面工具集的詳細資訊，請參閱[使用我的要求Widget](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)。

1. 在&#x200B;**要求**&#x200B;清單或&#x200B;**首頁**&#x200B;中的&#x200B;**我的要求** Widget中，將游標移至您要刪除的要求或草稿上，然後按一下&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)

1. 按一下&#x200B;**刪除**

   或

   以滑鼠右鍵按一下選取的請求，然後按一下&#x200B;**刪除**。

   >[!TIP]
   >
   >當您無權建立問題時，您會收到一則警告，指出管理員限制您建立請求。

1. 在開啟的對話方塊中，按一下&#x200B;**刪除**。

   已刪除請求或草稿。

   已刪除的請求會儲存在資源回收筒，而Workfront管理員最多可在30天內復原這些請求。 草稿無法復原。

### 從清單中大量刪除請求

{{step1-to-requests}}

1. 若要存取&#x200B;**首頁**&#x200B;中的&#x200B;**我的請求** Widget：

   {{step1-to-home}}

   1. 找到&#x200B;**我的請求** Widget。

      如需有關「我的請求」Widget的詳細資訊，請參閱[使用「我的請求」Widget](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)。

1. 在&#x200B;**請求**&#x200B;清單或&#x200B;**我的請求** Widget中，按一下要刪除之每個請求左側的方塊。
1. 在頁面底部的藍色列中，按一下&#x200B;**刪除**。

   >[!NOTE]
   >
   >如果藍色列中看不到&#x200B;**刪除**&#x200B;選項，則您沒有刪除一或多個選取之要求的許可權。

### 刪除請求草稿的先決條件

您必須先執行下列動作，才能刪除請求草稿：

* 開始建立請求。 這會自動將請求儲存為「草稿」區段中的草稿。

  如需建立請求的相關資訊，請參閱[建立並提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

## 刪除舊版請求體驗中的請求草稿

如果您認為草擬請求不再相關，可在草擬請求儲存為草稿後將其刪除。 您無法復原已刪除的草稿請求。

您無法從舊版請求體驗存取Planning請求或其草稿。

{{step1-to-requests}}

1. 按一下左側面板中的&#x200B;**草稿**。

   所有請求佇列的所有草稿都會顯示在此清單中。

1. 在清單中選取草稿，然後按一下清單頂端的&#x200B;**刪除**。
1. 按一下&#x200B;**是，刪除**。

   草稿已刪除，無法復原。






