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
source-git-commit: 7c39f54677be746ce6305124026df7df598b3da2
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 3%

---

# 編輯和建立風險類型

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Adobe Workfront有許多預設風險型別，您可以在計畫階段與專案建立關聯，以在核准任何工作之前識別潛在障礙。

風險是可能導致專案無法按時完成或無法在預算內完成的事件。

除了預設風險型別之外，您還可以新增風險型別以反映組織中的需求。

您可以將風險型別與專案風險建立關聯，以識別專案可能遇到的風險型別。

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

風險型別是可用於風險的標籤，可將其分類以用於報表用途。

作為[!DNL Workfront]管理員，您可以在&#x200B;[!UICONTROL **設定**]&#x200B;區域中建立[!UICONTROL 風險型別]。

設定風險型別後，這些風險型別對您的系統通用。

所有專案擁有者都可針對其專案使用相同的風險型別。

## 編輯和建立風險類型

某些風險型別預設已在[!DNL Workfront]中。


您可以執行下列操作來增加Workfront執行個體中的風險型別數量：

* [編輯現有的風險型別](#edit-existing-risk-types)
* [建立風險型別](#create-risk-types)

### 編輯現有的風險型別 {#edit-existing-risk-types}

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 風險型別]**。
1. 選取您要編輯的風險型別。
1. 按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

   [!UICONTROL **編輯風險型別**]&#x200B;方塊開啟。<!--add screen shot-->

   >[!TIP]
   >
   >   當您連按兩下清單中風險型別的「名稱」或「說明」時，可以內嵌編輯風險型別資訊。

1. （選擇性）變更風險型別的名稱和說明。


   **[!UICONTROL Name]**&#x200B;和&#x200B;**[!UICONTROL Description]**&#x200B;欄位有50個字元的字元限制。

1. 按一下&#x200B;**[!UICONTROL 儲存變更]。**

1. （選擇性）若要刪除風險型別，請在清單中選取它，然後按一下&#x200B;[!UICONTROL **刪除**]&#x200B;圖示![刪除圖示](assets/delete.png)，然後按一下&#x200B;[!UICONTROL **是，刪除**]。 風險型別已刪除，且無法復原。

1. （選擇性）若要匯出風險型別清單，請按一下&#x200B;[!UICONTROL **匯出**]&#x200B;圖示![匯出圖示](assets/export-icon.png)。 您可以匯出為下列檔案型別：

   * PDF
   * Excel
   * Excel (xlsx)
   * 頁籤分隔檔

   >[!TIP]
   >
   >   您可以先選取有限數量的風險型別，然後將其匯出以取得較小的清單。


### 建立風險型別 {#create-risk-types}

除了預設風險型別外，您還可以建立風險型別。

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 風險型別]**。
1. 按一下&#x200B;**[!UICONTROL 新增風險型別]**&#x200B;以開啟&#x200B;[!UICONTROL **新增風險型別**]&#x200B;方塊

   或

   按一下風險型別清單左下角的&#x200B;[!UICONTROL **新增更多風險型別**]，以內嵌新增風險型別。<!--add screen shot-->
1. 輸入風險型別的&#x200B;**[!UICONTROL Name]** （必要）和&#x200B;**[!UICONTROL Description]** （選用）。

   **[!UICONTROL Name]**&#x200B;和&#x200B;**[!UICONTROL Description]**&#x200B;欄位有50個字元的字元限制。

1. 按一下&#x200B;**[!UICONTROL 建立風險型別]**，

   或者，如果您使用內嵌編輯來新增風險型別，請在完成時按一下&#x200B;**[!UICONTROL Enter]**。

   >[!TIP]
   >
   >若要編輯自訂風險型別，請參閱本文章的[[!UICONTROL 編輯現有]風險型別](#edit-existing-risk-types)小節。

## 在專案上附加風險與風險型別

您可以使用風險型別來標示新增至專案的風險。

如需如何新增風險至專案的詳細資訊，請參閱[在專案上建立與編輯風險](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)。
