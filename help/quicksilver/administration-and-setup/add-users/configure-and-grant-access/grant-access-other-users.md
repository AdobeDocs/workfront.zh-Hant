---
title: 授予使用者存取許可權
description: 作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中其他使用者的存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
TQID: https://experienceleague.adobe.com/jLoqncsE3CSAK27siU8Ro2EQdZkbJC-gs040vGxX-5E
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 900
ht-degree: 3%

---

# 授予使用者存取許可權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中其他使用者的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

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
   <td><p>標準</p>
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

## 設定使用者的存取權

您可以使用預設存取層級或您建立的自訂存取層級，來管理使用者可以檢視和編輯的其他使用者資訊。 具有預設「標準」、「計畫」和「工作」授權的使用者可以檢視其他使用者的聯絡資訊。 下列任一使用者都可以建立及編輯其他使用者：

* Workfront管理員。

  如需詳細資訊，請參閱[授予使用者完整管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)。

* 具有預設Standard或Plan授權的使用者，也可以存取使用者，如本文所述。

  僅限於檢視其公司或主要公司使用者的使用者，只能編輯其可看到的使用者。 如需詳細資訊，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 具有預設Standard或Plan授權的使用者，也指定為其他使用者的管理員。

  在存取層級中授予使用者「編輯」存取許可權的使用者可以管理向其報告的使用者。 如需有關管理使用者的資訊，請參閱[檢視組織圖](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md)。

* 具有預設Standard或Plan授權的使用者建立使用者時，可以停用、刪除或編輯他們建立的使用者。 如需有關建立新使用者的資訊，請參閱[新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 設定使用者的存取權，以使用自訂存取層級編輯使用者

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 若要變更擁有標準、計畫或工作授權的使用者檢視其他使用者資訊的能力，請按一下&#x200B;**使用者**&#x200B;右側&#x200B;**檢視**&#x200B;按鈕上的齒輪圖示![齒輪圖示](assets/gear-icon-settings.png)，然後在&#x200B;**微調您的設定**&#x200B;方塊中選取您要授與的檢視選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>檢視收費率</strong> </td> 
      <td> 允許使用者檢視使用者設定檔的計費費率。</td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>檢視連絡人資訊</strong> </td> 
      <td> 允許使用者檢視其他使用者的使用者詳細資訊頁面。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>檢視成本費率</strong> </td> 
      <td> 允許使用者檢視使用者設定檔的成本率。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>檢視一般財務</strong> </td> 
      <td> 允許使用者檢視使用者設定檔上的一般財務欄位（與帳單或成本費率無關）。</td>
     </tr> 
    </tbody> 
   </table>

   ![微調檢視使用者設定](assets/fine-tune-view-users.png)

1. 若要修改具有Standard或Plan授權存取許可權的使用者編輯其他使用者的能力，請按一下&#x200B;**使用者**&#x200B;右側&#x200B;**編輯**&#x200B;按鈕上的齒輪圖示![齒輪圖示](assets/gear-icon-settings.png)，然後在&#x200B;**微調您的設定**&#x200B;方塊中選取您要授與的編輯選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>建立</strong> </td> 
      <td> <p>允許使用者建立使用者。<br>此選項預設為啟用。</p> 
     <p><b>注意</b>：如果您的組織已加入Adobe Admin Console，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。<!--Check this October 2026--></p>
        </td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>刪除</strong> </td> 
      <td> <p> 允許使用者刪除他們自己建立的使用者。<br>此選項預設為啟用。</p> <p><b>注意</b>：如果您的組織已加入Adobe Admin Console，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。<!--Check this October 2026--></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>編輯收費率</strong> </td> 
      <td> 允許使用者編輯使用者設定檔的計費費率。</td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>編輯成本費率</strong> </td> 
      <td> 允許使用者編輯使用者設定檔的成本率。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>編輯一般財務</strong> </td> 
      <td> 允許使用者編輯使用者設定檔上的一般財務欄位（與帳單或成本費率無關）。</td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>使用者管理員（所有使用者）</strong> </td> 
      <td> <p>允許使用者為Workfront中的任何使用者執行下列動作：</p> 
       <ul> 
        <li>編輯、刪除或停用使用者</li> 
        <li>以使用者身分登入<p><b>注意</b>：您無法作為系統管理員的任何使用者登入。</p></li> 
        <li>重設使用者密碼</li> 
       </ul> <p>此選項預設為停用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>使用者管理員（群組使用者）</strong> </td> 
      <td> <p>允許使用者對其所管理的群組中的任何使用者執行下列動作： 
        <ul>
         <li><p>編輯、刪除或停用使用者</p></li>
         <li>以使用者身分登入</li>
         <li><p>重設使用者密碼</p><p><b>注意</b>：群組管理員無法以Workfront管理員身分登入或重設密碼。</p></li>
        </ul><p>此選項預設為停用。</p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>檢視收費率</strong> </td> 
      <td> 允許使用者檢視使用者設定檔的計費費率。</td>  
     </tr>
     <tr> 
      <td role="rowheader"><strong>檢視成本費率</strong> </td> 
      <td> 允許使用者檢視使用者設定檔的成本率。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>檢視一般財務</strong> </td> 
      <td> 允許使用者檢視使用者設定檔上的一般財務欄位（與帳單或成本費率無關）。</td>
     </tr>
    </tbody> 
   </table>

   >[!TIP]
   >
   >如果您不想要授與群組管理員對其所管理群組之所有成員的存取權，請停用上述兩個「使用者管理員」選項。 群組管理員仍可存取他們新增至Workfront的群組成員，或在Workfront中向他們報告的群組成員。

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成時，按一下&#x200B;**儲存**。

## 依授權型別存取使用者

如需有關每個存取層級中的使用者可以對使用者執行哪些操作的資訊，請參閱文章[每個物件型別可用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)中的[使用者](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users)小節。
