---
title: 授予使用者管理特定區域的存取權
description: 身為Adobe Workfront管理員，您可以使用存取層級，授予擁有計畫授權的使用者對系統特定區域的管理存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 2%

---

# 授予使用者管理特定區域的存取權

<!--Linked in several places, do not rename or change URL.-->

身為Adobe Workfront管理員，您可以使用存取層級，授予擁有計畫授權的使用者對系統特定區域的管理存取權。

>[!NOTE]
>
>這與授與使用者Workfront的完整管理存取權（在[授與使用者完整管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)中說明）不同&#x200B;。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予Plan使用者對Workfront特定區域的管理存取權

>[!IMPORTANT]
>
>我們強烈建議您維持內建的存取層級不變，以便在設定使用者後參考。 若要自訂存取層級，請複製預設存取層級並修改副本。 （除了系統管理員和外部使用者之外，您可以對每個存取層級執行此動作。）

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 在左側面板中，按一下&#x200B;**存取層級**。
1. 按一下您要用來授予使用者對Workfront特定區域之管理存取權的存取層級名稱。
1. 在&#x200B;**允許**&#x200B;的管理存取許可權區段中，核取方塊可授與必要的管理存取許可權。

   這些選項可讓您授與下列功能：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">核准程序</td> 
      <td><p>建立並管理整個系統和特定群組的核准流程。</p><p>若無此存取權，使用者只能對其有權管理的專案建立臨時核准流程。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td><p>在Workfront中新增及編輯現有公司</p>
      <p>若無此存取權，使用者只能檢視現有公司。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂表單</td> 
      <td><p>在其群組中建立和編輯（新增、編輯和刪除欄位）自訂表單。</p><p>若無此存取權，使用者只能將現有表單附加至他們有權貢獻或管理的物件。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯率</td> 
      <td> <p>在Workfront中新增貨幣。</p> <p>如果沒有此存取權，使用者只能將現有貨幣新增到他們建立的專案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td><p>檢視Workfront中物件的所有費用。</p><p>這不允許使用者建立新的費用型別。</p><p>若無此存取權，使用者只能檢視下列專案：</p>
       <ul>
        <li>專案、任務或問題管理的費用</li>
        <li>他們自己的費用</li>
        <li>其下屬的費用</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">職務角色</td> 
      <td> <p>透過此存取權，使用者可以執行下列動作：</p> 
       <ul> 
        <li>檢視和編輯現有職位角色</li> 
        <li>新增職位角色</li> 
        <li>編輯角色帳單和成本費率</li> 
       </ul> <p><b>重要</b>：如果您授與供需規劃員使用者工作角色的管理存取權，將會自動為使用者啟用「財務資料」存取設定「編輯角色帳單與成本費率」。 稍後，如果您停用供需規劃員使用者對工作角色的管理存取權，使用者仍可看見工作角色，因為編輯角色帳單與成本費率設定仍處於啟用狀態。 如果發生此情況，並且您需要移除使用者檢視工作角色的存取權，您需要停用使用者的「編輯角色帳單和成本費率」許可權設定。 如需指示，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予財務資料的存取權</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的群組中的里程碑</td> 
      <td>在「設定」的「里程碑路徑」選單下，檢視系統中的所有里程碑路徑。 使用者也可以編輯或刪除屬於任何群組的所有里程碑路徑。 使用者無法管理（編輯或刪除）未指派給任何群組的里程碑路徑。<br><p>若無此存取權，使用者只能檢視現有的里程碑路徑，並將其套用至他們有權管理的專案。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>在Workfront中建立和管理提醒通知。<br>若無此存取權，使用者只能接收及檢視通知。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">時間表和時數</td> 
      <td> <p>允許使用者檢視Workfront中的所有時數與時間表。</p> <p>停用此選項時，使用者只可以在以下時間檢視小時：</p> 
       <ul> 
        <li>他們管理的專案、任務或問題</li> 
        <li>他們自己的時間表</li> 
        <li>他人所報之時程表</li> 
        <li>他們核准的時程表</li> 
       </ul> <p><b>附註</b>：  <p>無論此選項是啟用還是停用，群組管理員都可以為他們管理的群組和子群組建立時間表設定檔，並將其指派給他們有權編輯其使用者設定檔的群組成員。</p> <p>啟用此選項可能會為某些群組管理員提供太多存取權，因為他們可以檢視系統中所有使用者（而不僅僅是他們管理的群組中的使用者）的時程表設定檔產生的時程表（以及時數）。 您可以為不需要太多存取許可權的群組管理員停用此選項。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 完成時，按一下&#x200B;**儲存**。
1. 將新的存取層級指派給使用者，如[新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)中所述。

   >[!NOTE]
   >
   >您可以允許使用者管理使用者的存取權。 如需有關授予使用者管理存取許可權以便他們能夠管理使用者帳戶的詳細資訊，請參閱[授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。
