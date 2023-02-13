---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 建立自定義支出類型
description: 作為 [!DNL Adobe Workfront] 管理員，您可以建立自定義費用類型，以定義和跟蹤與任務和項目關聯的費用。 費用是可與任務或項目關聯的非人工成本。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 3%

---

# 建立自定義支出類型

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作為 [!DNL Adobe Workfront] 管理員，您可以建立自定義費用類型，以定義和跟蹤與任務和項目關聯的費用。 費用是可與任務或項目關聯的非人工成本。

您可以編輯或刪除您建立的任何費用類型。 您無法刪除或編輯內建 [!DNL Workfront] 費用類型。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 預設費用類型

中的費用類型 [!DNL Workfront] 預設情況下，無法刪除或編輯以下內容：

* [!UICONTROL 廣告]
* [!UICONTROL 諮詢]
* [!UICONTROL 娛樂]
* [!UICONTROL 一般]
* [!UICONTROL 材料]
* [!UICONTROL 差旅]

## 建立自定義支出類型

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront].
1. 按一下 **[!UICONTROL 費用類型]**.
1. 按一下 **[!UICONTROL 新費用類型]**.
1. 在 **[!UICONTROL 新費用類型]** 框中，指定以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td>指定費用的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>指定費用的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL計算單元]</td> 
      <td> <p>從下拉清單中選擇費用類型的度量單位。</p> <p>可使用下列測量單位：</p> 
       <ul> 
        <li>英里</li> 
        <li>公里</li> 
        <li>公斤</li> 
        <li>元</li> 
        <li>元</li> 
        <li>日</li> 
        <li>其他 — 選擇此選項將提示您為測量單位命名，並將測量單位定義為組織熟悉的單位。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯率</td> 
      <td> <p>指定每件的價格。 這是貨幣格式欄位，它表示在 <strong>[!UICONTROL計算單元]</strong> 欄位。 </p> <p>比率可包含一個數值，小數後最多有4個數字。 例如1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 建立費用類型]**.\
   費用類型現在可供用戶將其與其項目和任務費用關聯。

## 修改自定義費用類型

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront].
1. 按一下 **[!UICONTROL 費用類型]**.
1. 選擇要修改的費用類型，然後按一下 **[!UICONTROL 編輯]**.

   此 **[!UICONTROL 編輯費用類型]** 對話框。

1. 進行所需的變更，然後按一下 **[!UICONTROL 儲存變更]**.\
   費用類型現在可供用戶將其與其項目和任務費用關聯。

有關如何使用費用以及如何影響項目成本的詳細資訊，請參閱文章 [管理項目費用](../../../manage-work/projects/project-finances/manage-project-expenses.md).
