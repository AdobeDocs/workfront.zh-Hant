---
product-area: templates
navigation-topic: templates-navigation-topic
title: 從專案建立範本
description: 從專案建立範本
author: Alina
feature: Work Management
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 2%

---

# 從專案建立範本

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

將現有專案儲存為範本時，可以建立範本。

將現有專案儲存為範本後，即可使用新範本建立新專案。 這可簡化並加速專案建立程式。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯範本的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案的或更高權限 </p> <p>建立範本後，您就可取得範本的「管理」權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 從專案建立範本

1. 前往您要儲存為範本的專案。
1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png)，然後 **另存為範本**.
1. 指定範本的下列資訊：

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
      <td role="rowheader">活動</td> 
      <td> <p>從下列選項中選取：</p> 
       <ul> 
        <li> <p><strong>是</strong>:其他使用者可以找到範本並附加至專案。</p> </li> 
        <li><strong>否</strong>:其他使用者找不到範本，且無法將其附加至專案。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂表單</td> 
      <td>使用下拉式清單來選取要附加至範本的任何自訂表單。 如果任何自訂表單已與專案相關聯，則會顯示這些自訂表單的所有資料欄位。<br>在單一範本中，最多可包含10個自訂表單。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **管理Forms** 移除或重新排序表單。 如需如何移除和重新排序範本上自訂表單的詳細資訊，請參閱 [自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. 按一下 **下一步。**
1. 在&#x200B;**選項** 區段中，選取您要從範本中清除之任何資訊旁的核取方塊。

   ![](assets/save-as-template-options-step-350x109.png)

1. 按一下 **下一步。**
1. 在 **排除** 區，選擇要從項目中排除的任務。

   ![](assets/save-as-template-exclude-350x205.png)

1. 按一下 **完成並保存模板。**

   您的範本現在會顯示在可用範本清單中，且可附加至現有專案或用來建立新專案。

 
