---
title: 使用版面範本自訂篩選器、檢視和群組
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 身為Workfront管理員，您可以使用配置範本，指定在「篩選」、「檢視」和「分組」下拉式功能表中顯示的清單控制項。 這些功能表會顯示在整個Workfront的清單上方，例如專案的工作清單。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# 使用版面範本自訂篩選器、檢視和群組

身為Adobe Workfront管理員，您可以使用配置範本，指定在「篩選」、「檢視」和「分組」下拉式功能表中顯示的清單控制項。 以下功能表會顯示在整個Workfront的清單上方，例如專案的工作清單：

![](assets/filter-view-grouping-layout-templates.png)

如需版面範本的詳細資訊，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

如需群組版面範本的相關資訊，請參閱 [建立和修改群組的版面範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>要在系統級別執行這些步驟，需要系統管理員訪問級別。
要為組執行這些操作，您必須是該組的經理。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂篩選、檢視和分組清單控制項：

1. 開始使用版面範本，如 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 按一下向下箭頭 ![](assets/down-arrow-blue.png) 在 **自訂使用者看見的項目**，然後按一下 **清單** 在顯示的下拉式功能表中。

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. 按一下向下箭頭 ![](assets/down-arrow-blue.png) 在 **選取要自訂的清單**，然後選取您要自訂篩選、檢視和分組清單控制項的Workfront物件類型。

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >如果您選取「專案」作為自訂清單，然後在「篩選」區段中停用「我所在的專案」或「我擁有的專案」，使用者將看不到或無法使用該篩選：
   >
   >* 在篩選器清單中，當它們按一下篩選器圖示時顯示 ![](assets/filter-nwepng.png) 清單上方：
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* 在「項目」區域標題的標題中：
   >   
   >  ![](assets/disable-filter-pills.png)

1. （可選）如果您想要變更版面範本的預設篩選、檢視或分組，請將滑鼠指標暫留在篩選、檢視或分組上，然後按一下 **設為預設值**.

   當配置範本指派給使用者時，您選擇的預設值會決定使用者在整個Workfront的清單中會看到的篩選、檢視和分組。 如果您未變更這些預設值，使用者會查看下列所有清單：

   * **篩選器**:全部
   * **檢視**:標準(如適用；某些清單沒有此視圖)
   * **分組**:無

   選取不同的預設值後，您可以隱藏「全部」、「標準」和「無」選項（請參閱步驟5），但無法刪除這些選項。

   您可以刪除其他作為預設值的選項，但必須先選取不同的預設值。

   如需刪除篩選器、檢視和群組的相關資訊，請參閱 [建立、編輯和共用預設篩選器、檢視和群組](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. 按如下方式隱藏和添加清單控制項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">隱藏清單控制項</td> 
      <td> <p>清除或勾選您要隱藏或顯示的清單控制項旁的方塊。</p> <p>如果核取方塊呈暗灰色，則無法隱藏該清單控制項。 預設 <img src="assets/default-pill.png"> 每個清單控制項的設定都會呈現灰色，因為您無法隱藏目前設定為預設的設定。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">新增自訂清單控制項</td> 
      <td> <p> 
        <ol> 
         <li value="1"> 按一下 <strong>新增篩選</strong>, <strong>添加視圖</strong>，或 <strong>添加分組</strong> （在「篩選器」、「視圖」或「分組」清單的底部）。 在隨即顯示的方塊中，開始輸入先前為組織建立的現有自訂清單控制項的名稱，然後在出現時按一下名稱。</li> 
         <li value="2"> 如果要將新的自訂清單控制項設定為版面範本的預設篩選、檢視或分組，請按一下 <strong>設為預設值</strong>. </li> 
         <li value="3"> <p>按一下 <strong>新增</strong> 時，才能執行此操作。</p> <p><b>附註</b>: <p>使用者可將自訂清單控制項新增至自己的清單。 如果您在版面範本中新增自訂清單控制項，則會新增清單控制項，並將其移至面板底部；你的不能取代他們的。</p> <p>如果您將使用者指派至具有自訂清單控制項的新版面範本，也會是如此。 </p> <p>如需自訂清單控制項的相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Adobe Workfront中的篩選器概觀</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Adobe Workfront中的檢視概觀</a>，和 <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Adobe Workfront中的群組概觀</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續自訂配置範本。

   或

   如果您已完成自訂，請按一下 **儲存**.

   >[!TIP]
   >
   >您可以隨時按一下「儲存」以儲存進度，然後稍後繼續修改範本。
