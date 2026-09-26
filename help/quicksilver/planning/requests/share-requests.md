---
title: 共用計畫請求
description: 提交Workfront計畫請求後，您就可以與其他人共用該請求。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3934b1b333f86c8c700617871bfaac23d2b19213
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%
---
# 共用計畫請求

<!--add to TOC, and miniTOC-->

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 在「預覽」版發行後，啟用的客戶每月可在「生產」環境中使用相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

提交Planning請求後，您可以控制誰能看到請求、誰能處理請求，以及允許每個人員或團隊採取哪些動作。 這可以讓適當的人員專注於適當的請求，並確保他們只能採取與其角色適當的行動。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>具有Planning套件的任何Workfront或工作流程</p> 
或
<p>任何以獨立產品形式購買的Workfront Planning</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>任何</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>任何</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>擁有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到存取層級</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>如果您是Workfront使用者，可檢視或更高許可權的工作區和記錄型別</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共用請求時的注意事項

* 您可以將下列許可權授予請求的使用者：

  * 檢視：使用者只能看到請求。
  * 貢獻：使用者可以檢視、編輯和評論請求。
  * 管理：使用者可以檢視、編輯、評論和刪除請求。

* 系統會自動授予請求者管理許可權，以存取其提交的請求，除非管理員已設定其他預設值。

  如需詳細資訊，請參閱[建立請求表單](/help/quicksilver/planning/requests/create-request-form.md)。

* Workfront管理員可存取及管理所有請求。
* 擁有記錄型別管理存取權的使用者會繼承該記錄型別輸入表單的管理存取權，以及透過其提交的每個請求的管理存取權。
* 擁有請求許可權的任何人都可以共用具有相同許可權層級的請求，或比自己的許可權層級更低的層級。

  擁有「貢獻」許可權的使用者無法將「管理」許可權授與他人該請求。

* 不同的人員和團隊可針對相同請求保留不同的存取層級。
* 許可權可透過多個實體指派。 如果使用者擁有請求的Contribute許可權，但其群組或工作角色擁有檢視許可權，則他們仍會保留Contribute的最高許可權層級。
* 請求從工作區和記錄型別繼承許可權。 您無法移除或編輯Planning要求的繼承許可權。

## 共用請求

確保您使用新的請求體驗。

1. {{step1-to-requests}}
1. 尋找Planning請求，然後按一下以開啟該請求。
1. 按一下&#x200B;**共用**。

   已針對選取的請求開啟&#x200B;**共用**&#x200B;方塊。

   ![要求共用方塊](assets/requests-sharing-box.png)

1. 在&#x200B;**授與此要求欄位**&#x200B;的存取權中，開始輸入使用者、團隊、角色、群組或公司的名稱，並在其顯示在清單上時按一下該名稱。

   只有作用中的實體會顯示在清單中。
1. 從每個實體名稱右側的下拉式功能表中，選取下列其中一個許可權層級：

   * 管理
   * 參與
   * 檢視
1. （選擇性）對於每個許可權等級，按一下精細的許可權圖示，然後選取或取消選取任何精細的許可權，例如&#x200B;**編輯**、**註解**、**共用**&#x200B;或&#x200B;**刪除**。

   ![請求的精細許可權](assets/granular-permissions-on-requests.png)
1. （可選）展開「繼承許可權」行以檢視誰從工作區和記錄型別獲得許可權。

   >[!TIP]
   >
   >您無法移除或編輯Planning要求的繼承許可權。

1. 按一下「**儲存**」。


   系統會與您選取的實體共用請求。


