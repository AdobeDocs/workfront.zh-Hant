---
product-area: projects
navigation-topic: manage-issues
title: 複製問題
description: 您可以複製問題或請求，並將其儲存在相同或其他專案中。 您也可以將問題從任務複製到另一個專案。
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# 複製問題

<!--Audited: 08/2025-->

您可以複製問題或請求，並將其儲存在相同或其他專案中。 您也可以將問題從任務複製到另一個專案。

您可以從下列物件複製問題：

* 從專案複製到相同專案（複製到相同專案）
* 從任務到相同任務（若為相同任務則重複）
* 從專案到另一個專案
* 從任務到專案

>[!TIP]
>
>在Workfront中，「問題」和「要求」可互換使用。 您可以同時記錄專案和任務的問題，以指出需要解決的無法預見的工作。 您也可以在指定為「請求佇列」的專案上提交記錄為問題的請求。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <ul><li><p>投稿人或以上</p> </li>
   <li><p>輕度或以上授權，可複製專案問題區段中的問題</p></li></ul>
   或
   <ul><li><p>要求者或以上</p> </li>
   <li><p>檢閱者或以上授權，可在專案的問題區段中複製問題</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題的存取權</p> <p>檢視專案和任務的或更高存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理問題的許可權</p> <p>將許可權貢獻給您要複製問題的專案，並具有「新增問題」功能。</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to copy an issue in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying the issue to with the ability to Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 複製問題時的注意事項

### 複製問題時的一般考量

在復製程式進行期間，您可以選取將一些與問題相關的料號複製到複製的問題。 不過，有些專案會預設轉移至新問題，有些則否，如下表所述。

依預設，下列專案會複製到新問題：

* 主要連絡人
* 自訂表格。 只有在複製過程中選取「自訂資料」時，自訂欄位中的資訊才會複製到新問題。
* 核准
* 計劃開始與計畫完成日期

依預設，下列物件不會複製到新問題：

* 記錄時數

### 與檔案或請求佇列相關問題的考量事項

複製包含檔案或與請求佇列關聯的問題時，請考量下列事項：

* **當問題與請求佇列關聯時：**&#x200B;當您將問題複製到另一個物件且問題與請求佇列關聯時，複製的問題不再與第一個問題源自的原始佇列關聯。
* **當檔案附加到問題時：**&#x200B;當您將問題複製到另一個物件且問題具有附加的檔案時，檔案及其版本也會移至新問題。 與檔案關聯的任何校訂或核准都不會移動。
* **當問題連結至檔案或資料夾時：**&#x200B;當您複製具有連結至第三方服務(例如Google Drive)之檔案或資料夾的問題時，檔案連結會傳輸到已複製的問題。

## 複製清單中的問題

您可以從問題清單或問題報告中複製一個或多個問題。

1. 移至包含您要複製之問題的專案。

   或

   前往問題報告。

1. 如果您選擇前往專案，請按一下左側面板中的&#x200B;**問題**。
1. 選取您要複製的問題並按一下問題清單頂端的&#x200B;**更多功能表**，然後按一下&#x200B;**複製到**。

   ![在清單中複製問題](assets/copy-issue-in-list-nwe-350x169.png)

1. 繼續複製問題，如從步驟2開始的[複製單一問題](#copy-a-single-issue)一節中所述。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## 複製單一問題 {#copy-a-single-issue}

您可以在檢視時複製一個問題。

1. 移至您要複製的問題，然後按一下問題名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-icon.png)，然後&#x200B;**複製到**。

   ![複製問題層級](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   顯示&#x200B;**複製問題**&#x200B;方塊。

   ![複製問題方塊](assets/copy-issue-box-nwe-350x285.png)

1. 在&#x200B;**選取目的地專案**&#x200B;區段中，指定您要複製問題的專案名稱。 預設會顯示目前專案的名稱。

   >[!TIP]
   >
   >清單中只會顯示100個專案。

1. （視條件而定）如果您沒有將問題複製到專案的存取權，請按一下&#x200B;**要求存取權**。
1. （視條件而定）如果您有權將問題新增至目的地專案上的任務之一，請繼續將問題複製到所選目的地專案，而不要求存取權。

   ![複製問題並要求存取權](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >如果Workfront管理員防止將問題新增到這些專案中，所選專案處於未決核准、已完成或已終止狀態，則會顯示類似訊息。 如需詳細資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

1. （選擇性）在&#x200B;**選項**&#x200B;區段中，取消選取下表所列的任何專案，以將其從新問題中移除。 依預設會選取所有選項。

   >[!NOTE]
   >
   >這只會影響複製的問題，不會影響原始問題。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">指派</td> 
      <td>移除指派給問題的使用者、工作角色或團隊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進度</td> 
      <td>移除問題的完成百分比（如有）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">文件</td> 
      <td><span style="line-height: 1.5;">移除檔案索引標籤中的所有專案，包括檔案版本、連結的檔案和資料夾。</span> <br>依預設，檔案校訂和核准無法複製到另一個問題。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">權限</td> 
      <td>移除與問題共用的實體。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新</td> 
      <td>從問題的更新區段移除評論。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂資料</td> 
      <td>移除問題自訂表單中的資訊，以及與問題附加檔案相關聯的自訂表單中的資訊（如果這些資訊也隨問題複製）。 自訂表單將保留附加到問題和檔案，但表單上的資訊將不會轉移到新問題中。 </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）在&#x200B;**選取任務**&#x200B;區段中，選取您要移動問題的任務。
1. 按一下「**複製問題**」，或如果您在清單中選取多個問題，請按一下「**複製問題**」。

   複製的問題會新增至指定的專案。


