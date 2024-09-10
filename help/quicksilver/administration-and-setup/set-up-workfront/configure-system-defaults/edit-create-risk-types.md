---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 編輯與建立風險型別
description: 您可以在計畫階段為專案新增風險，以在核准任何工作之前識別潛在障礙。 風險是可能導致專案無法按時完成或無法在預算內完成的事件。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 2%

---

# 編輯和建立風險類型

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

您可以在計畫階段為專案新增風險，以在核准任何工作之前識別潛在障礙。 風險是可能導致專案無法按時完成或無法在預算內完成的事件。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新增：[！UICONTROL Standard]</p>
   或
   <p>目前： [！UICONTROL計畫]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 風險型別

風險型別是可用於風險的標籤，可將其分類以用於報表用途。 它們由[!DNL Adobe Workfront]管理員在&#x200B;**[!UICONTROL 設定]**&#x200B;區域中建立。 在您的&#x200B;**[!UICONTROL 設定]**&#x200B;區域中建立風險型別後，這些風險型別對您的系統而言是通用的。 所有專案擁有者都可針對其專案使用相同的風險型別。

## 編輯和建立風險類型

某些風險型別預設已在[!DNL Workfront]中。 若要反映貴組織的需求，您可以編輯現有的風險型別，或建立新的風險型別。

* [編輯現有的風險型別](#edit-existing-risk-types)
* [建立新的風險型別](#create-new-risk-types)

### 編輯現有的風險型別 {#edit-existing-risk-types}

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 風險型別]**。
1. 選取您要編輯的風險型別。
1. 按一下&#x200B;**[!UICONTROL 編輯]**。
1. （選擇性）變更風險型別的名稱和說明。

   **[!UICONTROL Name]**&#x200B;和&#x200B;**[!UICONTROL Description]**&#x200B;欄位有50個字元的字元限制。

1. 按一下&#x200B;**[!UICONTROL 儲存變更]。**

### 建立新的風險型別 {#create-new-risk-types}

除了預設風險型別外，您還可以建立新的風險型別以反映組織的需求。

若要建立新的風險型別，請執行下列步驟：

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 風險型別]**。
1. 按一下&#x200B;**[!UICONTROL 新增風險型別]**。
1. 輸入風險型別的&#x200B;**[!UICONTROL Name]** （必要）和&#x200B;**[!UICONTROL Description]** （選用）。

   **[!UICONTROL Name]**&#x200B;和&#x200B;**[!UICONTROL Description]**&#x200B;欄位有50個字元的字元限制。

1. 按一下&#x200B;**[!UICONTROL 建立風險型別]**。 如果您使用內嵌編輯來新增您的風險型別，請在完成時按一下&#x200B;**[!UICONTROL Enter]**。

   >[!NOTE]
   >
   >如果您需要編輯自訂風險型別，請參閱本文章的[[!UICONTROL 編輯現有]風險型別](#edit-existing-risk-types)小節。

## 在專案上附加風險與風險型別

風險型別可用於標示新增至專案的風險。 如需如何新增風險至專案的詳細資訊，請參閱[在專案上建立與編輯風險](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)。
