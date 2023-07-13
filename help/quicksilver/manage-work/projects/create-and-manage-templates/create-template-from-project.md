---
product-area: templates
navigation-topic: templates-navigation-topic
title: 從專案建立範本
description: 將現有專案另存為範本時，可以建立範本。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# 從專案建立範本

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

將現有專案另存為範本時，可以建立範本。

將現有專案另存為範本後，您可以使用新範本建立新專案。 這簡化並加速了專案建立流程。

>[!NOTE]
>
>將專案儲存為範本時，未儲存範本的任務和專案的實際日期。
>
>範本及其任務沒有實際日期，而是指出任務可能從哪一天開始（從未來專案可能開始）以及任務可能需要在哪一天完成。 使用範本建立未來的專案時，專案將收到實際日期。 如需詳細資訊，請參閱 [建立專案](../create-projects/create-project.md).

## 存取需求

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
   <td> <p>編輯範本的存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或更高許可權 </p> <p>建立範本後，您便可獲得範本的管理許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 從專案建立範本

1. 前往您要另存為範本的專案。
1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png)，則 **另存為範本**.
1. 為範本指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td>指定範本的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>提供範本的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">為使用中</td> 
      <td> <p>從下列選項中選取：</p> 
       <ul> 
        <li> <p><strong>是</strong>：其他使用者可以找到範本並將其附加至專案。</p> </li> 
        <li><strong>否</strong>：其他使用者找不到範本且無法將其附加至專案。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂表單</td> 
      <td>使用下拉式清單來選取要附加至範本的任何自訂表單。 如果有任何自訂表單已與專案相關聯，則會顯示這些自訂表單中的所有資料欄位。<br>您可以在單一範本上包含最多10個自訂表單。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **管理Forms** 以移除或重新排序表單。 如需如何在範本上移除和重新排序自訂表單的相關資訊，請參閱 [自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. 按一下 **下一步。**
1. 在&#x200B;**選項** 區段中，選取您要從範本中清除之任何資訊旁邊的核取方塊。

   ![](assets/save-as-template-options-step-350x109.png)

1. 按一下 **下一步。**
1. 在 **排除** 區段，選取您要從專案排除的任何任務。

   ![](assets/save-as-template-exclude-350x205.png)

1. 按一下 **完成並儲存範本。**

   您的範本現在會顯示在可用範本清單中，並可附加至現有專案或用來建立新專案。

 
