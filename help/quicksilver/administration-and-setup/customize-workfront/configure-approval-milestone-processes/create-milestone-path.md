---
title: 建立里程碑路徑
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 身為Adobe Workfront管理員，您可以建立里程碑路徑，然後將其套用至系統中的任何專案。 您在此區域對里程碑路徑所做的變更會影響整個Workfront系統。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 2%

---

# 建立里程碑路徑

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

身為Adobe Workfront管理員，您可以建立里程碑路徑，然後將其套用至系統中的任何專案。 您在此區域對里程碑路徑所做的變更會影響整個Workfront系統。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 里程碑和里程碑路徑

您可以將專案中的主要任務與預先定義的里程碑建立關聯。 這一職能可為管理人員和其他利益攸關方提供關於項目進展情況的高級別概覽。

所有預先定義里程碑的總和稱為里程碑路徑。

建立里程碑路徑的第一步是識別里程碑步驟是什麼並建立里程碑。 因為您可以將里程碑路徑關聯到多個項目，因此里程碑步驟必須是任何項目的一般階段或階段。

有關如何將里程碑路徑與項目關聯以及如何將里程碑與任務關聯的詳細資訊，請參閱 [將里程碑與任務關聯](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## 建立里程碑路徑

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **程式** > **里程碑路徑**.
1. 按一下 **新里程碑路徑。**
1. 在 **基本資訊** 區域：

   <table style="table-layout:auto">
    <tr>
      <td>里程碑路徑名稱</td>
       <td>輸入裡程碑路徑的名稱。</td>
    </tr>
    <tr>
      <td>說明</td>
      <td>輸入說明以定義里程碑路徑。</td>
    </tr>
    <tr>
       <td>活動</td>
      <td>如果希望里程碑路徑處於活動狀態，請選中此複選框。 其他使用者在建立或編輯專案時，可以找到此路徑並將其附加至專案。 非活動的里程碑路徑無法附加至專案。 預設會啟用。</td>
    </tr>
    <tr>
      <td>群組</td>
      <td>選取列出的群組，以允許這些群組中的使用者查看此里程碑路徑，並將此里程碑路徑套用至其專案。 預設會選取進入裡程碑路徑之使用者的首頁群組。</td>
    </tr>
   </table>

1. 在 **里程碑** 區域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td>為每個里程碑輸入描述性名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入裡程碑的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">顏色</td> 
      <td> <p>選擇要與里程碑關聯的顏色。 </p> <p>如果不選擇顏色，系統將選擇里程碑路徑中使用的最後一種顏色。 建議您為每個里程碑選擇唯一的顏色。 顏色用於視覺化和報告用途。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **添加里程碑** 並繼續視需要新增里程碑，直到路徑完成為止。
1. 按一下 **建立里程碑路徑** 來儲存變更。

   您的里程碑路徑已準備好與專案相關聯。

   如需如何將里程碑路徑與專案和里程碑與工作建立關聯的詳細資訊，請參閱 [將里程碑與任務關聯](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
