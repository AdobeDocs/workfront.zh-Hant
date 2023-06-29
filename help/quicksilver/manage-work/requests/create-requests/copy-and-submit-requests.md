---
title: 複製並提交請求
description: 當您經常提交類似請求時，可以複製現有的已提交請求。 在這種情況下，您可以複製現有請求、對請求進行最低限度的變更，然後將其作為新請求重新提交。
author: Alina
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: bb68f15c2d8ffabfb67a7789de14ef916cd2dbef
workflow-type: tm+mt
source-wordcount: '1367'
ht-degree: 2%

---

# 複製並提交請求

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在「預覽」環境中可用。</span>

當您經常提交類似請求時，可以複製現有的已提交請求。 在這種情況下，您可以複製現有請求、對請求進行最低限度的變更，然後將其作為新請求重新提交。

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
您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>要求或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯問題的存取權</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>將請求新增至請求佇列的存取權</p> <p>檢視現有請求的或更高許可權</p> <p>如需設定請求佇列的詳細資訊，請參閱 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須有您或您組織內某人員先前提交的請求，才能複製並重新提交。 如果請求屬於其他人，您必須至少具有「檢視」的存取權，才能複製請求並將其提交為新請求。

## 將請求複製和提交為新請求的考量事項

* 您只能複製並提交已提交的請求。 您無法複製草擬的請求。
* 您可以複製並提交您最初提交的請求，或複製其他人提交的請求，而您至少可以存取「檢視」。
* 除非有人將您的許可權移除，否則您一律可以複製並提交您自己的請求副本。
* 當請求佇列的建立者啟用 **來自同一公司的人員將會為所有請求繼承相同的許可權** 在「佇列詳細資訊」或「編輯專案」區域中。 停用此設定僅允許原始請求者檢視自己的請求。

  如需詳細資訊，請參閱下列文章：

   * [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)

* 您可以先更新原始請求的副本，然後再將其作為新請求重新提交。
* 如果在提交原始請求後發生下列變更，您將無法再複製並重新提交：

   * 請求佇列已刪除。
   * 已刪除佇列主題。

     >[!TIP]
     >
     >如果佇列主題是請求佇列中唯一的主題，您仍然可以複製並提交請求，並將它儲存在請求佇列本身下。

   * 請求佇列不再作為說明請求佇列發佈。 如需詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * 如果請求佇列沒有佇列主題，且原始請求在2022年1月之前提交。

   * 與請求佇列相關聯的專案狀態不再是目前。

* 如果轉換過程中保留請求，您可以複製並提交轉換後請求的副本。 如需詳細資訊，請參閱 [在Adobe Workfront中轉換問題的概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >複製的請求未連結到解析物件。

## 複製並提交請求

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **請求**.
1. （視條件而定）如果「已提交」區段預設未顯示，請按一下 **已提交** 在左側面板中。
1. 找到您要複製並提交為新請求，然後執行下列任一項作業：

   * 選取它，然後按一下 <span class="preview"> **複製** ![](assets/copy-and-submit-as-new-requests-area-nwe.png)</span> （位於已提交請求清單的左上角）。

   >[!TIP]
   >
   > <span class="preview">如果您未先選取請求，復製圖示會變暗。</span>

   * 按一下 **更多** 功能表 ![](assets/more-icon.png) 請求名稱右側，然後按一下 **複製並提交為新檔案**

     或

     以滑鼠右鍵按一下選取的請求，然後按一下 **複製並提交為新檔案**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >當您無權建立問題時，您會收到一則警告，指出管理員限制您建立請求。

1. （選用）視需要更新下列資訊：

   * **請求型別**：儲存所複製請求的請求佇列。 依預設，複製的請求會儲存至原始請求的請求佇列。
   * **主題群組** 和 **佇列主題**，表示已選取。 系統會根據您的環境自訂名稱或主題群組以及佇列主題。 依預設，複製的請求會儲存至主題群組和原始請求的佇列主題。

     >[!TIP]
     >
     >如果路徑從原始請求的路徑變更，則請求佇列的建立者會修改佇列。

1. （選用）更新所複製請求的任何資訊。 根據請求佇列建立者在「 」中啟用的欄位 **新問題欄位** 部分 **佇列詳細資訊** 子索引標籤中，您可以找到下列任何欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>主旨</strong> </td> 
      <td>顯示原始請求的名稱。 如有需要，請加以更新。 否則，Workfront會將複製的請求命名為 <b>副本 &lt;name of="" original="" request=""&gt;</b>. 此為必填欄位。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>說明</strong> </td> 
      <td>顯示原始請求的描述。 如有需要，請加以更新。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>顯示原始請求的URL。 如有需要，請加以更新。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先順序</strong> </td> 
      <td> <p>指定要求的優先順序。 優先順序應定義您認為解決此請求的速度。 預設選項為：</p> 
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
      <td> <p>指定要求的嚴重程度。 嚴重程度應定義若無法及時解決此請求對您工作的影響。 預設選項為：</p> 
       <ul> 
        <li>輕微</li> 
        <li>導致混淆</li> 
        <li>有因應措施的錯誤</li> 
        <li>無因應措施的錯誤</li> 
        <li>致命錯誤</li> 
       </ul> <p>您的Workfront管理員可以修改嚴重程度的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>主要連絡人</strong> </td> 
      <td>請求的主要聯絡人預設為您負責，因為您是處理與請求相關之任何問題的聯絡人。 不過，您可以將其變更為任何其他Workfront使用者。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>指派</strong></span> </td> 
      <td> <p>指出請求應指派至之作用中使用者、工作角色或團隊的名稱。 </p> <p> 您可以指定多個使用者、工作角色或團隊。 </p> <p>視請求佇列的設定方式而定，您可能只能將請求指派給一或兩種型別的資源，而非全部三種。 </p> <p>我們建議對您的請求佇列使用路由規則，以便這些佇列可以自動路由到適當的資源。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">視要求佇列的設定方式而定，您只能將一種資源型別指派給要求（例如使用者）。 如果路由規則也與請求佇列相關聯，並且自動將請求路由到不同型別的資源（例如，團隊），則您的請求會同時指派給提交請求時手動指定的實體（使用者）和路由規則中指定的資源（團隊）。</p> <p style="font-weight: normal;">如需詳細資訊，請參閱下列文章：</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">建立路由規則</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫小時</strong> </td> 
      <td> <p>預估完成此請求需要多少小時。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫開始日期</strong> </td> 
      <td> <p>開始處理此請求的日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫完成日期</strong> </td> 
      <td>您想要解決此請求的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>狀態</strong> </td> 
      <td>新請求的預設狀態為「新」。 您的Workfront管理員可能已變更此狀態的名稱。 您也可以從此下拉式功能表將狀態變更為其他內容。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文件</strong> </td> 
      <td> <p>將檔案新增至您的請求。 附加至原始請求的檔案不會轉移到複製的請求。</p> <p><b>秘訣</b>

   視請求佇列的設定方式而定，檔案區段可能會顯示在自訂欄位之前或之後。</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. （選用）如有需要，可更新附加自訂表單中的任何資訊。

   >[!TIP]
   >
   >* 附加到原始請求的所有自訂表單和自訂欄位中包含的值都會轉移到複製的請求。 這包括包含邏輯的欄位。
   >* 您無法從複製的請求中移除自訂表單。

1. 按一下 **提交**.

   複製的請求會以新請求的形式提交至您指定的請求佇列中。
