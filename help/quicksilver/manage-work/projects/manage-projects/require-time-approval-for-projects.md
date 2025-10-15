---
product-area: projects
navigation-topic: manage-projects
title: 專案需要時間核准
description: 您可以設定專案，要求專案擁有者核准針對專案記錄的時數。 若以此方式設定，時數必須先由專案所有者核准，然後才能有資格用於計費記錄。
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# 專案需要時間核准

<!--audited: 08/2024-->

您可以設定專案，要求專案擁有者核准針對專案記錄的時數。 若以此方式設定，時數必須先由專案所有者核准，然後才能有資格用於計費記錄。\
如需有關付費記錄的詳細資訊，請參閱文章[建立付費記錄](../../../manage-work/projects/project-finances/create-billing-records.md)。

>[!NOTE]
>
>啟用此選項不會移除時程表核准者核準時程表上時間的能力。 如果專案所有者未核准或拒絕時間，時程表核准者仍可核準時程表上的時間。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>若要在專案上要求核准時間：</p>
   <ul><li><p>標準</p></li>
   <li><p>規劃</p></li></ul>

<p>若要核准專案上記錄的時數：</p>
   <ul><li><p>淺色或更高</p></li>
   <li><p>評論或以上</p></li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或以上版本的許可權</p>
  </tr> 
  <tr> 
   <td role="rowheader">其他存取權</td> 
   <td> <p>您必須至少符合下列其中一個條件，才能核准專案時間：</p> 
    <ul> 
     <li>您是具有上述指定存取權和許可權的專案所有者。 在這種情況下，如果存在以下條件之一，您可以執行以下操作： 
      <ul>
       <li>如果您擁有專案的管理許可權，您可以核准或拒絕任何其他使用者在專案上記錄的時數。</li>
       <li> 如果您擁有專案的「貢獻」或「檢視」存取權，您將只能核准或拒絕您或任何其他回報您的使用者記錄的時數。<br></li>
      </ul></li> 
     <li>您擁有對時程表和時數具有管理存取權的計畫授權。 在此案例中：
      <ul>
       <li>您可以核准或拒絕您至少擁有檢視許可權之專案的任何時數。 </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>To require time to be approved on the project:</p>
   <ul><li>New: Standard</li>
   <li>Current: Plan</li></ul>
   
   <p>To approve hours logged on a project:</p>
   <ul><li>New: Light or higher</li>
   <li>Review or higher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects or higher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher</p>
  </tr> 
  <tr> 
   <td role="rowheader">Additional access</td> 
   <td> <p>You must meet at least one of the following conditions to approve time on a project:</p> 
    <ul> 
     <li>You are the Project Owner with the access and permissions specified above. In this case, you can do the following if one of the conditions below exists: 
      <ul>
       <li>If you have Manage permissions on the project, you can approve or reject hours logged on the project by any other user.</li>
       <li> If you have Contribute or View access to the project you will be able to approve or reject only the hours logged by you or any other user that reports you.<br></li>
      </ul></li> 
     <li>You have a Plan license with administrative access to Timesheets &amp; Hours. In this case:
      <ul>
       <li>You can approve or reject any hours on the projects you have at least permissions to View. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>-->

## 專案需要時間核准

若要要求專案經理核准專案的時數，請執行下列步驟：

1. 前往您想要要求核準時數的專案。
1. 按一下專案名稱右側的&#x200B;**更多**&#x200B;圖示![更多圖示](assets/more-icon.png)，然後按一下&#x200B;**編輯**。\
   「編輯專案」對話方塊隨即顯示。

1. 在&#x200B;**專案設定**&#x200B;區段中，選取&#x200B;**需要時間才能核准此專案**。
1. 按一下「**儲存**」。\
   現在，當時間被記錄並核準時，這些小時將被鎖定，並且不能由在專案或時間表上輸入這些小時的使用者更改。 只有Workfront管理員可以調整記錄時間。

## 核准和拒絕專案時間

作為專案經理，您可以核准或拒絕為任務、問題或專案記錄的小時數。

在專案層級核準時數，並不會對記錄時數之任何使用者的時程表造成任何影響。 例如，專案中的時數可能由專案經理核准，但時程表尚未由使用者的經理或時程表核准者核准。

如果您將專案設定為需要核准記錄的時數，專案經理必須核準時數，才能將其納入專案的計費記錄中。 如需有關建立付費記錄的詳細資訊，請參閱文章[建立付費記錄](../../../manage-work/projects/project-finances/create-billing-records.md)。

若要核准或拒絕專案的時數：

1. 前往專案。
1. 按一下左側面板中的&#x200B;**小時**&#x200B;區域。

1. 為問題、任務和專案顯示所記錄的時數，其狀態應為&#x200B;**已提交**。\
   按一下小時專案左側的方塊，以選取您要核准的小時。

1. 按一下小時清單頂端的&#x200B;**核准**&#x200B;圖示![](assets/approve-hours-icon.png)。\
   時數的狀態變更為&#x200B;**已核准**。\
   如果您稍後拒絕核准的時數，時數的狀態會變更為&#x200B;**未核准**。\
   當您在付費記錄中包含核准的時數時，時數的狀態會變更為&#x200B;**已付費和已核准**。 無法刪除新增到計費記錄的時數。 如需有關建立付費記錄的詳細資訊，請參閱文章[建立付費記錄](../../../manage-work/projects/project-finances/create-billing-records.md)

1. （選擇性）按一下&#x200B;**拒絕**&#x200B;圖示![](assets/reject-hours-icon.png)以拒絕專案上的時間專案。\
   時數的狀態變更為&#x200B;**已拒絕**。

   >[!NOTE]
   >
   >   如果您選取的時數包含在已標示為「已記帳」或「已記帳且已核准」的記帳記錄中，則不會顯示「核准」和「拒絕」圖示。 您只能核准計費記錄中未計費的時數。

