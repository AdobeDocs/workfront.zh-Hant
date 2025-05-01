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
source-git-commit: 6e2e337969fccba88ea7089fe9a6d9db605343f7
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 3%

---

# 建立里程碑路徑

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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
   <td>規劃</td> 
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


1. （選擇性）按一下&#x200B;**匯出**&#x200B;圖示![匯出圖示](assets/export-icon.png)，然後從下列格式中選取，以將里程碑路徑清單匯出至檔案：

   * PDF
   * Excel
   * Excel (xlsx)
   * 頁籤分隔檔

1. （選擇性）選取里程碑清單中的里程碑，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)以編輯里程碑資訊。
1. （選擇性）選取里程碑清單中的里程碑，然後按一下&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete-icon.png)以刪除它。
1. 按一下&#x200B;**是，刪除**。
里程碑已刪除且無法復原。 與里程碑關聯的任何專案資訊以及與里程碑路徑關聯的任何任務資訊也會被刪除。


## 在專案報告中檢視里程碑路徑詳細資訊

您可以在專案報告中檢視里程碑路徑的詳細資訊。

您必須先將里程碑路徑與專案建立關聯，才能在專案報告中檢視其詳細資訊。

如需有關將里程碑路徑關聯至專案的資訊，請參閱[編輯專案](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)。

{{step1-to-reports}}

1. 按一下&#x200B;**新報告**，然後按一下&#x200B;**專案**。
1. 按一下「**新增欄**」。
1. 在&#x200B;**顯示在此欄**&#x200B;區域中，開始輸入&#x200B;**里程碑路徑**，然後在顯示時按一下&#x200B;**里程碑路徑名稱**。
1. （選用）按一下&#x200B;**篩選器**，並將下列篩選器新增至報表： **專案里程碑路徑ID不是空白的**。

   此篩選器可確保您只顯示與報告中里程碑路徑相關聯的專案。

1. 按一下「**儲存並關閉**」。
1. 新增報表名稱，然後按一下[套用]。****

   專案報告隨即顯示。 與每個專案相關聯的里程碑路徑會顯示在報表的最後一欄。
1. 按一下報告最後一欄中的里程碑路徑名稱。

   里程碑路徑的詳細資訊隨即顯示。

   ![專案報告的里程碑路徑詳細資料](assets/milestone-details-from-project-report.png)

   里程碑路徑詳細資訊頁面會顯示下列資訊：

   * 里程碑路徑名稱、ID和說明
   * 里程碑路徑群組
   * 里程碑名稱、說明、顏色和顏色圖示

1. （選擇性）按一下&#x200B;**上一步**&#x200B;返回專案報告。



