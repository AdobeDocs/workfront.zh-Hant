---
product-area: requests
navigation-topic: create-requests
title: 在請求區域中建立和管理檢視
description: 如果您使用新的請求體驗，您可以建立和儲存請求區域的檢視。
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 31aff197d6af521df2258f3f99fea6fb5785b9e3
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 3%

---


# 在請求區域中建立和管理檢視

<!--

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

如果您在Adobe Workfront中使用新的請求體驗，您可以建立和儲存請求區域的檢視。 這些檢視包括篩選器、欄排列和群組。

>[!IMPORTANT]
>
>* 此功能僅在請求區域的新請求體驗中可用。
>* 檢視設定也可在首頁的「我的請求」Widget中使用。 不過，請求區域的檢視與我的請求Widget的檢視不同。
>* 「請求」區域和「我的工作」Widget中的請求清單，會使用Workfront中的增強清單。 如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

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
   <p>任何Workfront Planning授權，以在請求清單中檢視Workfront Planning請求</p>
    </td> 
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
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 請求的系統檢視

>[!WARNING]
>
>此章節中記錄的系統檢視尚無法使用。 這些功能將於2026年4月16日之後推出。

除了您可以自行建立的檢視外，Workfront還在首頁的「請求」區域和「我的請求」Widget中提供下列系統檢視：

* **所有請求**：您或其他任何人在佇列或工作區中提交且您有權檢視的所有請求。 這不適用於我的請求Widget。
* **我的請求**：無論狀態為何，您提交的請求。
* **我的未完成請求**：您已經提交且仍在未完成中的請求。
* **我的草稿**：您的要求草稿尚未提交。
* **開啟的要求**：您或其他人在佇列中提交的要求，或您有權檢視且仍在開啟的工作區的要求。 這不適用於我的請求Widget。

您無法編輯系統檢視。 您可以修改其元素，然後複製檢視並編輯或共用副本。

## 建立請求檢視

使用新請求體驗時，您可以在Workfront的請求區域中建立檢視。 啟用和新請求體驗後，您也可以在首頁為「我的請求」Widget建立檢視。

1. 若要存取&#x200B;**要求**&#x200B;清單：

   {{step1-to-requests}}

   1. 請確定&#x200B;**使用新體驗**&#x200B;設定已開啟。

1. 若要存取首頁的&#x200B;**我的請求** Widget：

   {{step1-to-home}}

   1. 新增或前往&#x200B;**我的請求** Widget。

1. 在要求清單中，按一下&#x200B;**檢視**&#x200B;下拉式功能表![檢視下拉式功能表](assets/view-icon-requests.png)，然後按一下&#x200B;**新增檢視**。

   <!-- 
   
   replace the screen shot with release
   ![New view](assets/create-new-view.png)

   -->

1. 輸入新檢視的名稱，然後按一下[建立]。****
1. 繼續[編輯要求的檢視](#edit-a-view-for-requests)。

## 編輯請求的檢視

您可以編輯現有檢視，包括您剛才在要求區域中建立的檢視或首頁中的我的要求Widget 。

透過編輯檢視，您可以變更檢視的下列元素：

* 名稱
* 篩選器
* 欄
* 分組
* 設定儲存格格式
* 列高

如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

<!-- 
hide these details - all the information is in "Use enhanced lists" - we need one point of messaging for this feature: 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!-keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.

1. (Optional) Click **Columns** to open the **Fields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
-->

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * 檢視的變更會自動儲存。
> * 只有在您對檢視進行變更後共用新的檢視副本時，使用該檢視的任何人都可以看到檢視的變更。
> * 在任何以使用者作為值的欄位中使用&#x200B;**我（已登入的使用者）**&#x200B;篩選器萬用字元。

## 將請求檢視新增到版面配置範本

Workfront管理員可以在請求區域的版面配置範本中新增檢視。

如需指示，請參閱[使用版面配置範本自訂篩選器、檢視和群組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

## 共用檢視

您可以與其他使用者、團隊、群組或公司共用您建立的檢視。

共用檢視後，其他使用者可以在共用檢視之前檢視您為檢視編輯的更新檢視元素。

如果他們更新檢視，其他人將無法看到他們的更改，除非他們製作同一檢視的副本，並在共用副本之前保留他們的更改。

如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

<!--
Let's just redirect to Use enhanced lists so we avoid duplicating information. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. 
-->