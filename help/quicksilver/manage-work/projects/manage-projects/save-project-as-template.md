---
product-area: projects;templates
navigation-topic: manage-projects
title: 將專案另存為範本
description: 在專案層級將專案儲存為templateSave as template （範本），讓使用者在UI中看到；此連結的另一篇文章有更深入的連結（逐步進行）。
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# 將專案另存為範本

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<!--
<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>
-->

如果您決定某個專案將在未來再次發生，則可以從現有專案建立範本。 然後，您可以再次使用範本來建立未來專案，這些專案可能包含類似的資訊，或與現有專案共用相同的時間表或工作分派。

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
   <td> <p>標準</p>
   <p>規劃</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯範本的存取權</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或更高的許可權 </p> <p>將專案另存為範本後，即可取得範本的管理許可權</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard </p>
   Or 
   <p>Current: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> /td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 將專案另存為範本

<!--
Saving a project as a template differs in the Production and the Preview environments. 

### Save a project as a template in the Production environment


1. Go to the project that you want to save as a template. 
1. Click the **More** menu ![More icon](assets/more-icon.png), then **Save as Template**. 
1. Specify the following information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Provide a description for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is Active</td> 
      <td> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Yes</strong>: Other users can find the template and attach it to projects.</p> </li> 
        <li><strong>No</strong>: Other users cannot find the template and cannot attach it to projects.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td>Use the drop-down list to select any custom forms to attach to the template. If any custom forms have already been associated with the project, all of the data fields from those custom forms are displayed.<br>You can include up to 10 custom forms on a single template.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Manage Forms** to remove or reorder the forms. For information about how to remove and reorder custom forms on the template, see [Custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Click **Next Step.**
1. In the **Options** section, select the checkbox beside any information you want to clear from the template.

   ![](assets/save-as-template-options-step-350x109.png)

1. Click **Next Step.**
1. In the **Exclude** section, select any tasks that you want to exclude from the project.

   ![](assets/save-as-template-exclude-350x205.png)

1. Click **Finish and Save Template.**

   Your template now appears in the list of available templates and can either be attached to an existing project or used to create a new one.


<div class="preview">

### Save a project as a template in the Preview environment

-->

1. 前往您要另存為範本的專案。
1. 按一下&#x200B;**更多**&#x200B;功能表![更多圖示](assets/qs-more-icon-on-an-object.png)，然後&#x200B;**另存為範本**。
1. 在&#x200B;**另存為範本**&#x200B;區段中，指定範本的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">範本名稱</td> 
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

1. 按一下左側面板中的「自訂Forms」****，移除或重新排序表單。

   若要重新排序表單，請以正確順序拖放表單。
若要移除表單，請選取該表單，然後按一下[移除]。**** 按一下&#x200B;**取消**&#x200B;以移除選取的表單。

   ![儲存為範本方塊中的自訂表單區域](assets/custom-forms-ara-in-save-as-template-box.png)

1. 如有需要，請更新附加自訂表單中的資訊。 資訊將會傳輸至範本。

1. 按一下左側面板中的&#x200B;**選項**，然後選取您要傳送至範本的任何資訊旁的核取方塊。 取消選取的專案不會轉移到範本。 預設會取消選取所有選項。

   另存為範本方塊中的![選項區域](assets/options-area-in-save-as-template-box.png)

1. 按一下左側面板中的「排除&#x200B;****」，然後選取您要從專案排除的任何工作。 預設會取消選取所有工作。

   ![另存為範本方塊中的排除區域](assets/exclude-area-save-as-template-box.png)

1. 按一下畫面右上角的&#x200B;**完成並儲存範本**。

   您的範本現在會顯示在可用範本清單中，並可附加至現有專案或用來建立新專案。

