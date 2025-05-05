---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 建立自訂費用型別
description: 作為 [!DNL Adobe Workfront] 管理員，您可以建立自訂費用型別，以定義及追蹤與您的任務和專案相關的費用。 費用是可與任務或專案相關聯的非人工成本。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 428e6a9365c793ce5944941ec5368a674c208c78
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 4%

---

# 建立自訂費用類型

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作為[!DNL Adobe Workfront]管理員，您可以建立自訂費用型別以定義及追蹤與您的任務和專案相關的費用。 費用是可與任務或專案相關聯的非人工成本。

您可以編輯或刪除您建立的任何費用型別。 您無法刪除或編輯內建[!DNL Workfront]費用型別。

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
   <td><p>新增：[!UICONTROL Standard]</p>
   或
   <p>目前： [!UICONTROL 計畫]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td>
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 預設費用型別

[!DNL Workfront]中無法刪除或編輯的預設費用型別包括下列專案：

* [!UICONTROL Advertising]
* [!UICONTROL 諮詢]
* [!UICONTROL 娛樂]
* [!UICONTROL 一般]
* [!UICONTROL 材料]
* [!UICONTROL 旅遊]

## 建立自訂費用類型

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 費用型別]**。
1. 按一下&#x200B;**[!UICONTROL 新增費用型別]**。
1. 在&#x200B;**[!UICONTROL 新費用型別]**&#x200B;對話方塊中，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名稱]</td> 
      <td>指定費用的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 說明]</td> 
      <td>指定費用的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 計算單位]</td> 
      <td> <p>從下拉式清單中選取您費用型別的測量單位。</p> <p>可用的測量單位如下：</p> 
       <ul> 
        <li>英里</li> 
        <li>公里</li> 
        <li>公斤</li> 
        <li>元</li> 
        <li>元</li> 
        <li>日</li> 
        <li>其他 — 選取此選項會提示您為度量單位命名，並將度量單位定義為組織所熟悉的單位。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費率</td> 
      <td> <p>指定單價。 這是貨幣格式欄位，它代表在<strong>[!UICONTROL 計算單位]</strong>欄位中建立的每個單位的成本。 </p> <p>速率可包含小數點後最多4個數字的數值。 例如：1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**[!UICONTROL 儲存]**」。

   使用者現在可以使用此費用型別，將其與其在專案和任務上的費用建立關聯。

## 修改自訂費用型別

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 費用型別]**。
1. 選取您要修改的費用型別，然後按一下[編輯]。**&#x200B;**

   **[!UICONTROL 編輯費用型別]**&#x200B;對話方塊就會顯示。

1. 進行您想要的變更，然後按一下[儲存]。**&#x200B;**

   使用者現在可以使用此費用型別，將其與其在專案和任務上的費用建立關聯。

如需有關如何使用費用以及這些費用如何影響專案成本的詳細資訊，請參閱文章[管理專案費用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。
