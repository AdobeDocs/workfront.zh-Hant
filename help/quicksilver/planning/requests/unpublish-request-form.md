---
title: 在Adobe Workfront Planning中取消發佈請求表單
description: 如果您不再需要或不相關的請求表單，您可以取消發佈該表單。 取消發佈後，您就會移除每個人存取表單的許可權。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 4%

---

# 在Adobe Workfront Planning中取消發佈請求表單


<!--take Preview and Production references at Production time-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

如果您不再需要或不相關的請求表單，您可以取消發佈該表單。 取消發佈後，您就會移除每個人存取表單的許可權。

如果您希望讓一小群人可以使用請求表單，也可以變更與您共用請求表單的實體。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<ul><li><p>任何Workfront套件</p></li>
與
<li><p>任何Planning套件</p></li></ul>
或
<ul><li><p>任何Workflow封裝</p></li>
與
<li><p>任何Planning套件</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區與記錄型別</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 變更請求表單的共用

如果您與所有人（包括組織外部的使用者）共用公開的要求，您可以考慮將此存取許可權製為只有檢視或管理表單相關聯之工作區的特定使用者。

若要變更請求表單的共用：

{{step1-to-planning}}

1. 按一下您要共用表單的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   記錄型別頁面會在您上次存取的檢視中開啟。 依預設，會在表格檢視中開啟記錄型別頁面。

1. 按一下頁面標頭中記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**管理請求表單**。

   與記錄型別相關的所有請求表單都會顯示在表格檢視中。
1. 暫留在要求表單的名稱上，然後按一下名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**共用**。
1. 選取下列其中一項，更新共用選擇：

   * 在工作區擁有檢視或更高存取權限的任何人
   * 對工作區具有貢獻或更高權限的任何人
   * 擁有此連結的任何人

   如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。
1. （選擇性）如果您已變更要求表單的共用，而且想要透過新連結與新群組的人共用，請按一下&#x200B;**複製連結**。

## 取消發佈記錄型別的請求表單

當請求表單變得無關緊要，並且您不希望任何人再存取它時，您可以取消發佈。

{{step1-to-planning}}

1. 按一下您要新增記錄的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   記錄型別頁面會在您上次存取的檢視中開啟。 依預設，會在表格檢視中開啟記錄型別頁面。

1. 按一下頁面標頭中記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**管理請求表單**。

   與記錄型別相關的所有請求表單都會顯示在表格檢視中。
1. 暫留在要求表單的名稱上，然後按一下名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**取消發佈**

或

按一下要求表單的名稱以開啟它，然後按一下要求表單右上角的&#x200B;**取消發佈**。

![取消發佈按鈕醒目提示](assets/unpublish-button-highlighted.png)

畫面底部會顯示確認訊息，通知您表單已取消發佈。

**取消發佈**&#x200B;連結或按鈕變更為&#x200B;**發佈**。

1. （視條件而定）如果您在開啟表單後取消發佈表單，請按一下&#x200B;**儲存**。

   使用者無法再透過連結或Workfront要求區域中的要求佇列存取要求表單。

   先前使用請求表單新增的任何記錄都會保留在記錄型別頁面上。

   先前新增的任何請求都會保留在Workfront的「請求」區域的「計畫」標籤上。
