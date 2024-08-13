---
title: 授予Portfolio存取權
user-type: administrator
product-area: system-administration;portfolios
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront投資組合的存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f4a9c4f3-8ed4-4629-aced-9cc09b8acd3f
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# 授予投資組合的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對投資組合的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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

+++

## 使用自訂存取層級設定投資組合的使用者存取權

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下Portfolio右側&#x200B;**檢視**&#x200B;或&#x200B;**編輯**&#x200B;按鈕上的齒輪圖示![](assets/gear-icon-settings.png)，然後在&#x200B;**微調您的設定**&#x200B;下選取您要授與的功能。

   ![](assets/fine-tune-portfolios.png)

   >[!NOTE]
   >
   >當您為特定型別的物件設定存取層級設定時，該設定不會影響使用者存取排名較低的物件。 例如，您可以限制使用者刪除其存取層級的專案組合，但這不會限制他們刪除排名低於專案組合的專案。如需物件階層的詳細資訊，請參閱[瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)一文中的[相互相依性和物件階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)一節。

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成時，按一下&#x200B;**儲存**。

   建立存取層級後，您可以將其指派給使用者。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 依授權型別存取產品組合

如需有關每個存取層級中的使用者可以對產品組合執行哪些操作的資訊，請參閱文章[每個物件型別可用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)中的[Portfolio](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#portfoli)小節。

## 存取共用的投資組合

作為投資組合的擁有者或建立者，您可以授予其他使用者對投資組合的許可權，與他們共用，如[共用投資組合](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md)中所述。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

當您與另一個使用者共用任何物件時，收件者對該物件的權利取決於兩個專案的組合：

* 您授予收件者的物件許可權
* 收件者物件型別的存取層級設定

如需使用者在共用投資組合時可授與的許可權相關資訊，請參閱[共用投資組合](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md)。
