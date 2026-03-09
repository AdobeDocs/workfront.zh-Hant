---
product-area: requests
navigation-topic: create-requests
title: 在請求區域中建立和管理檢視
description: 如果您使用新的請求體驗，您可以建立和儲存請求區域的檢視。
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: e4d57d0b5042dc4889d5b676396b56c05ab1515d
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 2%

---


# 在請求區域中建立和管理檢視

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>





如果您在Adobe Workfront中使用新的請求體驗，您可以建立和儲存請求區域的檢視。 這些檢視包括篩選器和欄排列。

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* 此功能僅在請求區域的新請求體驗中可用。
>* 檢視設定也可在首頁的「我的請求」Widget中使用。 不過，請求區域的檢視與我的請求Widget的檢視不同。
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
   <td> <p>編輯問題的存取權</p>  <p>您必須是Workfront管理員才能新增檢視到版面配置範本</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 產品</td> 
   <td> <ul><li>Adobe Workfront</li><li>您必須安裝Adobe Workfront Planning才能檢視Planning請求或請求表單</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立請求檢視

使用新請求體驗時，您可以在Workfront的請求區域中建立檢視。

1. 若要存取「請求」清單：

   {{step1-to-requests}}

1. 請確定&#x200B;**使用新體驗**&#x200B;設定已開啟。

1. 在&#x200B;**要求**&#x200B;清單中，按一下&#x200B;**檢視**&#x200B;下拉式功能表![檢視下拉式功能表](assets/view-icon-requests.png)，然後按一下&#x200B;**新增檢視**。

   ![新檢視](assets/create-new-view.png)

1. 輸入新檢視的名稱，然後按一下[建立]。****
1. 繼續[在要求區域](#edit-a-view-in-the-requests-area)編輯檢視。

## 編輯請求的檢視

您可以編輯現有檢視，包括您剛才在Workfront的「要求」區域中建立的檢視。

透過編輯請求區域中的檢視，您可以變更檢視的下列元素：

* 名稱
* 篩選器
* 欄

您對檢視所做的變更，對您共用該檢視的所有使用者都是可見的。

1. 若要存取請求中的請求清單，請執行下列動作：

   {{step1-to-requests}}

1. 請確定&#x200B;**使用新體驗**&#x200B;設定已開啟。
1. 在&#x200B;**要求**&#x200B;清單中，找出您要從&#x200B;**檢視**&#x200B;下拉式功能表![檢視下拉式功能表](assets/view-icon-requests.png)編輯的檢視。

1. 按一下&#x200B;**檢視**&#x200B;下拉式清單![檢視下拉式清單](assets/view-icon-requests.png)，然後按一下檢視旁邊的三個點功能表，選取&#x200B;**重新命名**，然後輸入檢視的新名稱。
1. 按下Enter以儲存新名稱。
1. 按一下&#x200B;**檢視**&#x200B;下拉式清單![檢視下拉式清單](assets/view-icon-requests.png)，然後選取您要編輯的檢視。
1. 若要將欄位新增為欄，請按一下清單右上角的&#x200B;**新增欄**&#x200B;圖示![新增欄](assets/add-column.png)。

   **資料行管理員**&#x200B;開啟。
1. 按一下您要新增為欄位至檢視的欄位旁的加號圖示，然後按一下&#x200B;**儲存**。

   與清單中物件關聯的欄位可新增為欄。<!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >新增至欄的欄位必須先存在，才可在&#x200B;**欄管理員**&#x200B;中使用。


1. （選擇性）按一下&#x200B;**欄**&#x200B;以開啟F **欄可見度和順序**&#x200B;方塊。
1. 開啟您要在清單中顯示的每個欄位的設定，關閉它以隱藏它，或以不同的順序拖放欄位。

1. （選擇性）按一下&#x200B;**篩選器**，然後開始為您要檢視的請求新增條件。

   您可以依下列請求欄位進行篩選：

   * **Workspace**：與請求表單相關聯的工作區。
   * **物件型別**：與要求表單關聯的記錄型別。
   * **輸入日期**：提交要求的日期。
   * **要求表單**：用來提交要求的要求表單名稱。
   * **狀態**：要求的狀態。
   * **輸入者**：新增請求的使用者名稱。 如果要求是由Workfront外部的人員加入，則&#x200B;**輸入者**&#x200B;欄位會顯示`N/A`。

   您也可以依已新增至檢視的任何欄位來篩選檢視中可見的任何物件。

   您可以有多個&#x200B;**And**&#x200B;或&#x200B;**Or**加入的篩選器。
當您新增篩選條件時，要求清單會自動篩選。


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * 檢視的變更會自動儲存。
> * 任何使用檢視的使用者都可以看到檢視的變更。
> * 在任何以使用者作為值的欄位中使用&#x200B;**我（已登入的使用者）**&#x200B;篩選器萬用字元。

## 將請求檢視新增到版面配置範本。

Workfront管理員可以將新檢視新增至版面配置範本。

如需指示，請參閱[使用版面配置範本自訂篩選器、檢視和群組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

## 共用檢視

您可以與其他使用者、團隊或群組共用您建立的檢視。

1. 若要存取請求中的請求清單，請執行下列動作：

   {{step1-to-requests}}

1. 請確定&#x200B;**使用新體驗**&#x200B;設定已開啟。
1. 在&#x200B;**要求**&#x200B;清單中，找出您要共用的檢視。
1. 將游標暫留在您要共用的檢視上，然後按一下檢視名稱右側的三個點功能表，再按一下[共用]。****
1. 在&#x200B;**共用**&#x200B;方塊中，輸入您要共用檢視的人員、團隊、角色、群組或公司，然後在它們出現時從清單中選取它們。
1. 按一下「**儲存**」。

   檢視與您指定的實體共用。 他們可以在共用檢視之前檢視您為檢視編輯的更新檢視元素。 <span class="preview">如果他們更新檢視，其他人將無法看到他們的變更，除非他們製作相同檢視的復本，並在共用復本之前保留變更。 如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。</span>
