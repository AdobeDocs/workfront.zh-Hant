---
product-area: projects
navigation-topic: manage-projects
title: 複製專案
description: 您可以複製專案，而非從頭建立專案。 一次只能複製一個專案。 您無法大量複製專案。
author: Alina
feature: Work Management
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 5e0e1425f45886a805726de49357c43b0aecb7f4
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 5%

---

# 複製專案

<!--some areas are drafted for the 23.2 release story-->

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

您可以複製專案，而非從頭建立專案。 一次只能複製一個專案。 您無法大量複製專案。

>[!IMPORTANT]
>
>不會將下列項目從現有項目複製到新項目：
>
>* 問題
>* 收費率
>* 付費記錄
>* 附註
>* 時數
>* 跨專案的前置作業
>* 預算時數 <!-- drafted for release 23.2: take this out and move it to the one below IF there is no UI component for the story that allows you to check/uncheck this information as you copy the project. If there is a UI component, take this out of here and just add it to the new screen shot below. -->
>
>下列項目一律會從現有專案複製到新專案：
>
>* 任務
>* 範本
>* 風險
>* 隊列設定資訊
>* Portfolio與方案
>* 計分卡
>* 任務預設資訊(任務預設審批流程、任務預設自定義Forms)
>


## 存取需求

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront授權*</p> </td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>編輯專案的存取權並建立 <span>和複製</span> 專案</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>檢視專案的權限或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 複製單一專案

複製專案也會將一些資訊從原始專案複製到新專案。 您也可以指定在複製過程中不應將哪些項目複製到新專案。

若要複製專案：

1. 前往您要複製的專案，然後按一下 **更多** 圖示 ![](assets/qs-more-menu.png) 項目名稱的右側

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   前往專案清單或報表，然後選取專案，然後按一下 **更多** 圖示 ![](assets/qs-more-menu.png) 清單頂端。

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. 按一下 **複製**.

1. 更新新專案的名稱。

   依預設，新名稱為 **副本 `<Original project name>`.**

   ![](assets/copy-project-box-nwe-350x276.png)

1. 選取 **狀態** 新專案。

   依預設， **狀態** 與原始專案的相符項目。

1. （選用）取消選取您不要複製到新專案的項目。 下表說明取消選取項目時會發生什麼事：

   <!--drafted for story for the 23.2 release: add another line in the table below for "Budgeted hours" and add this information to that row:
      Removes the hours budgeted in the Resource Planning area of the project's Business Case from the copied project. 
      <b>NOTE</b>
      Hours budgeted using the Scenario Planner are never copied to the new project because the new project is not linked to an initiative in the Scenario Planner. For more information, see <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Budget resources in the Business Case using the Scenario Planner</a>
      -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全選</td> 
      <td> <p>選取所有選項，並清除新專案中列出的所有欄位和物件。</p> <p><b>筆尖</b>

   取消選取 <strong>全選</strong> 取消選取所有項目。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">指派</td> 
      <td>刪除所有項目和任務分配</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進度</td> 
      <td>刪除所有任務的進度，並將其顯示為「新建」。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂資料</td> 
      <td> <p>從專案的自訂表單中移除資訊，以及與下列項目相關聯的自訂表單資訊：</p> 
       <ul> 
        <li>任務</li> 
        <li>費用</li> 
        <li> 文件</li> 
       </ul> <p><b>附註</b>

   自訂表單仍會附加至工作、費用、檔案和專案，但表單的自訂欄位中的資訊不會複製到新專案。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">文件</td> 
      <td> <p>刪除文檔頁簽中的所有內容，包括文檔版本、連結的文檔和資料夾。</p> <p>預設情況下，文檔校樣和批准不能複製到另一個項目。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任務</td> 
      <td> <p>刪除項目上任務之間的所有前置任務關係。 </p> <p>提示：跨項目前置任務不會轉移到新項目，無論是否選擇了此項目。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">財務資訊</td> 
      <td> <p>移除下列區域中的資訊： </p> 
       <ul> 
        <li>項目的財務子頁簽</li> 
        <li> 業務案例中的計畫利益</li> 
        <li>所有任務的財務資訊<br></li> 
       </ul> <p>有關項目「財務」子頁簽的詳細資訊，請參見 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">管理項目財務區域中的資訊</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准流程</td> 
      <td>刪除與任務或項目關聯的所有批准。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td> 刪除與任務或項目關聯的提醒通知。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>刪除與任務或項目相關的費用。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">權限</td> 
      <td> 移除任務或專案上所有使用者的權限。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **複製** 來建立專案副本。

   這會建立與您複製的專案類似的新專案。

   您可以開始對新複製的項目進行更改，如審閱任務分配或調整時間軸。
