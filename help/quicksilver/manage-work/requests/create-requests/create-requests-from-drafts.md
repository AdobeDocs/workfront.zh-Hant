---
product-area: requests
navigation-topic: create-requests
title: 從草稿建立請求
description: 除了使用Workfront在您輸入新請求時向您建議的可用草稿之外，您還可以從「草稿」區段存取草稿請求並從那裡完成提交。
author: Becky
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 38843e2c093d5af9d74d8b4442fd28e194996e8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 3%

---

# 從草稿建立請求

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽Sandbox」環境中使用。</span>

除了使用Workfront在您輸入新請求時向您建議的可用草稿之外，您還可以從「草稿」區段存取草稿請求並從那裡完成提交。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何 </p> </td> 
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
  <tr> 
   <td role="rowheader"> 產品</td> 
   <td> <ul><li>Adobe Workfront</li><li>您必須安裝Adobe Workfront Planning才能檢視Planning請求或請求表單</td> 
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

從草稿建立請求的程式在新的請求體驗和舊版體驗之間有所不同。

* <span class="preview">[從新請求體驗中的草稿建立請求](#create-requests-from-drafts-in-the-new-requesting-experience)</span>
* [從舊版請求體驗中的草稿建立請求](#create-requests-from-drafts-in-the-legacy-requesting-experience)

<div class="preview">

### 從新請求體驗中的草稿建立請求



<!--
   
1. Open the draft.

   Drafts can be found in the following locations:

   * In the requests list in the Requests area
   * In the requests list in the My Requests widget in Home
   * In the New request dialog (includes only drafts of requests created with the selected form)
   
-->
1. 開啟草稿。

   草稿可在新請求對話方塊中找到（僅包含以所選表單建立的請求草稿）。
1. 依照[建立和提交Adobe Workfront要求](../../../manage-work/requests/create-requests/create-submit-requests.md)中的說明更新要求的資訊。
1. （選擇性和條件性）在輸入請求期間，如果想要刪除草稿，請按一下&#x200B;**捨棄**&#x200B;草稿。 這將刪除草稿。

   如果您誤棄草稿，可以立即在熒幕底部的訊息中按一下&#x200B;**還原**。 此選項僅供幾秒鐘使用。

   如需有關刪除草稿的詳細資訊，請參閱[刪除提交的請求或請求草稿](../../../manage-work/requests/create-requests/delete-request-draft.md)。

1. （選用）若要儲存草稿的變更而不提交，請離開新請求頁面。 變更會自動儲存。

1. 完成要求的資訊後，請按一下&#x200B;**提交**。

   當您提交請求時，草稿會被刪除且無法還原。

</div>

### 從舊版請求體驗中的草稿建立請求

{{step1-to-requests}}

1. 在左側面板中選取&#x200B;**草稿**。

   此清單中會顯示每個請求佇列之每個佇列主題的草稿。

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. （選擇性）按一下欄標題，依該欄排序清單。

1. 在「草稿」清單的下列欄位中複查有關每個草稿的資訊：

   | 主旨 | 這是您開始建立請求時為其提供的名稱。 |
   |---|---|
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

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     當您提交請求時，草稿會被刪除且無法還原。

   >[!NOTE]
   >
   >在新的請求體驗中，草稿與已提交請求位於相同清單中。
   >如需有關在新體驗中建立要求的詳細資訊，請參閱「建立及提交要求」一文中的[在Workfront網頁應用程式中建立要求並產生草稿](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md#create-requests-and-generate-drafts-in-the-workfront-web-app)。

