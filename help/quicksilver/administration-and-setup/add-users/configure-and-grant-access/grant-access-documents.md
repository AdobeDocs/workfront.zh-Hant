---
title: 授與檔案的存取權
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: 作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中檔案的存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 1%

---

# 授與檔案的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對檔案的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

此存取權也適用於檔案資料夾。

如需使用自訂存取層級來管理使用者對Workfront中其他物件型別的存取的相關資訊，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 使用自訂存取層級設定檔案的使用者存取權

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下檔案右側![](assets/gear-icon-settings.png)檢視&#x200B;**或**&#x200B;編輯&#x200B;**按鈕上的齒輪圖示**，然後在&#x200B;**微調您的設定**&#x200B;下選取您要授與的功能。

   ![document_access.png](assets/document-access.png)

   您可以允許使用者針對其有權存取的專案、任務和問題執行以下操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">建立</td> 
      <td>上傳檔案。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除</td> 
      <td> <p>移除已上傳的檔案。</p> <p>啟用此選項時，<b>建立</b>選項會自動啟用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">共用</td> 
      <td>與特定使用者、工作角色、團隊共用檔案。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">共用公開文件</td> 
      <td>與外部使用者共用檔案(沒有Workfront授權)。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">全系統共用</td> 
      <td> <p>讓您的Workfront執行個體中的每個人都能使用檔案。</p> <p>在下列情況下，系統中的任何人都可以看見以這種方式共用的檔案：</p> 
       <ul> 
        <li> <p>您向他們傳送上傳檔案所在頁面的連結。</p> </li> 
        <li> <p>他們在Workfront中搜尋</p> </li> 
       </ul> <p>啟用此選項時，<b>共用</b>選項會自動啟用。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >當您為特定型別的物件設定存取層級設定時，該設定不會影響使用者存取排名較低的物件。 例如，您可以限制使用者刪除其存取層級的專案，但這不會限制他們刪除等級低於專案的檔案。如需物件階層的詳細資訊，請參閱[瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)一文中的[相互依存性和物件階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)一節。

1. （選擇性）若要限制從較高等級物件繼承的檔案許可權，請按一下[設定其他限制]**，然後選取[從專案、任務、問題等繼承檔案存取權]****。**
1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成時，按一下&#x200B;**儲存**。

   建立存取層級後，您可以將其指派給使用者。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 依授權型別存取檔案

如需有關每個存取層級中的使用者可以對檔案執行的詳細資訊，請參閱文章[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document)可用的功能[檔案](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)一節。

## 存取共用檔案

上傳檔案至Workfront後，您可以授予其他使用者許可權來共用檔案，如[共用檔案](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md)中所述。

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

當您與另一個使用者共用任何物件時，收件者對該物件的權利取決於兩個專案的組合：

* 您授予收件者的物件許可權
* 收件者物件型別的存取層級設定
