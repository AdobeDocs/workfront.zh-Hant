---
content-type: overview
product-area: projects
navigation-topic: manage-projects
title: 管理專案概述區域中的資訊
description: 管理專案概述區域中的資訊
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6113bc62-18f2-4558-bc2f-986b1e7d1a83
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 4%

---

# 管理專案概述區域中的資訊

<!--
<p>(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

您可以存取專案詳細資訊區段的概觀區域來檢視或編輯專案的資訊。 您可以在此區域中檢視或編輯的欄位數量有限。 如需有關編輯專案所有資訊的資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

## 存取需求

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
   <td role="rowheader"> <p role="rowheader">Adobe Workfront授權*</p> </td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視專案的存取權或以上許可權 </p>

<p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何變更您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案的存取權以檢視專案的有限資訊</p> 
   <p>管理專案的存取權以編輯專案的相關資訊</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 存取「概覽」區段

1. 前往您要檢視其概觀區段的專案。
1. 按一下 **專案詳細資訊** 在左側面板中。
1. 此 **概觀** 區段應該首先顯示為專案詳細資料的一部分，並且預設應該展開

   或

   按一下 **編輯** 圖示 ![](assets/edit-icon.png) 「詳細資訊」區段的右上角，然後按一下 **概觀**. 如此將可開啟「概述」區域以進行編輯。

   >[!NOTE]
   >
   >根據Workfront管理員設定版面配置範本的方式，概觀區段可能不會列在前，在此情況下會摺疊。 如需詳細資訊，請參閱 [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. （視條件而定）如果專案上有特定欄位需要更新，但未顯示在此區段中，請按一下 **更多選單** ![](assets/more-icon.png) 在專案名稱旁，然後 **編輯** 以檢視更多專案欄位。

   如需有關編輯專案的詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 編輯或檢閱下表中顯示在中的欄位 **概觀** 區段。\
   若要編輯任何可編輯的欄位，請按一下該欄位或按一下 **+新增** 將資訊新增至空白欄位。

   >[!NOTE]
   >
   >視您的Workfront管理員如何設定版面配置範本而定，可能不會顯示所有欄位。 如需詳細資訊，請參閱 [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader"><b>欄位</b></td> 
      <td><b>說明</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader">說明</td> 
      <td>說明此專案的用途。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td>在此欄位中插入任何URL。 它可以是Workfront URL或任何其他網址。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">優先順序</td> 
      <td>作為專案的指定優先順序或重要性。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">狀態</td> 
      <td> <p>專案狀態。 </p> <p>提示：除非已完成所有任務和問題，否則您無法完成專案。 如果專案的「完成模式」設定為「自動」，您將無法手動完成專案。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">條件型別</td> 
      <td>判斷管理員是否設定專案條件，或Workfront是否設定。 如需有關專案狀況的資訊，請參閱文章 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">專案狀態與狀態型別概觀</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">排程模式</td> 
      <td>設定專案的排程方式。 例如，專案是從「開始日期」排程，還是從「完成日期」排程。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計劃開始日期和時間</td> 
      <td> 專案計劃開始的時間。 當專案從開始日期排程時，這由專案經理手動設定。 當專案從完成日期排程時，Workfront會根據專案中任務的持續時間自動設定此日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">計畫完成日期和時間</td> 
      <td> 專案計畫完成的時間。 當專案從「完成日期」開始排程時，這由專案經理手動設定。 當專案從開始日期排程時，Workfront會根據專案中任務的持續時間自動設定此日期。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">專案組合</td> 
      <td>與專案相關聯的投資組合。 您必須先建立投資組合，才能將其新增至專案。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">方案</td> 
      <td>與專案投資組合關聯的方案。 您必須先建立方案，才能將其新增至專案。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">群組</td> 
      <td> <p>與專案相關聯的群組。</p> <p>您可以將游標移至正確的群組上，並按一下資訊圖示，藉此確定您選取的群組正確 <img src="assets/info-icon.png"> 隨即顯示。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
      依照預設，除非您指定不同的群組，否則下列其中一個群組會在建立專案時自動與專案相關聯：
        <ul> 
         <li> <p><span>從專案區域建立專案時，專案建立者的「主群組」會與專案相關聯。</span> </p> </li> 
         <li> <p><span>從設定區域中群組的首頁面建立專案時，該群組會自動與專案建立關聯。</span> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td>與專案關聯的公司。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">專案所有者 </td> 
      <td>這是專案的所有者。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">專案贊助者</td> 
      <td> <p>這是專案的主要利害關係人。 這通常是主管監督及支援專案，或是負責預算的人。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">資源管理員</td> 
      <td> <p>這是可以管理專案中使用者資源的人員。 </p> <p>如需有關Resource Manager的資訊，請參閱文章 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md" class="MCXref xref">指定專案或範本的資源管理員 </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >更新「專案所有者」、「專案贊助者」和「資源管理員」欄位時，請注意顯示圖片、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。
   >
   >使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
   > 
   >您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱 [授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. 檢閱「概述」區段中的下列欄位。 您無法編輯下列欄位：

   | 欄位 | 說明 |
   |---|---|
   | 參考號碼 | 這是自動產生的欄位，且每個專案一律有唯一值。 |
   | 預計開始日期 | 這是根據已完成工作和剩餘工作開始工作的「即時」日期。 |
   | 預計完成日期 | 這是專案即將完成的「即時」日期，此日期會根據已完成任務的進度以及處於「新增」或「進行中」狀態之任務的進度更新。 |
   | 計畫小時 | 專案上的計畫時數。 這些時數是每個任務的計畫時數總計。 |
   | 實際時數 | 專案所記錄的小時。 這些小時是專案、任務或專案問題的記錄小時總數。 |
   | 計畫持續時間 | 專案將持續的時間，根據任務的最早計劃開始日期與專案上任務的最近計畫完成日期之間的時間範圍。 |
   | 實際期間 | 根據任務的最早實際開始日期與專案上任務的最晚實際完成日期之間的時間範圍，專案實際跨越的時間量。 |
   | 輸入日期 | 專案的建立日期和時間。 |
   | 輸入者 | 建立專案的使用者名稱。 |
   | 上次更新日期 | 專案上次更新的日期與時間。 |
   | 上次更新者 | 上次更新專案的使用者名稱。 |
   | 範本 |   |


1. 如果您的公司已購買Adobe Workfront Scenario Planner的額外授權，並且專案具有從連結的方案發佈的資訊，請在Scenario Planner區域中檢閱以下方案資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>欄位</b></td> 
      <td><b>說明</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader"><span>行動方案期間</span> </td> 
      <td><span>專案連結至方案時，對應方案的持續時間。 此欄位不可編輯。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>上次發佈日期</span> </td> 
      <td><span>專案上次從對應方案發佈的日期。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>方案開始日期</span> </td> 
      <td><span>當專案連結至方案時，方案開始月份的第一天。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>方案結束日期</span> </td> 
      <td><span>方案結束月份的最後一天，即專案連結至方案時。 </span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>FTE和時數中的方案工作角色</span> </td> 
      <td> <p>方案之相關職務角色及其時間配置的相關資訊。 其中包括：</p> 
       <ul> 
        <li>工作角色名稱</li> 
        <li>FTE數量</li> 
        <li> <p>所有FTE的小時數</p> <p>您可以使用時數或FTE來預估計畫或方案所需的工作角色數量。 </p> <p>如需詳細資訊，請參閱 <a href="../../../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在「情境規劃工具」中建立和編輯計畫</a>. </p> </li> 
       </ul> <p>秘訣： <span>如果方案中每個月的工作角色數量不同，此欄位會顯示方案所需的最大角色數量。 例如，如果您在1月需要1名顧問，在2月需要2名，則欄會顯示2FTE以及所有月份2個FTE的對應時數金額。</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   如需連結專案與方案的詳細資訊，請參閱 [透過在情境規劃工具中發佈行動方案來更新或建立專案](../../../scenario-planner/publish-scenarios-update-projects.md).

1. 按一下 **儲存變更**.
