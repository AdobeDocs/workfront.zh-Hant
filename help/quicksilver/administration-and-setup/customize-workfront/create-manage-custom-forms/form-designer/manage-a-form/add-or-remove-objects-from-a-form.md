---
title: 使用表單設計器從現有自定義表單中添加或刪除對象類型
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表單設計工具從自訂表單中新增或移除物件類型。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: c0082dd73e3db8123f9cc08f1798ef8e70730625
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---


# 使用表單設計器從現有自定義表單中添加或刪除對象類型

{{highlighted-preview-article-level}}

您可以使用表單設計工具從現有自訂表單中新增或刪除物件類型。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>
   <p>當前計畫：標準</p>
   <p>或</p>
   <p>舊計畫：計畫</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td><p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 將物件類型新增至現有的自訂表單

您可以將其他對象類型添加到窗體中，以便可以將其附加到多個對象。

>[!NOTE]
>
>區段劃分權限可能受對象類型影響。 自訂表單區段分段的「有限編輯」權限僅適用於「專案」、「任務」、「問題」和「使用者」物件類型。
>
>如需詳細資訊，請參閱 [多種對象類型如何影響分節符權限](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms** 中。

   在顯示的檢視中，您可以檢閱為貴組織建立的所有自訂表單。 您也可以查看每個表單的建立者、其適用的物件類型，以及其是否使用中。

1. 選擇要添加其他對象類型的自定義表單，然後按一下 **編輯**.

1. 在表單頂端按一下加號+之後 **物件類型**，然後在顯示的功能表中選取您要的類型。 您可以重複此操作，以新增任意數量的物件類型。

   ![](assets/add-new-object.png)

1. 按一下 **儲存並關閉**.

   >[!TIP]
   >
   >您可以按一下 **套用** 在您建立自訂表單時隨時儲存變更並保持表單開啟。

## 刪除自訂表單上的物件類型

您可以從現有的自訂表單中刪除物件類型。 自訂表單至少必須有一個物件類型。

>[!CAUTION]
>
>如果已將自定義表單附加到您要刪除的類型的對象中，並將資料添加到該對象中，則在您刪除表單上的該對象類型時，該資料將被永久刪除。 其中可能包含使用者日後需要的歷史資訊。
>
>一般而言，建議您將編輯已使用中自訂表單的次數減到最少。 沒有通知系統可提醒使用自訂表單的使用者您所做的變更。

要刪除對象類型：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms** 中。
1. 選取您要編輯的自訂表單，然後按一下 **編輯**.
1. 按一下 **物件類型** 從表單中刪除，然後按一下 **刪除** 顯示的警告訊息。

   ![](assets/delete-object-types.png)

1. （可選）對要從表單中刪除的任何其他對象類型重複上一步。
1. 按一下 **完成**，然後按一下 **關閉並儲存**.
