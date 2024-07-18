---
product-area: projects;templates
navigation-topic: manage-projects
title: 將專案另存為範本
description: 在專案層級將專案儲存為templateSave as template （範本），讓使用者在UI中看到；此連結的另一篇文章有更深入的連結（逐步進行）。 此功能需要同時保留在專案和範本區域。)」
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 1%

---

# 將專案另存為範本

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

如果您決定某個專案將在未來再次發生，則可以從現有專案建立範本。 然後，您可以再次使用範本來建立未來專案，這些專案可能包含類似的資訊，或與現有專案共用相同的時間表或工作分派。

## 存取需求

<!--drafted for P&P:
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
   <td> <p>Current license: Standard </p>
   Or 
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯範本的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或更高的許可權 </p> <p>將專案另存為範本後，即可取得範本的管理許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 將專案另存為範本

1. 前往您要另存為範本的專案。
1. 按一下&#x200B;**更多**&#x200B;功能表![](assets/qs-more-icon-on-an-object.png)，然後&#x200B;**另存為範本**。
1. 指定範本的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td>指定範本的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>提供範本的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">為作用中</td> 
      <td> <p>從下列選項中選取：</p> 
       <ul> 
        <li> <p><strong>是</strong>：其他使用者可以找到範本並將其附加至專案。</p> </li> 
        <li><strong>否</strong>：其他使用者找不到範本，也無法將其附加至專案。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂表單</td> 
      <td>使用下拉式清單來選取要附加至範本的任何自訂表單。 如果有任何自訂表單已與專案相關聯，則會顯示這些自訂表單中的所有資料欄位。<br>您最多可以在單一範本上包含10個自訂表格。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**管理Forms**&#x200B;以移除或重新排序表格。 如需如何在範本上移除和重新排序自訂表單的相關資訊，請參閱[自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md)。

   ![](assets/save-as-template-first-step-350x159.png)

1. 按一下&#x200B;**下一步。**
1. 在&#x200B;**選項**&#x200B;區段中，選取您要從範本中清除之任何資訊旁的核取方塊。

   ![](assets/save-as-template-options-step-350x109.png)

1. 按一下&#x200B;**下一步。**
1. 在&#x200B;**排除**&#x200B;區段中，選取您要從專案排除的任何工作。

   ![](assets/save-as-template-exclude-350x205.png)

1. 按一下&#x200B;**完成並儲存範本。**

   您的範本現在會顯示在可用範本清單中，並可附加至現有專案或用來建立新專案。
