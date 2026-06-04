---
product-area: requests
navigation-topic: create-requests
title: 從草稿建立請求
description: 除了使用Workfront在您輸入新請求時向您建議的可用草稿之外，您還可以從「草稿」區段存取草稿請求並從那裡完成提交。
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/LyLchKrtMU1ffu--wjrys6zyRr5gZm6saJoxxg82m-M
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 857
ht-degree: 2%

---

# 從草稿建立請求

除了使用Workfront在您輸入新請求時向您建議的可用草稿之外，您還可以從「草稿」區段存取草稿請求並從那裡完成提交。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何Adobe Workfront或Workflow套件</p>
   <p>可建立Adobe Workfront Planning請求的任何Workfront Planning套件 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>投稿人或以上</p>
   <p>要求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題的存取權</p>  </td> 
  </tr>

</tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從草稿建立請求的先決條件

您必須先執行下列動作，才能從草稿建立請求：

* 開始建立請求。 這會自動將請求儲存為「草稿」區段中的草稿。

  如需建立請求的相關資訊，請參閱[建立並提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

## 從草稿建立請求

您可以從草稿為Workfront與Planning請求建立請求。

從草稿建立請求的新請求體驗和舊版體驗不同。

* [從新請求體驗中的草稿建立請求](#create-requests-from-drafts-in-the-new-requesting-experience)
* [從舊版請求體驗中的草稿建立請求](#create-requests-from-drafts-in-the-legacy-requesting-experience)

### 從新請求體驗中的草稿建立請求

1. 開啟草稿。

   草稿可在下列位置找到：

   * 在請求清單的請求區域
   * 在首頁我的請求Widget中的請求清單中
   * 在新請求對話方塊中（僅包含以所選表單建立的請求草稿）

   >[!NOTE]
   >
   >在舊版請求體驗中建立的草稿在新請求體驗中無法使用。

1. 依照[建立和提交Adobe Workfront要求](../../../manage-work/requests/create-requests/create-submit-requests.md)中的說明更新要求的資訊。
1. （選擇性和條件性）在輸入請求期間，如果想要刪除草稿，請按一下&#x200B;**捨棄**&#x200B;草稿。 這將刪除草稿。

   如果您誤棄草稿，可以立即在熒幕底部的訊息中按一下&#x200B;**還原**。 此選項僅供幾秒鐘使用。

   如需有關刪除草稿的詳細資訊，請參閱[刪除提交的請求或請求草稿](../../../manage-work/requests/create-requests/delete-request-draft.md)。

1. （選用）若要儲存草稿的變更而不提交，請離開新請求頁面。 變更會自動儲存。

1. 完成要求的資訊後，請按一下&#x200B;**提交**。

   當您提交請求時，草稿會被新請求取代，且無法恢復為草稿。

### 從舊版請求體驗中的草稿建立請求

>[!NOTE]
>
>您無法使用舊版體驗從Planning請求草稿建立請求。


{{step1-to-requests}}

1. 在左側面板中選取&#x200B;**草稿**。

   此清單中會顯示每個請求佇列之每個佇列主題的草稿。

   ![草稿區段包含草稿清單](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. （選擇性）按一下欄標題，依該欄排序清單。

1. 在「草稿」清單的下列欄位中複查有關每個草稿的資訊：

   | 主旨 | 這是您開始建立請求時為其提供的名稱。 |
   | --- | --- |
   | 路徑 | 您原本要提交請求的請求佇列、主題群組和佇列主題的名稱。 |
   | 輸入日期 | 您起始建立請求的日期。 |
   | 上次更新日期 | 您上次更新的日期。 如果您在第一次開始請求後沒有更新，「輸入日期」和「上次更新日期」應該相同。 |

   {style="table-layout:auto"}

1. （選擇性）使用「草稿」清單右上角的快速篩選，開始輸入草稿請求、請求佇列、佇列主題或主題群組的名稱，然後按一下草稿名稱以開啟它。

   >[!TIP]
   >
   >您無法在請求區域的草稿區段中套用永久篩選器。 此外，沒有選項可修改或變更草稿清單的檢視。

1. 依照[建立和提交Adobe Workfront要求](../../../manage-work/requests/create-requests/create-submit-requests.md)中的說明更新要求的資訊。
1. （選擇性和條件性）在輸入請求期間，如果想要刪除草稿，請按一下&#x200B;**捨棄**&#x200B;草稿。 這將刪除無法復原的草稿。 如需有關刪除草稿的詳細資訊，請參閱[刪除請求草稿](../../../manage-work/requests/create-requests/delete-request-draft.md)。

1. （選擇性）如果您要回覆動作並保留草稿，請按一下頁面左下角的&#x200B;**取消**。

1. 完成請求的資訊後，請執行下列任一項作業：

   * 如果您已準備好提交要求，請按一下&#x200B;**提交**。 請求會儲存在「已提交」區段。 根據「請求佇列」的「路由規則」，此請求可能會路由至指定為「請求佇列」的不同專案。 如需路由規則的詳細資訊，請參閱[建立路由規則](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)。

     或

     如果您尚未準備好提交，請按一下&#x200B;**關閉**，稍後可能會回來完成它。 您的請求會儲存在「草稿」區段，當您下次提交此請求佇列的請求時，即可使用此請求。

     ![新要求上的提交、關閉、捨棄按鈕](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     當您提交請求時，草稿會被刪除且無法還原。

