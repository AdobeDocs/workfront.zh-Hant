---
product-area: requests
navigation-topic: create-requests
title: 在「請求」區域中建立和管理視圖
description: 如果使用新的請求體驗，則可以建立並保存「請求」區域的視圖。
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: 78ad910e8d121dda38c9a7da27b0b338e0e1dcda
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 2%

---


# 在「請求」區域中建立和管理視圖

<span class="preview">此頁上的資訊指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 在每月發佈到生產版之後，在生產環境中，對於啟用了快速發佈的客戶也提供了相同的功能。</span>

<span class="preview">有關快速版本的資訊，請參閱[啟用或禁用貴組織的快速版本](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


如果您在Adobe Workfront使用新的請求體驗，則可以建立並保存「請求」區域的視圖。 這些視圖包括篩選器和列安排。

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* 此功能僅在「請求」區域的新請求體驗中可用。
>* 「首頁」中的「我的請求」小部件中也提供了視圖設定。 但是，「請求」區域的視圖與「我的請求」小部件的視圖是分開的。
>* 請求區域中的請求清單會使用Workfront中的增強清單。 如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何Workfront或Workflow套件</p>

<p>任何Worfront Planning許可證，以在請求清單中查看WorkfrontPlanning請求</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront牌照</td> 
   <td> <p>投稿人或以上</p>
   <p>要求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題的存取權</p>  <p>您必須是Workfront管理員才能將視圖添加到佈局模板</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

有關此表中資訊的詳細資訊，請參閱[Workfront文檔中的訪問要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 為請求建立視圖

使用新請求體驗時，可以在Workfront的「請求」區域建立視圖。

1. 要訪問「請求」清單，請執行以下操作：

   {{step1-to-requests}}

1. 確保&#x200B;**啟用新體驗**&#x200B;設定。

1. 在&#x200B;**請求**&#x200B;清單中，按一下&#x200B;**視圖**&#x200B;下拉菜單![視圖下拉清單](assets/view-icon-requests.png)，然後按一下&#x200B;**新建視圖**。

   ![新建視圖](assets/create-new-view.png)

1. 輸入新視圖的名稱，然後按一下&#x200B;**建立**。
1. 繼續[在「請求」區域](#edit-a-view-in-the-requests-area)中編輯視圖。

## 編輯請求的視圖

您可以編輯現有檢視，包括您剛才在Workfront的「要求」區域中建立的檢視。

透過編輯請求區域中的檢視，您可以變更檢視的下列元素：

* 名稱
* 篩選器
* 欄

在視圖上所做的更改對與視圖共用的所有用戶都可見。

1. 要訪問「請求」中的請求清單，請執行以下操作：

   {{step1-to-requests}}

1. 請確定&#x200B;**使用新體驗**&#x200B;設定已開啟。
1. 在&#x200B;**要求**&#x200B;清單中，找出您要從&#x200B;**檢視**&#x200B;下拉式功能表![檢視下拉式功能表](assets/view-icon-requests.png)編輯的檢視。

1. 按一下&#x200B;**檢視**&#x200B;下拉式清單![檢視下拉式清單](assets/view-icon-requests.png)，然後按一下檢視旁邊的三個點功能表，選取&#x200B;**重新命名**，然後輸入檢視的新名稱。
1. 按下Enter以儲存新名稱。
1. 按一下&#x200B;**視圖**&#x200B;下拉清單![視圖下拉清單](assets/view-icon-requests.png)，然後選擇要編輯的視圖。
1. 若要將欄位添加為列，請按一下清單右上角的&#x200B;**添加列**&#x200B;表徵圖![添加列](assets/add-column.png)。

   **列管理器**&#x200B;開啟。
1. 按一下要作為列添加到視圖的欄位旁邊的加號表徵圖，然後按一下&#x200B;**保存**。

   與清單中的對象關聯的欄位可以作為列添加。<!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >添加到列的欄位必須存在，才能在&#x200B;**列管理器**&#x200B;中提供。


1. （選擇性）按一下&#x200B;**欄**&#x200B;以開啟F **欄可見度和順序**&#x200B;方塊。
1. 開啟您要在清單中顯示的每個欄位的設定，關閉它以隱藏它，或以不同的順序拖放欄位。

1. （選擇性）按一下&#x200B;**篩選器**，然後開始為您要檢視的請求新增條件。

   您可以依下列請求欄位進行篩選：

   * **Workspace**：與請求表單相關聯的工作區。
   * **對象類型**：請求表單關聯的記錄類型。
   * **輸入日期**：請求提交的日期。
   * **請求表單**：用於提交請求的請求表單的名稱。
   * **狀態**：要求的狀態。
   * **輸入者**：新增請求的使用者名稱。 如果要求是由Workfront外部的人員加入，則&#x200B;**輸入者**&#x200B;欄位會顯示`N/A`。

   也可以按添加到視圖的任何欄位過濾，以查看中可見的任何對象。

   您可以有多個由&#x200B;**和**&#x200B;或&#x200B;**或**聯接的篩選器。
在添加篩選條件時，將自動篩選請求清單。


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * 視圖更改將自動保存。
> * 對視圖的更改對使用該視圖的任何人都可見。
> * 在任何以用戶為值的欄位中使用&#x200B;**Me（已登錄用戶）**&#x200B;篩選通配符。

## 將請求視圖添加到佈局模板。

Workfront管理員可以將新視圖添加到佈局模板。

有關說明，請參閱[使用佈局模板自定義篩選器、視圖和分組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

## 共用視圖

您可以與其他用戶、團隊或組共用您建立的視圖。

1. 若要存取請求中的請求清單，請執行下列動作：

   {{step1-to-requests}}

1. 請確定&#x200B;**使用新體驗**&#x200B;設定已開啟。
1. 在&#x200B;**要求**&#x200B;清單中，找出您要共用的檢視。
1. 將游標暫留在您要共用的檢視上，然後按一下檢視名稱右側的三個點功能表，再按一下[共用]。****
1. 在&#x200B;**共用**&#x200B;方塊中，輸入您要共用檢視的人員、團隊、角色、群組或公司，然後在它們出現時從清單中選取它們。
1. 按一下「**儲存**」。

   視圖與您指定的實體共用。 它們可以在共用視圖之前查看您為視圖編輯的更新視圖元素。 <span class="preview">如果他們更新了視圖，則其更改將不會對其他人可見，除非他們製作了同一視圖的副本並在共用副本之前保留其更改。 如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。</span>
