---
title: 複製並提交請求
description: 當您經常提交類似的請求時，可以複製現有的已提交請求。 在這種情況下，您可以複製現有請求、對請求進行最低限度的變更，然後將其作為新請求重新提交。
author: Alina
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 0ffae8ed285f6e9164a239552feb90465bea3cca
workflow-type: tm+mt
source-wordcount: '1361'
ht-degree: 2%

---

# 複製並提交請求

當您經常提交類似的請求時，可以複製現有的已提交請求。 在這種情況下，您可以複製現有請求、對請求進行最低限度的變更，然後將其作為新請求重新提交。

<!--Old?? 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++
-->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：投稿人或更高版本</p>
   或
   <p>目前：要求或以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題的存取權</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader">物件許可權</td> 
   <td><p>將請求新增至請求佇列的存取權</p> <p>檢視現有請求或更高的許可權</p> <p>如需設定要求佇列的資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立要求佇列</a>。 </p> </td> 
  </tr>
  <tr> 
   <td role="rowheader"> 產品</td> 
   <td> <ul><li>Adobe Workfront</li><li>您必須安裝Adobe Workfront Planning才能檢視Planning請求或請求表單</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須要求您或您組織內的某人先前已提交，才能複製並重新提交。 如果請求屬於其他人，您必須至少具有「檢視」存取權，才能複製並提交為新請求。

## 複製和提交請求為新請求的考量事項

* 您只能複製並提交已提交的請求。 您無法複製草擬的請求。
* 您可以複製並提交您最初提交的請求，或其他人提交的請求，而您至少可以存取檢視。
* 除非有人將您的許可權移除，否則您一律可以複製並提交您自己的請求副本。
* 當請求佇列的建立者啟用&#x200B;**來自相同公司的人員將會在「佇列詳細資料」或「編輯專案」區域中繼承所有請求的相同許可權**&#x200B;時，原本由其他人提交之複製及提交請求的存取權可能會自動授予相同公司的人員。 停用此設定僅允許原始請求者檢視其自己的請求。

  如需詳細資訊，請參閱下列文章：

   * [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)

