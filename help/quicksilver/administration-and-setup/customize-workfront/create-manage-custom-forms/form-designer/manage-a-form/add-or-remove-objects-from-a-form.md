---
title: 使用表單設計工具從現有自訂表單新增或刪除物件型別
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表單設計工具，在自訂表單中新增或移除物件型別。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# 使用表單設計工具從現有自訂表單新增或刪除物件型別

您可以使用表單設計工具，在現有自訂表單中新增或刪除物件型別。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td><p>管理自訂表單的存取權</p></td> 
  </tr>  
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 將物件型別新增至現有的自訂表單

您可以將其他物件型別新增至表單，使其可附加至多個物件。

>[!NOTE]
>
>分割槽符號許可權會受到物件型別的影響。 自訂表單分割槽符號的「有限編輯」許可權僅適用於專案、任務、問題和使用者物件型別。
>
>如需詳細資訊，請參閱[多個物件型別如何影響分割槽符號許可權](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions)。


{{step-1-to-setup}}

1. 按一下左側面板中的&#x200B;**自訂Forms**。

   在出現的檢視中，您可以檢閱為組織建立的所有自訂表單。 您也可以檢視每個表單的建立者、表單使用的物件型別，以及表單是否使用中。

1. 選取要新增其他物件型別的自訂表單，然後按一下![編輯圖示](assets/edit-icon2.png)。

1. 在表單頂端按一下&#x200B;**物件型別**&#x200B;之後的加號+，然後在顯示的功能表中選取您要的型別。 您可以重複此步驟，新增任意數目的物件型別。

   ![](assets/add-new-object.png)

1. 按一下&#x200B;**儲存並關閉**。

   >[!TIP]
   >
   >建立自訂表單時，您可以隨時按一下&#x200B;**套用**，以儲存變更並保持表單開啟。

## 刪除自訂表單上的物件型別

您可以從現有的自訂表單中刪除物件型別。 自訂表單必須至少有一個物件型別。

>[!CAUTION]
>
>如果人員已將自訂表單附加到您要刪除的物件型別並新增資料，當您刪除表單上的該物件型別時，該資料將會永久刪除。 其中可能包含使用者稍後所需的歷史資訊。
>
>一般而言，建議您儘可能減少編輯已使用中的自訂表單的次數。 沒有通知系統可提醒使用自訂表單的人員您的變更。

若要刪除物件型別，請執行下列動作：

{{step-1-to-setup}}

1. 按一下左側面板中的&#x200B;**自訂Forms**。
1. 選取您要編輯的自訂表單，然後按一下![編輯圖示](assets/edit-icon2.png)。
1. 在您要從表單刪除的任何&#x200B;**物件型別**&#x200B;上按一下X。

   ![](assets/delete-object-types.png)

1. （可選）針對您要從表單中移除的任何其他物件型別，重複上一步驟。
1. 按一下&#x200B;**套用**，然後按一下&#x200B;**儲存並關閉**。
