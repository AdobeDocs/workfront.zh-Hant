---
product-area: requests
navigation-topic: create-requests
title: 在請求區域中建立和管理檢視
description: 如果您使用新的請求體驗，您可以建立和儲存請求區域的檢視。
author: Becky
feature: Work Management
source-git-commit: 4061163b8b761bc3922bfb95da6c0110b6ee5871
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 3%

---

# 在請求區域中建立和管理檢視

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽Sandbox」環境中使用。</span>

如果您使用新的請求體驗，您可以建立和儲存請求區域的檢視。 這些檢視包括篩選器和欄排列。

您可以在Workfront的要求區域中建立和管理檢視。

>[!IMPORTANT]
>
>* 此功能僅在新的請求體驗中可用。
>* 檢視設定無法在首頁的我的請求Widget中使用。

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

## 在請求區域中建立檢視

您可以在Workfront的要求區域中建立檢視。

1. 若要存取「請求」清單：

   {{step1-to-requests}}

1. 在要求清單中，按一下&#x200B;**檢視**&#x200B;下拉式清單![檢視下拉式清單](assets/view-icon-requests.png)，然後選取&#x200B;**新檢視**。

   ![新檢視](assets/create-new-view.png)

1. 輸入新檢視的名稱，然後按一下[建立]。**&#x200B;**
1. 繼續[在要求區域](#edit-a-view-in-the-requests-area)編輯檢視。

## 在請求區域中編輯檢視

您可以編輯現有檢視，包括您剛建立的檢視。

1. 若要存取「請求」清單：

   {{step1-to-requests}}
1. 在「請求」清單中，找出您要編輯的檢視。

1. （選擇性）若要重新命名檢視，請按一下&#x200B;**檢視**&#x200B;下拉式清單![檢視下拉式清單](assets/view-icon-requests.png)，然後按一下檢視旁邊的三個點功能表，選取&#x200B;**重新命名**，然後輸入檢視的新名稱。
1. 按一下&#x200B;**檢視**&#x200B;下拉式清單![檢視下拉式清單](assets/view-icon-requests.png)，然後選取您要編輯的檢視。
1. <span class="preview">若要將自訂欄位新增為欄，請按一下熒幕右側附近的&#x200B;**新增欄**&#x200B;圖示![新增欄](assets/add-column.png)，然後按一下您想要新增為欄位至檢視的自訂表單欄位旁的加號圖示。</span>

   <span class="preview">附加至清單中物件的表單上的自訂欄位可以新增為欄。</span>

   >[!TIP]
   >
   >您目前無法在生產環境中新增欄。
1. （選擇性）按一下&#x200B;**欄**，然後隱藏、顯示或重新排列要求清單中的欄。

   ![資料行方塊](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >您目前無法在生產環境中新增更多欄。

1. （選擇性）按一下&#x200B;**篩選器**，開始新增條件以決定您要在Planning標籤中檢視哪些請求。

   ![在Planning要求索引標籤中編輯篩選器](assets/filters-editing-box-in-requests-planning-tab.png)

   您可以依下列欄位進行篩選：

   * **Workspace**：與請求表單相關聯的工作區。
   * **記錄型別**：與要求表單關聯的記錄型別。
   * **輸入日期**：提交要求的日期。
   * **要求表單**：用來提交要求的要求表單名稱。
   * **狀態**：要求的狀態。
   * **輸入者**：新增請求的使用者名稱。 如果要求是由Workfront外部的人員加入，則&#x200B;**輸入者**&#x200B;欄位會顯示`N/A`。

   <span class="preview">在預覽環境中，您也可以依已新增至檢視的任何自訂欄位進行篩選。</span>

   您可以有多個&#x200B;**And**&#x200B;或&#x200B;**Or**&#x200B;加入的篩選器。
當您新增篩選條件時，要求清單會自動篩選。



>[!IMPORTANT]
>
> * 檢視的變更會自動儲存。
> * 任何使用檢視的使用者都可以看到檢視的變更。

## 新增檢視到版面配置範本。

Workfront管理員可以將新檢視新增至版面配置範本。

如需指示，請參閱[使用版面配置範本自訂篩選器、檢視和群組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

## 共用檢視

您可以與其他使用者、團隊或群組共用您建立的檢視。

1. 若要存取「請求」清單：

   {{step1-to-requests}}

1. 在「要求」清單中，找到您要共用的檢視。
1. 將滑鼠停留在您要共用的檢視上，然後在三點功能表出現時按一下。
1. 選取「**分享**」。
1. 在開啟的對話方塊中，輸入您要與其共用檢視的使用者、專案團隊或群組名稱，然後在它們出現時從清單中選取它們。
1. 按一下「**儲存**」。

