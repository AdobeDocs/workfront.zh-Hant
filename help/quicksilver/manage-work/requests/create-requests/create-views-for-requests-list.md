---
product-area: requests
navigation-topic: create-requests
title: 在請求區域中建立檢視
description: 如果您使用新的請求體驗，您可以建立和儲存請求區域的檢視。
author: Becky
feature: Work Management
source-git-commit: 1c7e2fb7de500083f0f7e42f1016323305054d88
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# 在請求區域中建立或編輯檢視

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它只能在「預覽Sandbox」環境中使用。</span>

如果您使用新的請求體驗，您可以建立和儲存請求區域的檢視。 這些檢視包括篩選器和欄排列。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
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

{{step1-to-requests}}

1. （選擇性和條件性）如果下列專案適用於您的組織和Workfront執行個體，請選取畫面右上角的&#x200B;**切換至新體驗**&#x200B;設定：

   * 您的組織已購買Workfront套件
   * 您的組織已加入Adobe Unified Experience。
   * 您的管理員已授與您存取Workfront Planning的許可權
   * 您至少擁有Workfront Planning工作區的檢視許可權

   如需詳細資訊，請參閱[提交Adobe Workfront Planning要求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)

1. 按一下&#x200B;**檢視**&#x200B;下拉式清單![檢視下拉式清單](assets/view-icon-requests.png)，然後選取&#x200B;**新檢視**。

   ![新檢視](assets/create-new-view.png)

1. 輸入新檢視的名稱，然後按一下[建立]。****
1. 繼續[在要求區域](#edit-a-view-in-the-requests-area)編輯檢視。

## 在請求區域中編輯檢視

您可以編輯現有檢視，包括您剛建立的檢視。

{{step1-to-requests}}

1. （選擇性和條件性）如果下列專案適用於您的組織和Workfront執行個體，請選取畫面右上角的&#x200B;**切換至新體驗**&#x200B;設定：

   * 您的組織已購買Workfront套件
   * 您的組織已加入Adobe Unified Experience。
   * 您的管理員已授與您存取Workfront Planning的許可權
   * 您至少擁有Workfront Planning工作區的檢視許可權

   如需詳細資訊，請參閱[提交Adobe Workfront Planning要求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)1。

1. （選擇性）若要重新命名檢視，請按一下&#x200B;**檢視**&#x200B;下拉式清單![檢視下拉式清單](assets/view-icon-requests.png)，然後按一下檢視旁邊的三個點功能表，選取&#x200B;**重新命名**，然後輸入檢視的新名稱。
1. 按一下&#x200B;**檢視**&#x200B;下拉式清單![檢視下拉式清單](assets/view-icon-requests.png)，然後選取您要編輯的檢視。
1. （選擇性）按一下&#x200B;**篩選器**，開始新增條件以決定您要在Planning標籤中檢視哪些請求。

   ![在Planning要求索引標籤中編輯篩選器](assets/filters-editing-box-in-requests-planning-tab.png)

   您可以依下列欄位進行篩選：

   * **Workspace**：與請求表單相關聯的工作區。
   * **記錄型別**：與要求表單關聯的記錄型別。
   * **輸入日期**：提交要求的日期。
   * **要求表單**：用來提交要求的要求表單名稱。
   * **狀態**：要求的狀態。
   * **輸入者**：新增請求的使用者名稱。 如果要求是由Workfront外部的人員加入，則&#x200B;**輸入者**&#x200B;欄位會顯示`N/A`。

   您可以有多個&#x200B;**And**&#x200B;或&#x200B;**Or**加入的篩選器。
當您新增篩選條件時，要求清單會自動篩選。

1. （選擇性）按一下&#x200B;**欄**，然後隱藏、顯示或重新排列要求清單中的欄。

   ![資料行方塊](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >您無法再新增任何欄。

>[!IMPORTANT]
>
> * 檢視的變更會自動儲存。
> * 任何使用檢視的使用者都可以看到檢視的變更。

## 新增檢視到版面配置範本。

Workfront管理員可以將新檢視新增至版面配置範本。

如需指示，請參閱[使用版面配置範本自訂篩選器、檢視和群組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。
