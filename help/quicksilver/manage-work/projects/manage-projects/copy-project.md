---
product-area: projects
navigation-topic: manage-projects
title: 複製專案
description: 您可以複製專案，而不用從頭開始建立。 您一次只能複製一個專案。 您無法大量複製專案。
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 4%

---

# 複製專案

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

您可以複製專案，而不用從頭開始建立。 您一次只能複製一個專案。 您無法大量複製專案。

>[!IMPORTANT]
>
>下列專案絕不會從現有專案複製到新專案：
>
>* 問題
>* 收費率
>* 付費記錄
>* 附註
>* 時數
>* 跨專案前置任務
>* 預算時數
>
>下列專案一律會從現有專案複製到新專案：
>
>* 任務
>* 範本
>* 風險
>* 佇列設定資訊
>* Portfolio與程式
>* 計分卡
>* 任務預設資訊(任務預設核准流程、任務預設自訂Forms)
>
> 專案上原始任務的日期複製到新專案。 您必須變更專案的開始或完成日期（視其排程模式而定）以更新任務的日期。 任務限制可能會阻止您變更專案日期。

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
   <td> <p>規劃 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>存取層級設定*</strong> </td> 
   <td> <p>編輯具有建立<span>和複製</span>專案功能的專案存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件許可權</strong> </p> </td> 
   <td> <p>檢視專案或更高的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 複製單一專案

複製專案也會將一些資訊從原始專案複製到新專案。 您也可以在複製過程中指定哪些專案不應複製到新專案。

若要複製專案：

1. 前往您要複製的專案，然後按一下專案名稱右側的&#x200B;**更多**&#x200B;圖示![更多功能表](assets/qs-more-menu.png)

   ![更多下拉式清單](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   前往專案清單或報告並選取專案，然後按一下清單頂端的&#x200B;**更多**&#x200B;圖示![更多](assets/qs-more-menu.png)。

   ![其他功能表已展開](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. 按一下&#x200B;**複製**。

1. 更新新專案的名稱。

   依預設，新名稱是&#x200B;**`<Original project name>`的復本。**

   ![複製專案方塊](assets/copy-project-box-nwe-350x276.png)

1. 選取新專案的&#x200B;**狀態**。

   根據預設，**狀態**&#x200B;與原始專案的狀態相符。

1. （選擇性）取消選取您不想要複製到新專案的專案。 下表說明取消選取專案時所發生的情況：


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全選</td> 
      <td> <p>選取所有選項，並清除新專案中列出的所有欄位和物件。</p> <p><b>秘訣</b>

   取消選取<strong>全選</strong>取消選取所有專案。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">指派</td> 
      <td>移除所有專案和任務指派</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進度</td> 
      <td>移除所有任務的進度，且顯示為新任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂資料</td> 
      <td> <p>從專案的自訂表單中移除資訊，以及與以下專案相關聯的自訂表單上的資訊：</p> 
       <ul> 
        <li>任務</li> 
        <li>費用</li> 
        <li> 文件</li> 
       </ul> <p><b>附註</b>

   自訂表單仍附加到任務、費用、檔案和專案，但表單自訂欄位中的資訊不會複製到新專案。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">文件</td> 
      <td> <p>移除檔案標籤中的所有專案，包括檔案版本、連結的檔案和資料夾。</p> <p>依預設，檔案校訂和核准無法複製到另一個專案。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任務</td> 
      <td> <p>移除專案上任務間的所有前置任務關係。 </p> <p><b>秘訣</b>

   跨專案前置任務絕不會轉移到新專案，無論是否選取此選項。 </p> </td>
   </tr>

<tr> 
      <td role="rowheader">預算時數</td> 
      <td> <p>從複製的專案中移除專案之業務案例的資源規劃區域中預算的時數。</p>

<b>附註</b>

使用「情境規劃工具」的預算時數永遠不會複製到新專案，因為新專案未連結到「情境規劃工具」中的方案。 如需詳細資訊，請參閱使用案例規劃工具</a>的業務案例中的<a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">預算資源
</tr></td>
    <tr> 
      <td role="rowheader">財務資訊</td> 
      <td> <p>移除下列區域中的資訊： </p> 
       <ul> 
        <li>專案的財務子標籤</li> 
        <li> 業務案例中的計畫收益</li> 
        <li>所有工作的財務資訊<br></li> 
       </ul> <p>如需有關專案財務子標籤的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">管理專案財務區域的資訊</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准流程</td> 
      <td>移除與任務或專案相關的所有核准。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td> 移除與任務或專案關聯的提醒通知。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>移除與任務或專案相關聯的費用。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">權限</td> 
      <td> 移除任務或專案上所有使用者的許可權。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**複製**&#x200B;以建立專案副本。

   這會建立一個新專案，其內容與您所複製的專案類似。

   您可以開始變更新複製的專案，例如稽核任務指派或調整時間表。
