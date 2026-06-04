---
title: 授予使用者對特定區域的管理存取權
description: 身為Adobe Workfront管理員，您可以使用存取層級，授予擁有計畫授權的使用者對系統特定區域的管理存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
TQID: https://experienceleague.adobe.com/1nXA0NxLQW3tiIrhCKAd5EMfqBjQW68GHNN42dQmptQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 686
ht-degree: 5%

---

# 授予使用者管理特定區域的存取權

<!--Linked in several places, do not rename or change URL.-->

身為Adobe Workfront管理員，您可以使用存取層級，授予具有「標準」或「計畫」授權的使用者對系統特定區域的管理存取權。

>[!NOTE]
>
>這與授與使用者Workfront的完整管理存取權（在[授與使用者完整管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)中說明）不同&#x200B;。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>   <p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 授予Standard或Plan使用者對Workfront特定區域的管理存取權

>[!IMPORTANT]
>
>我們強烈建議您維持內建的存取層級不變，以便在設定使用者後參考。 若要自訂存取層級，請複製預設存取層級並修改副本。 （除了系統管理員和外部使用者之外，您可以對每個存取層級執行此動作。）

{{step-1-to-setup}}

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
      <td role="rowheader">我的群組中的里程碑</td> 
      <td>在「設定」的「里程碑路徑」選單下，檢視系統中的所有里程碑路徑。 使用者也可以編輯或刪除屬於任何群組的所有里程碑路徑。 使用者無法管理（編輯或刪除）未指派給任何群組的里程碑路徑。<br><p>若無此存取權，使用者只能檢視現有的里程碑路徑，並將其套用至他們有權管理的專案。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>在Workfront中建立及管理提醒通知。<br>若無此存取權，使用者只能接收及檢視通知。</td> 
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


<!--     
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> <p><b>NOTE</b>: In the Preview environment, access to job roles is controlled as an object type in the access level. See <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-job-roles.md">Grant access to job roles</a>.</p>
      <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Standard or Plan user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Standard or Plan user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
     </tr>
-->
