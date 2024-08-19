---
title: 建立里程碑路徑
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 身為Adobe Workfront管理員，您可以建立里程碑路徑，然後將其套用至系統中的任何專案。 您在此區域中對里程碑路徑所做的變更會影響整個Workfront系統。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 3%

---

# 建立里程碑路徑

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

身為Adobe Workfront管理員，您可以建立里程碑路徑，然後將其套用至系統中的任何專案。 您在此區域中對里程碑路徑所做的變更會影響整個Workfront系統。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 里程碑和里程碑路徑

您可以將專案中的關鍵任務與預先定義的里程碑建立關聯。 此函式可為經理和其他利害關係人提供專案進展方式的高層級概觀。

所有預先定義的里程碑的總和稱為里程碑路徑。

建立里程碑路徑的第一步是識別里程碑步驟是什麼，並建立里程碑。 由於您可以將里程碑路徑關聯到多個專案，因此里程碑步驟必須是任何專案的一般階段或階段。

如需如何關聯里程碑路徑與專案的詳細資訊，以及關聯里程碑與任務的詳細資訊，請參閱[關聯里程碑與任務](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)。

## 建立里程碑路徑

{{step-1-to-setup}}

1. 按一下&#x200B;**處理序** > **里程碑路徑**。
1. 按一下&#x200B;**新增里程碑路徑。**
1. 在&#x200B;**基本資訊**&#x200B;區域中指定下列資訊：

   <table style="table-layout:auto">
    <tr>
      <td>里程碑路徑名稱</td>
       <td>輸入里程碑路徑的名稱。</td>
    </tr>
    <tr>
      <td>說明</td>
      <td>輸入描述以定義里程碑路徑。</td>
    </tr>
    <tr>
       <td>為作用中</td>
      <td>如果您希望里程碑路徑為作用中路徑，請選取此核取方塊。 其他使用者可在建立或編輯專案時找到此路徑並將其附加至專案。 非使用中的里程碑路徑無法附加到專案。 這預設為啟用。</td>
    </tr>
    <tr>
      <td>群組</td>
      <td>選取列出的群組，以允許這些群組中的使用者檢視此里程碑路徑並將其套用至他們的專案。 依照預設，會選取進入里程碑路徑的使用者主群組。</td>
    </tr>
   </table>

1. 在&#x200B;**里程碑**&#x200B;區域中指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td>輸入每個里程碑的描述性名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入里程碑的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">顏色</td> 
      <td> <p>選擇要與里程碑關聯的顏色。 </p> <p>如果不選擇顏色，系統會選擇里程碑路徑中使用的最後一個顏色。 建議您為每個里程碑選擇唯一的顏色。 該顏色用於視覺效果和報表用途。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**新增里程碑**，然後視需要繼續新增里程碑，直到路徑完成為止。
1. 按一下&#x200B;**建立里程碑路徑**&#x200B;以儲存變更。

   您的里程碑路徑已準備好與專案相關聯。

   如需有關如何將里程碑路徑與專案建立關聯以及將里程碑與任務建立關聯的詳細資訊，請參閱[將里程碑與任務建立關聯](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)。
