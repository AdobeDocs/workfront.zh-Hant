---
product-area: projects
navigation-topic: manage-tasks
title: 在「任務詳細資訊」部分中管理任務財務
description: 在「任務詳細資訊」部分中管理任務財務
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 5%

---

# 在「任務詳細資訊」部分中管理任務財務

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

通過訪問「任務詳細資訊」部分的「概覽」區域，可以查看或編輯任務的財務資訊。 在此區域中可查看或編輯的欄位數量有限。 有關編輯任務的所有財務資訊的資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案和工作的存取權</p> <p>查看對Financial Data或更高版本的訪問</p> <p>您必須具有對財務資料的編輯訪問權限，才能編輯有關任務的財務資訊</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看包含查看財務或更高版本的任務的權限</p> <p>您必須對包括編輯財務的任務具有管理權限，才能編輯有關任務的財務資訊</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在「任務詳細資訊」部分中編輯任務財務

1. 轉到要查看任務的項目。

   >[!NOTE]
   >
   >要查找任務，您也可以搜索該任務，然後按一下名稱以訪問該任務。 如需在Workfront中搜尋物件的詳細資訊，請參閱 [搜尋Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. 按一下 **工作** 中。
1. 按一下要查看的任務的名稱。
1. 按一下 **任務詳細資訊**.
1. （選用）按一下 **全部折疊** 表徵圖。

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >視您的Workfront管理員或群組管理員設定「配置範本」的方式而定，「任務詳細資料」區段中的欄位可能會重新排列或未顯示。 如需詳細資訊，請參閱 [使用版面範本自訂「詳細資料」檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 按一下 **金融** 展開並查看任務的財務資訊。

   按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在「詳細資料」區段的右上角，按一下 **金融**.

1. 按一下欄位或按一下，編輯任何可供編輯的欄位 **+添加** 將資訊添加到空欄位。
1. 在 **金融** 區域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">成本類型</td> 
      <td> <p>指定任務的成本類型。 這將根據任務的小時數確定如何計算任務的成本。 </p> <p>從下列選項中選取： </p> 
       <ul> 
        <li> <p>無成本</p> </li> 
        <li> <p>固定小時 </p> </li> 
        <li> <p> 使用者小時 </p> </li> 
        <li> <p> 角色小時</p> </li> 
       </ul> <p>如需追蹤成本的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a> . 您的Workfront管理員或群組管理員會為系統或群組中的任務選取預設的成本類型設定。 有關設定項目預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入類型</td> 
      <td> <p>指定任務的「收入類型」。 這將根據任務上的小時數，確定如何計算任務上的收入。 </p> <p>從下列選項中選取： </p> 
       <ul> 
        <li> <p> 不可記帳 </p> </li> 
        <li> <p>使用者小時 </p> </li> 
        <li> <p>角色小時 </p> </li> 
        <li> <p>固定小時 </p> </li> 
        <li> <p>受限使用者小時 </p> </li> 
        <li> <p>受限角色小時 </p> </li> 
        <li> <p>使用者小時加固定 </p> </li> 
        <li> <p>角色小時加固定 </p> </li> 
        <li> <p>固定收入 </p> </li> 
       </ul> <p>如需追蹤收入的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單和收入概觀</a> . </p> <p>您的Workfront管理員或群組管理員會針對您系統或群組中的任務選取預設的「收入類型」設定。 有關設定項目預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計畫成本</td> 
      <td> <p>此計算根據計畫小時數、成本類型以及用戶或職務職責的小時費率顯示任務成本。 如需追蹤成本的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際成本</td> 
      <td> <p> 這是一種計算，它根據實際小時數、成本類型以及用戶或任務角色的小時費率顯示任務成本。 如需追蹤成本的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計畫收入</td> 
      <td> <p>此計算會根據計畫小時數、收入類型以及用戶或職務角色的小時費率顯示與任務關聯的收入。 如需追蹤成本的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際收入</td> 
      <td> <p>此計算會根據實際小時數、收入類型以及用戶或職務角色的小時費率，顯示與任務關聯的收入。 如需追蹤成本的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI / SPI / CSI</strong> </td> 
      <td> <p>這些是任務效能度量，顯示您的任務在給定時間的執行情況。 其值是根據專案的「效能索引」方法計算。<br>如需詳細資訊，請參閱下列文章：</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">計算成本績效指數(CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">計算計畫效能索引(SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">計算成本計畫效能指數(CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成時估計(EAC)</td> 
      <td> <p>此計算顯示任務完成時的總成本。 如需完成時預估的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">完成時計算估計值(EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （條件性）如果您正在編輯「財務」部分中的欄位，請按一下 **儲存****變更**.
