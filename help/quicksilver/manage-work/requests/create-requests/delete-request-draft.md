---
product-area: requests
navigation-topic: create-requests
title: 刪除已提交的請求重新請求草稿
description: 您可以刪除已提交的請求或請求草稿。
author: Becky
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: 8b08336431d2e4ebfcb078d8329f8748fac66eda
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 3%

---

# 刪除提交的請求或請求草稿

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽」環境中供所有客戶使用，或在「生產」環境中供啟用快速發行的客戶使用。</span>

您可以刪除已提交的請求，或是您在新的請求體驗中建立的請求草稿。 Workfront管理員和Planning工作區管理員也可以刪除請求。

在舊版請求體驗中，您可以刪除請求草稿。 您無法刪除已提交的請求。

如需詳細資訊，請參閱：

* [建立並提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [從草稿建立請求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)

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
   <td> <p>您必須是Workfront管理員或Planning工作區管理員，才能刪除未建立的請求。</p><p>您必須擁有問題的編輯存取權，才能刪除舊版請求體驗中的草稿。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>您必須先建立請求或草稿，才能在新的請求體驗中刪除它。</p><p>您必須擁有問題的編輯存取權，才能刪除舊版請求體驗中的草稿。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 產品</td> 
   <td> <ul><li>Adobe Workfront</li><li>您必須安裝Adobe Workfront Planning才能檢視Planning請求或請求表單</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<div class="preview">

## 刪除新請求體驗中的請求<!--or request drafts -->

您可以在Workfront的「請求」區域或「首頁」的「我的請求」Widget中刪除請求。

* Workfront管理員可以刪除其組織中的請求<!-- and drafts-->。
* Workfront Planning工作區管理員可以刪除他們所管理的Planning工作區中的請求<!--and drafts-->。
* 使用者可以刪除他們提交的要求<!--and drafts-->。

若要刪除新請求體驗中的請求或草稿：

1. 若要存取「要求」清單，請按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 要求]**。

1. 若要存取「首頁」中的「我的請求」Widget：

   1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
   1. 找出「我的請求」Widget。

      如需有關「我的請求」Widget的詳細資訊，請參閱[使用「我的請求」Widget](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)。

1. 在「請求」清單或「我的請求」Widget中，暫留在您要刪除的請求<!--or draft -->上。

   出現「更多」三點選單。
   ![](assets/more-menu.png)

1. 按一下要求&#x200B;**名稱右側的**&#x200B;更多<!--or draft-->功能表，然後按一下&#x200B;**刪除**。

   或

   以滑鼠右鍵按一下選取的請求，然後按一下&#x200B;**刪除**。

   >[!TIP]
   >
   >當您無權建立問題時，您會收到一則警告，指出管理員限制您建立請求。

1. 在開啟的對話方塊中，按一下&#x200B;**刪除**。

   已刪除要求<!--or draft-->。

</div>

## 刪除舊版請求體驗中的請求草稿

如果您認為草擬請求不再相關，可在草擬請求儲存為草稿後將其刪除。 您無法復原已刪除的草稿請求。

### 刪除請求草稿的先決條件

您必須先執行下列動作，才能刪除請求草稿：

* 開始建立請求。 這會自動將請求儲存為草稿區段中的草稿。

  如需建立請求的相關資訊，請參閱[建立並提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

### 刪除請求草稿

{{step1-to-requests}}

1. 在左側面板中選取&#x200B;**草稿**。

   所有請求佇列的所有草稿都會顯示在此清單中。

1. （選擇性）按一下草稿清單右上角的&#x200B;**依請求型別篩選**，然後選取包含您要顯示之草稿的請求佇列。
1. 在清單中選取草稿，然後按一下清單頂端的&#x200B;**刪除**。
1. 按一下&#x200B;**是，刪除**。

   草稿已刪除，無法復原。
