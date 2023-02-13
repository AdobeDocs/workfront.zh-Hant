---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''篩選：通過比較兩個欄位來消除清單中的項'
description: 您可以比較項目的兩個欄位，從清單中篩選項目。 例如，您只能顯示任務的實際完成日期大於計畫完成日期的任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 篩選：比較兩個欄位以消除清單中的項目

您可以比較項目的兩個欄位，從清單中篩選項目。 例如，您只能顯示任務的實際完成日期大於計畫完成日期的任務。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 比較兩個欄位以篩選項目

1. 轉到任務清單。
1. 從 **篩選** 下拉式功能表，選取 **新增篩選**.

1. 按一下 **新增篩選規則** 新增 **實際完成日期** >**大於** > **選擇日期**.

   >[!TIP]
   >
   >選擇要用於選定欄位的篩選修改量（如果可用）。

1. 按一下 **切換到文本模式**.
1. 在 **設定報表的篩選規則** 區域，新增下列程式碼：

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. 按一下 **完成**，然後 **儲存篩選**.
