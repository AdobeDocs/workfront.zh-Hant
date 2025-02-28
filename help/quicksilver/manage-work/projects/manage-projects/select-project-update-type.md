---
product-area: projects
navigation-topic: manage-projects
title: 選取專案更新型別
description: 透過為專案選取更新型別，您可以控制您對專案時間表所做的變更在父任務或專案上的儲存頻率。
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# 選取專案更新型別

透過為專案選取更新型別，您可以控制您對專案時間表所做的變更在父任務或專案上的儲存頻率。

更新專案時間表時，會根據對專案所做的變更、其任務或對時間表所依賴的其他專案所做的變更來重新計算時間表。

例如，專案上任務的下列變更會觸發時間表的更新  專案的：

* 更新任務日期
* 變更任務的前置任務關係
* 除了變更任務限制或期間型別外，變更父子關係、新增或移除工作分派。

## 存取需求

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>規劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 更新專案的更新型別

任務更新時，其父物件（父任務或專案）會在「更新型別」所指示的時間更新。  若要指定專案的更新型別，請執行下列動作：

1. 前往您要指定其更新型別的專案。
1. 按一下專案名稱旁的「更多」功能表![「更多」圖示](assets/more-icon.png)，然後按一下「**編輯**」。

1. 按一下&#x200B;**專案** **設定**。

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. 在&#x200B;**更新型別**&#x200B;欄位中，選取您是否希望Workfront每天自動計算專案的時間表、當有變更時，或是希望專案經理手動計算。

   從下列清單中的選項中選取。 

   >[!IMPORTANT]
   >
   >如果專案的時間表超過15年，Workfront不會自動計算或於變更時計算時間表。 超過15年的專案更新型別一律為手動。

   * **自動與變更時：**&#x200B;這是預設設定。 每次在專案中或時間表所依存的其他專案中發生變更時，專案時間表都會更新。 專案時間表也會每晚更新。 \
     這是建議的設定，可確保專案時間表隨時保持最新。

     當您更新任務或專案並觸發時間表重新計算時，所有可用日期會立即顯示，允許您繼續工作。 在擁有超過100個任務的專案中，需要更長計算的日期會變暗。

     ![](assets/dates-dimmed-when-insline-editing-350x146.png)

     這表示重新計算尚未完成，日期可能會變更。

   * **僅變更：**&#x200B;每次專案或時間表所依賴的其他專案發生變更時，專案時間表都會更新；不會發生排程更新。\
     如果您擔心系統效能，而且專案或時間表所依賴的其他專案中很少發生變更，您可能會想要選取此選項。

   * **僅限自動：**&#x200B;專案時間表每晚都會更新；變更後不會立即更新。\
     如果您擔心系統效能，以及專案或時間表所依賴的其他專案中每天都發生許多變更，您可能會想要選取此選項。

     >[!NOTE]
     >
     >如果專案處於Planning狀態，則不會每晚自動重新計算。 它只會在變更時重新計算。

   * **僅限手動：**&#x200B;專案時間表只有在您選取&#x200B;**重新計算時間表**&#x200B;的選項時才會更新，如[重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)一節中的「手動重新計算」一節所述。\
     如果您一次對專案進行許多變更，且希望在所有變更完成後（而不是在每次個別變更後）重新計算時間表，則可能需要選取此選項。

1. 按一下「**儲存**」。
