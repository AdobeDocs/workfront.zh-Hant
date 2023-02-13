---
title: 複製和提交請求
description: 複製和提交請求
author: Alina
draft: Probably
feature: Work Management
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# 複製和提交請求

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is NWE only - hard code it in classic articles!)</p>
-->

當您經常提交類似請求時，可以複製現有的已提交請求。 在這種情況下，您可以複製現有請求，對其進行最少的更改，然後作為新請求重新提交。

## 存取需求

<!--drafted - replace table with P&P:

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
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
-->
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
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯問題的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>將請求新增至請求佇列的存取權</p> <p>檢視現有請求的或更高權限</p> <p>如需設定請求佇列的相關資訊，請參閱 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您之前必須提交您或組織中的某人的請求，才能複製並重新提交。 如果請求屬於其他人，您必須至少擁有「檢視」的存取權，才能複製並以新的形式提交。

## 將請求複製和提交為新請求的考量事項

* 您只能複製和提交已提交的請求。 您不能複製起草的請求。
* 您可以複製並提交您最初提交的請求，或請求其他人提交且您至少有權存取「檢視」。
* 除非有人移除了您的權限，否則您一律有權複製並提交您自己請求的副本。
* 當請求佇列的建立者啟用 **來自同一公司的人員將繼承所有請求的相同權限** 在「隊列詳細資訊」或「編輯項目」區域中。 停用此設定只允許原始請求者檢視其自己的請求。

   如需詳細資訊，請參閱下列文章：

   * [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)

* 您可以在將原始請求重新提交為新請求之前，更新其副本。
* 如果在提交原始請求後發生了以下更改，則無法再複製並重新提交：

   * 請求隊列已刪除。
   * 已刪除隊列主題。

      >[!TIP]
      >
      >如果佇列主題是請求佇列中唯一的主題，您仍可以複製並提交請求，請求會儲存在請求佇列本身下。

   * 請求佇列不再發佈為「說明請求佇列」。 如需詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * 如果請求佇列沒有佇列主題，且原始請求是在2022年1月之前提交的。

   * 與請求佇列相關聯的專案狀態已不再為「最新」。

* 如果請求保留在轉換過程中，您可以複製並提交轉換請求的副本。 如需詳細資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

   >[!TIP]
   >
   >複製的請求不連結到解析對象。

## 複製和提交請求

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **請求**.
1. （條件性）如果「已提交」區段預設未顯示，請按一下 **已提交** 中。
1. 找到您要複製並以新方式提交的請求，然後執行下列任一操作：

   * 選取它，然後按一下 **複製並提交為新** 圖示 ![](assets/copy-and-submit-as-new-requests-area-nwe.png) 位於「已提交請求」清單的左上角。
   * 按一下 **更多** 功能表 ![](assets/more-icon.png) 在請求名稱的右側，按一下 **複製並提交為新**

      或

      以滑鼠右鍵按一下所選取的請求，然後按一下 **複製並提交為新**.

      ![](assets/request-selected-more-menu-options-nwe-350x191.png)

      >[!TIP]
      >
      >當您沒有建立問題的存取權時，會收到警告，指出管理員限制您建立請求。

1. （選用）視需要更新下列資訊：

   * **請求類型**:儲存複製請求的請求佇列。 依預設，複製的請求會儲存至原始請求的請求佇列。
   * **主題群組** 和 **佇列主題**，則會選取。 系統會根據您的環境自訂名稱或主題群組和佇列主題。 依預設，複製的請求會儲存至原始請求的主題群組和佇列主題。

      >[!TIP]
      >
      >如果路徑與原始請求的路徑不同，則請求隊列的建立者修改了隊列。

1. （選用）更新複製之請求的任何資訊。 請求佇列建立者會在 **新問題欄位** 區段 **隊列詳細資訊** 在專案上的子標籤中，您可能會找到下列任何欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>主旨</strong> </td> 
      <td>顯示原始請求的名稱。 如有需要，請更新。 否則，Workfront會為複製的請求命名 <b>副本 &lt;name of="" original="" request=""&gt;</b>. 這是必填欄位。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>說明</strong> </td> 
      <td>顯示原始請求的說明。 如有需要，請更新。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>顯示原始請求的URL。 如有需要，請更新。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先順序</strong> </td> 
      <td> <p>指定請求的優先順序。 優先順序應定義您認為此請求應解決的速度。 預設選項為：</p> 
       <ul> 
        <li>無</li> 
        <li>低</li> 
        <li>標準</li> 
        <li>高</li> 
        <li>緊急</li> 
       </ul> <p>您的Workfront管理員可以修改優先順序的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>嚴重程度</strong> </td> 
      <td> <p>指定請求的嚴重性。 嚴重性應定義此請求對您的工作所產生的影響，以防其及時解決。 預設選項為：</p> 
       <ul> 
        <li>輕微</li> 
        <li>導致混淆</li> 
        <li>有因應措施的錯誤</li> 
        <li>無因應措施的錯誤</li> 
        <li>致命錯誤</li> 
       </ul> <p>您的Workfront管理員可以修改嚴重性名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>主要連絡人</strong> </td> 
      <td>請求的主要聯繫人預設為您，因為您是處理與請求相關的任何問題的要員。 不過，您可以將此變更為任何其他Workfront使用者。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>指派</strong></span> </td> 
      <td> <p>指定應將請求分配給的活動用戶、作業角色或團隊的名稱。 </p> <p> 您可以指定多個用戶、作業角色或團隊。 </p> <p>根據請求佇列的設定方式，您可能只能將請求指派給一或兩種資源類型，而非全部三種資源。 </p> <p>我們建議使用「請求隊列」的「路由規則」，以便自動將它們路由到相應的資源。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">根據請求佇列的設定方式，您可能只能將一種類型的資源指派給請求（例如使用者）。 如果路由規則也與請求隊列關聯，並且它自動將請求路由到不同類型的資源（例如，團隊），則您的請求將分配給在提交請求時手動指定的實體（用戶）和路由規則中指定的資源（團隊）。</p> <p style="font-weight: normal;">如需詳細資訊，請參閱下列文章：</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">建立路由規則</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫小時</strong> </td> 
      <td> <p>預估完成此要求所需的時間。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫開始日期</strong> </td> 
      <td> <p>處理此請求的開始日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫完成日期</strong> </td> 
      <td>您要解決此請求的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>狀態</strong> </td> 
      <td>新請求的預設狀態為「新」。 您的Workfront管理員可能已變更此狀態的名稱。 您也可以從此下拉式功能表，將狀態變更為其他項目。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文件</strong> </td> 
      <td> <p>將檔案新增至您的請求。 附加至原始請求的檔案不會轉移至複製的請求。</p> <p><b>筆尖</b>

   視請求佇列的設定方式而定， 「檔案」區段可能會在自訂欄位之前或之後顯示。</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. （可選）視需要更新附加的自訂表單中的任何資訊。

   >[!TIP]
   >
   >* 附加至原始請求的所有自訂表單以及自訂欄位中包含的值，都會轉移至複製的請求。 這包括包含邏輯的欄位。
   >* 您無法從複製的請求中移除自訂表單。


1. 按一下 **提交**.

   複製的請求會在您指定的請求佇列中，以新請求的形式提交。
