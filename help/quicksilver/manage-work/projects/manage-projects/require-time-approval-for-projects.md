---
product-area: projects
navigation-topic: manage-projects
title: 需要為項目批准的時間
description: 需要為項目批准的時間
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# 需要為項目批准的時間

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

您可以設定專案，要求專案擁有者核准依專案記錄的時數。 以此方式配置時，小時數必須先經項目所有者批准，才有資格用於計費記錄。\
如需帳單記錄的詳細資訊，請參閱文章 [建立計費記錄](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>啟用此選項不會刪除工時單批准者在工時單上批准時間的能力。 如果項目所有者未批准或拒絕時間，則時間表審批者仍可批准時間表上的時間。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計畫需要在項目上獲得批准的時間</p>
   <p>檢閱或更高版本，以核准登入專案的時數</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對專案或以上版本的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案或更新版本的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他存取</td> 
   <td> <p>您至少必須符合下列條件之一，才能核准專案的時間：</p> 
    <ul> 
     <li>您是專案擁有者，具有上述指定的存取權和權限。 在此情況下，如果存在下列其中一個條件，您可以執行下列操作： 
      <ul>
       <li>如果您對專案擁有「管理」權限，則可以核准或拒絕任何其他使用者登入專案的時數。</li>
       <li> 如果您擁有專案的「貢獻」或「檢視」存取權，則您只能核准或拒絕您或任何其他報表使用者記錄的小時數。<br></li>
      </ul></li> 
     <li>您擁有計畫許可證，可以管理對工時單和工時的訪問。 在此情況下：
      <ul>
       <li>您至少可以在具有「檢視」權限的專案上，核准或拒絕任何時數。 </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 需要為項目批准的時間

要在項目上要求項目經理批准數小時，請執行以下操作：

1. 轉到需要批准數小時的項目。
1. 按一下 **更多** 圖示 ![](assets/more-icon.png) 在專案名稱的右側，按一下 **編輯**.\
   「編輯專案」對話方塊隨即顯示。

1. 在 **專案設定** 部分，選擇 **需要為此項目批准的時間**.
1. 按一下&#x200B;**儲存**。\
   現在，當時間被記錄並批准時，這些小時將被鎖定，並且無法由在項目或時間表中輸入這些小時的用戶更改。 只有Workfront管理員可以調整記錄的時間。

## 批准和拒絕項目時間

作為項目經理，您可以批准或拒絕記錄任務、問題或項目的時數。

在項目級別批准工時不會對記錄工時的任何用戶的工時單產生任何影響。 例如，項目中的工時可能由項目經理批准，但工時單仍有待用戶經理或工時單批准者批准。 

如果您將項目設定為需要在記錄的小時數上進行審批，項目經理必須批准該小時數，以便這些小時數可被納入項目的計費記錄中。 有關建立計費記錄的詳細資訊，請參閱文章 [建立計費記錄](../../../manage-work/projects/project-finances/create-billing-records.md).

要批准或拒絕項目的工時，請執行以下操作：

1. 前往專案。
1. 按一下 **小時** 框中。 這可能位於 **顯示更多** 的上界。

1. 針對問題、工作和專案記錄的小時數會顯示，且狀態應為 **已提交**.\
   按一下小時條目左側的框，以選擇要批准的小時數。

1. 按一下 **核准**.\
   小時的狀態變更為 **已核准**.\
   如果您稍後拒絕批准的小時數，則小時的狀態將更改為 **未批准**.\
   當您將核准的小時數納入計費記錄時，小時的狀態會變更為 **計費和批准**. 無法刪除添加到計費記錄的小時數。 有關建立計費記錄的詳細資訊，請參閱文章 [建立計費記錄](../../../manage-work/projects/project-finances/create-billing-records.md)

1. （選用）按一下 **拒絕** 拒絕項目上的時間條目。\
   小時的狀態變更為 **已拒絕**.