* 您可以更新原始請求的副本，然後再將它重新提交為新請求。
* 如果在提交原始請求後發生以下變更，您將無法再複製並重新提交：

   * 請求佇列已刪除。
   * 已刪除佇列主題。

     >[!TIP]
     >
     >如果佇列主題是請求佇列中唯一的主題，您仍可以複製並提交請求，並將它儲存在請求佇列本身下。

   * 此請求佇列不再作為說明請求佇列發佈。 如需詳細資訊，請參閱[建立要求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。
   * 如果請求佇列沒有佇列主題，且原始請求是在2022年1月之前提交。

   * 與請求佇列關聯的專案狀態不再是目前。

* 如果轉換過程中保留了請求，您可以複製並提交轉換請求的副本。 如需詳細資訊，請參閱[在Adobe Workfront中轉換問題的概觀](../../../manage-work/issues/convert-issues/convert-issues.md)。

  >[!TIP]
  >
  >複製的請求未連結到解析物件。

## 複製並提交請求

{{step1-to-requests}}

1. （視條件而定）如果「已提交」區段預設未顯示，請按一下左側面板中的&#x200B;**已提交**。

   >[!TIP]
   >
   >   您的Workfront或群組管理員可能會自訂您的版面配置範本，並從您的環境的主功能表或左側面板中移除區域。 在此情況下，您可能無法使用它們。

1. 找到您要複製並提交為新內容的請求，然後執行下列任一項作業：

   * 選取它，然後按一下[已提交請求]清單左上角的&#x200B;**複製** ![](assets/copy-and-submit-as-new-requests-area-nwe.png)。

   >[!TIP]
   >
   > 如果您未先選取請求，復製圖示會變暗。

   * 按一下要求名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**複製並送出為新專案**

     或

     在選取的請求上按一下滑鼠右鍵，然後按一下[複製]並送出為新請求&#x200B;**。**

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >當您無權建立問題時，您會收到一則警告，指出管理員限制您建立請求。

1. （選用）如有需要，請更新下列資訊：

   * **請求型別**：儲存所複製請求的請求佇列。 依預設，複製的請求會儲存至原始請求的請求佇列。
   * 如果選取&#x200B;**主題群組**&#x200B;和&#x200B;**佇列主題**。 系統會針對您的環境自訂名稱或主題群組以及佇列主題。 依預設，複製的請求會儲存至主題群組和原始請求的佇列主題。

     >[!TIP]
     >
     >如果路徑從原始請求的路徑變更，則請求佇列的建立者會修改佇列。

1. （選用）更新所複製請求的任何資訊。 根據請求佇列建立者在專案的&#x200B;**佇列詳細資料**&#x200B;子標籤的&#x200B;**新問題欄位**&#x200B;區段中啟用的欄位，您可能會找到下列任何欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>主旨</strong> </td> 
      <td>顯示原始請求的名稱。 如有需要，請更新。 否則，Workfront會將複製的請求命名為<b> &lt;原始請求的名稱&gt;</b>的副本。 此為必填欄位。</td> 
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
      <td> <p>指定要求的優先順序。 優先順序應定義您認為解決此請求的速度。 預設選項為：</p> 
       <ul> 
        <li>無</li> 
        <li>低</li> 
        <li>正常</li> 
        <li>高</li> 
        <li>緊急</li> 
       </ul> <p>您的Workfront管理員可以修改優先順序的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>嚴重性</strong> </td> 
      <td> <p>指定要求的嚴重程度。 嚴重程度應該定義如果不能及時解決此請求對您工作的影響。 預設選項為：</p> 
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
      <td>您會預設為請求的主要聯絡人，因為您是處理任何與請求相關問題的直接人員。 不過，您可以將其變更為任何其他Workfront使用者。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>指派</strong></span> </td> 
      <td> <p>指出請求應指派至之作用中使用者、工作角色或團隊的名稱。 </p> <p> 您可以指定多個使用者、工作角色或團隊。 </p> <p>根據請求佇列的設定方式，您或許只能將請求指派給一或兩種資源，而非全部三種。 </p> <p>建議您使用請求佇列的路由規則，讓請求佇列可自動路由至適當的資源。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">視要求佇列的設定方式而定，您只能將一種資源型別指派給要求（例如使用者）。 如果路由規則也關聯到請求佇列，而且它會自動將請求路由到不同型別的資源（例如，小組），則您的請求會同時指派給提交請求時手動指定的實體（使用者）以及路由規則中指定的資源（小組）。</p> <p style="font-weight: normal;">如需詳細資訊，請參閱下列文章：</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">建立路由規則</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>規劃時數</strong> </td> 
      <td> <p>預估完成此請求所需的時間。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計劃開始日期</strong> </td> 
      <td> <p>開始處理此請求的日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫完成日期</strong> </td> 
      <td>您想要解決此請求的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>狀態</strong> </td> 
      <td>新請求的預設狀態為「新增」。 您的Workfront管理員可能已變更此狀態的名稱。 您也可以從此下拉式功能表將狀態變更為其他專案。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文件</strong> </td> 
      <td> <p>將檔案新增至您的請求。 附加到原始請求的檔案不會轉移到複製的請求。</p> <p><b>秘訣</b>

   視請求佇列的設定方式而定，檔案區段可能會顯示在自訂欄位之前或之後。</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. （選用）如有需要，可更新附加自訂表單中的任何資訊。

   >[!TIP]
   >
   >* 附加到原始請求的所有自訂表單和自訂欄位中包含的值都會轉移到複製的請求。 這包括包含邏輯的欄位。
   >* 您無法從複製的請求中移除自訂表單。

1. 按一下&#x200B;**提交**。

   複製的請求會在您指定的請求佇列中作為新請求提交。
