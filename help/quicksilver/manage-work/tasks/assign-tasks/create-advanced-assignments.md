---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 建立進階任務指派
description: 您可以使用「進階指派」來管理任務或問題指派。
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: daaa13d5a3ebbd249f0093181ee7834f9db43fdb
workflow-type: tm+mt
source-wordcount: '3457'
ht-degree: 0%

---

# 建立進階任務指派

<!-- Audited: 11/2025-->

<!--remove the bullet indicated when we get rid of the new/old experience of editing tasks-->


<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

您可以使用「進階指派」來管理任務或問題指派。

進行進階指派時，您可以調整下列指派資訊：

* 將使用者指派給任務或問題（這可以在進階指派之外完成）。
* 調整並重新分配每個受指派人分配的時數。
* 決定應指定為任務或問題之擁有者或主要受指派者的使用者。
* 指定每個使用者在處理任務或問題時履行哪個角色。
* 在指定層次新增帳單與成本費率資訊。
* 複查每個指派的下列明細：計畫時數、總成本及總收入。

>[!NOTE]
>
>指派使用者工作時，其根據排程的可用性會影響任務和問題的計畫和預計日期。 如需排程的相關資訊，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

## Adobe Workfront中您可以進行進階指派的區域

本文會說明如何在任務或問題的標題中存取進階工作總攬。

此外，您可以在Workfront的下列區域中執行進階任務指派：

* 在清單與報表中，當「工作總攬」欄位顯示在檢視中時。
* 編輯任務時顯示在「工作總攬」區段中。 如需詳細資訊，請參閱[編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。<!--When we remove the old/ new experience: take this bullet out completely; in the new Edit Task experience, this is no longer possible-->
* 在任務或問題標題中，在指派區域中。
* 在工作負載平衡器中。 如需詳細資訊，請參閱[使用工作負載平衡器](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md)手動指派工作。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td> <p>若要在任務指派上新增帳單與成本費率，並使用進階搜尋：工作流程Ultimate</p> <p>若要建立進階工作分派：任何Workfront或Workflow封裝</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>工作或更高層級</p>
   </td> 
  </tr> 
  <tr> 
   <td role>存取層級設定</td> 
   <td> <p>編輯任務和問題的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p>貢獻或更高的任務或問題許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立進階任務指派 — 工作流程Ultimate套件

此「進階工作總攬」的版面配置僅適用於任務。 如需瞭解問題，請參閱[建立進階指派 — 所有其他封裝](#create-advanced-assignments--all-other-packages)。

>[!NOTE]
>
>預設為舊的進階指派體驗。 您必須使用「進階指定」視窗右上角的按鈕，手動開啟新體驗。
>如需舊體驗的相關資訊，請參閱下方的[建立進階工作分派 — 所有其他套件](#create-advanced-assignments--all-other-packages)。

1. 前往您要指派任務的專案。
1. 按一下左側面板中的&#x200B;**任務**&#x200B;或&#x200B;**問題**，然後按一下清單中任務的名稱。

   >[!TIP]
   >
   >您可以直接在任務清單上進行進階指派。 按一下與工作同列的&#x200B;**工作總攬**&#x200B;欄位，然後按一下清單底部的&#x200B;**進階**，或工作總攬方塊右上角的&#x200B;**人員圖示**，以開啟「進階工作總攬」視窗。 跳到步驟5以繼續建立進階工作分派。
   >![按一下[進階]或[人員]圖示](assets/access-aa-from-lists.png)

1. 在任務標題的&#x200B;**工作總攬**&#x200B;欄位中按一下&#x200B;**指派給**

   或

   如果任務已指派，請按一下其中一個指派名稱。

1. 按一下&#x200B;**進階**。

   ![按一下[進階]](assets/assignments-from-task-header-0825.png)

   「進階指定」視窗即會出現。

   ![進階指派視窗](assets/advanced-assignments-031826.png)

1. 視需要檢閱工作期間資訊。 這些欄位都是來自「進階工作總攬」的僅供檢視欄位，您可以在任務中更新它們。

   如需有關任務期間、期間型別、時間單位和計畫時數的資訊，請參閱[任務期間和期間型別概觀](/help/quicksilver/manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

   >[!NOTE]
   >
   >如果您要檢視的資料欄未顯示，您可以將其新增。 請參閱下方的[進階工作總攬]清單[上的](#add-and-remove-columns-on-the-advanced-assignments-list)新增及移除欄。

1. （選擇性）選取&#x200B;**小時**、**FTE**&#x200B;或&#x200B;**百分比**&#x200B;以檢視配置。

   您可以檢視在計畫時數中指派了多少使用者、以容量百分比表示，或以FTE （全職相當值，0-1比例）表示。 預設設定為「小時」。

   如需有關FTE的資訊，請參閱[設定資源管理喜好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

1. 按一下&#x200B;**新增列**&#x200B;以新增工作分派。

1. 按一下&#x200B;**受指派人**&#x200B;欄以新增使用者或團隊。 開始輸入使用者或團隊的名稱，然後按一下該名稱（當它出現在下拉式清單中時）。

   >[!NOTE]
   >
   >如果名稱包含特殊字元，您必須在搜尋欄位中包含特殊字元。

   當您新增具有主要工作角色的使用者時，就會填入&#x200B;**受指派人角色**。

   如果使用者將屬性指派給其設定檔，則屬性會填入任務指派中。

1. 若要在不認識將處理工作的使用者時新增工作角色，請按一下&#x200B;**受指派人角色**&#x200B;欄。 開始輸入工作角色的名稱，然後在名稱出現在下拉式清單中時按一下該名稱。

   >[!NOTE]
   >
   >如果名稱包含特殊字元，您必須在搜尋欄位中包含特殊字元。

   如果工作角色具有從專案費率卡指派的屬性，則會將屬性植入任務指派中。

   當您稍後使用「受託人」欄位指派使用者時，基本搜尋會遵循此演演算法：

   * 完全符合：工作角色和所有屬性
   * 部分符合：工作角色和部分屬性
   * 僅符合工作角色

   如需有關進階搜尋的資訊，請參閱本文中的[使用進階搜尋](#use-the-advanced-search)。

1. （選擇性）繼續將受指派人新增至新列，以將多個資源新增至工作。

   >[!TIP]
   >
   >* 您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。 每個任務最多允許200個受指派人。
   >
   >
   >* 新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。
   >使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
   >您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱[授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。
   >
   >
   >* 如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
   >   
   >   * 將工作專案重新指派給作用中的資源。
   >   * 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。

1. 若要將受指派人標示為工作擁有者，請選取該列的核取方塊，然後按一下「進階工作分派」視窗底部動作列中的&#x200B;**設定主要**。

   依預設，Workfront會將您指派給任務的第一個使用者或工作角色標示為擁有者或主要指派。 不能將團隊指定為任務的主要擁有者。

   如果未顯示任務的主要擁有者，您可以將&#x200B;**Is Primary**&#x200B;資料行新增至資料表。

   >[!IMPORTANT]
   >
   >根據您的Workfront管理員或群組管理員設定專案偏好設定的方式，當您有多個使用者指派至任務時，Workfront可能會使用任務擁有者的排程來計算任務的時間表。 如需有關多個任務受指派人的資訊，請參閱文章[指派任務](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users)中的[對工作角色、團隊和使用者的多個指派的考量事項](../../../manage-work/tasks/assign-tasks/assign-tasks.md)一節。

1. 請為&#x200B;**受指派人**&#x200B;欄中的每個使用者指定下列資訊：

   * （選擇性） **計費工作角色**：搜尋並選取此特定受指派人和工作的計費工作角色。

     計費工作角色僅用於此指派，不會自動套用至使用者的其他指派。 例如，使用者的主要職務角色為Designer，但在某項任務上，他們將會擔任高級Designer，而計費率應反映這一點。 用於計費的工作角色僅適用於使用者，並且不能用於其他工作角色。

     將計費工作角色套用至使用者指派時，可能會使用附加到計費工作角色的費率，而不是在計費和收入計算中的使用者或工作角色費率。

     也可以為使用者設定計費的專案層級工作角色，此值用於該專案上所有使用者的指派。

     如需詳細資訊，請參閱[設定工作角色以計費](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md)。

   * **配置**：當任務的期間型別為「簡單」時，請指定每個使用者或工作角色應指派給任務的小時數。 每位使用者的所有指派時數總和等於「進階指派」視窗頂端之&#x200B;**計畫時數**&#x200B;欄位中的數字。 在所有其他情況下，請指定您希望受分派者花在解決工作上的時間（或配置）百分比。

     >[!TIP]
     >
     >在您手動修改任務的指派分配後，任務的計畫時數可能會相應地更新。 請注意，您無法手動修改指派給任務的專案團隊的分配。 如需詳細資訊，請參閱文章[計畫時數概觀](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations)中的[管理使用者配置時更新任務計畫時數](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md)一節。

   * **屬性**：任何可供使用者使用的屬性都會顯示在屬性欄位中。 管理員會設定屬性，這些屬性會新增至使用者設定檔，或與費率卡中的工作角色相關聯。 如需詳細資訊，請參閱[定義費率屬性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)和[編輯使用者的設定檔](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

     屬性目前在使用者指派上是唯讀的。 它們可供職務角色編輯。

   * **匯率貨幣**：帳單和成本匯率的貨幣預設自專案，但您可以變更此指派的貨幣。

   * （選擇性） **收費率**：收費率可能來自系統的其他區域，例如費率卡。 如需詳細資訊，請參閱[收入與成本階層概覽](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。 您可以在此欄位中手動覆寫此特定指派的收費率，它將在收入計算中覆寫使用者的所有其他費率。
   * （選擇性） **成本費率**：成本費率可能來自系統的其他區域。 如需詳細資訊，請參閱[收入與成本階層概覽](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。 您可以在此欄位中手動修訂此特定指定的成本費率，它將會在成本計算中修訂使用者的所有其他費率。
   * **可記帳**：選取此選項可將指派納入財務計算。 清除此選項可排除財務計算中的指派。

     當任務具有收入型別時，預設會針對所有指派開啟此欄位。

1. （選擇性）若要依日期檢視使用者或角色的指派資料，請選取表格列，然後按一下「進階指派」視窗底部動作列中的&#x200B;**依日期檢視**。 如需詳細資訊，請參閱本文中的[依日期檢視指派資料](#view-assignment-data-by-dates)。
1. （選擇性）若要從清單中刪除一或多個指派，請選取每一列的核取方塊，然後按一下[進階指派]視窗底部動作列中的&#x200B;**刪除**。
1. 完成編輯進階工作分派時，按一下&#x200B;**儲存**&#x200B;或&#x200B;**儲存並關閉**。

### 新增和移除進階指派清單上的欄

欄位必須先存在，您才能將其新增至清單。

1. 按一下清單右上角的&#x200B;**+**&#x200B;以開啟&#x200B;**資料行管理員**。

   ![進階工作分派資料行管理員](assets/aa-column-manager.png)

1. 選取&#x200B;**屬性**&#x200B;標籤或&#x200B;**KPI**&#x200B;標籤，以選擇要新增的欄位型別。

   位置或成本中心等屬性會提供內容相關資訊。 時間分段KPI，例如跨期間的收入或成本細分值。

1. 在&#x200B;**可用**&#x200B;區段中搜尋現有的物件欄位，然後按一下欄位名稱右側的&#x200B;**+**，將其新增至&#x200B;**已選取**&#x200B;欄。
1. 按一下&#x200B;**已選取**&#x200B;區段中欄位右側的&#x200B;**-**，將其從清單中移除。
1. 按一下「**儲存**」。

   如需資料行管理員的詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

### 將檢視套用至「進階工作總攬」清單

檢視表是一組可套用至清單的個人化欄位安排。

1. 按一下&#x200B;**檢視**&#x200B;下拉式清單，然後選取您要套用至清單的檢視。

   **系統檢視**&#x200B;是系統管理員新增的檢視，無法變更。 **我的檢視**&#x200B;是您建立或與您共用的檢視。

1. 按一下&#x200B;**檢視**&#x200B;下拉式清單中的&#x200B;**新檢視**&#x200B;以建立檢視。

   當您新增、移除或重新排序欄時，變更會自動儲存到檢視中。 下次套用此檢視時，欄會保持設定的方式。

   如需檢視的詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

### 使用進階搜尋

進階搜尋可協助您找出要新增至指派的正確使用者或工作角色。

1. 若要開啟進階搜尋視窗，請執行下列任一項作業：

   * 按一下「進階指派」視窗右上角的&#x200B;**進階搜尋**。
   * 選取工作分派列，然後按一下[進階工作分派]視窗底部動作列中的&#x200B;**進階搜尋**。 這會開啟進階搜尋，並針對該特定指派自動套用篩選器。

1. 在進階搜尋視窗中選取使用者或工作角色標籤。
1. 視需要套用篩選器：

   1. 按一下清單上方的&#x200B;**篩選器**。
   1. 在[篩選]方塊中，按一下[**新增條件**]。
   1. 選取欄位作為篩選依據。
   1. 選取篩選修飾元，例如「具有任何」、「不具有任何」、「早於」或「晚於」。 修正因子選項會因您篩選的欄位型別而異。
   1. 選取一或多個欄位值。 根據您篩選的欄位型別，系統可能會提示您從清單中選取專案、搜尋專案，或使用日曆來選取日期範圍。

   篩選器會自動套用至清單。 如需篩選的詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

1. 搜尋工作角色或使用者。

   搜尋符合工作角色指派的使用者時，只會顯示完全符合專案（工作角色和所有屬性）。

1. 按一下&#x200B;**+**&#x200B;以新增資料行至資料表。 如需詳細資訊，請參閱[在進階工作分派清單](#add-and-remove-columns-on-the-advanced-assignments-list)上新增及移除欄。
1. 選取一或多個使用者或工作角色，然後按一下視窗底部動作列中的&#x200B;**新增使用者**&#x200B;或&#x200B;**新增角色**。

   這些指定會新增至「進階指定」視窗中。

### 依日期檢視指派資料

進階指派的&#x200B;**依日期檢視**&#x200B;視窗會顯示特定使用者或角色指派的完整日期有效歷史記錄。 過去和未來的變更都會顯示。

日期有效專案可能會影響指定歷史記錄，其範例為：

* 使用者的主要/其他職位角色
* 計費的專案層級工作角色
* 使用者設定檔計費/成本費率
* 專案覆寫計費/成本費率（使用者或工作角色）
* 依工作角色/屬性評定卡片費率
* 使用者屬性
* 使用者排程

請注意，這不是一個完整的清單，而且變更的欄位不一定顯示在指派資料表中，但是它會影響使用者或工作角色的帳單和成本費率或屬性。

您只能依日期檢視單一使用者或角色的指派資料。

1. 選取使用者或角色的表格列，然後按一下「進階工作總攬」視窗底部動作列中的&#x200B;**依日期檢視**。

   **依日期檢視**&#x200B;視窗會出現。 資料是唯讀的。

   表格中的每一列代表指定專案的日期有效變更。 如果沒有發生日期有效的變更，表格會有一列顯示目前的資料。 反白顯示的欄位指出已變更的專案，並列出每個更新的開始和結束日期。 例如，如果計費率從8月20日的202變更為8月21日的205，則會醒目顯示費率。 括弧內的文字表示對費率進行變更的位置，例如專案。

   ![依日期視窗檢視](assets/resource-changes-view-by-dates.png)

   檢閱完資料後，按一下左上方的箭頭以返回「進階工作總攬」視窗。

## 建立進階任務指派 — 所有其他套件

此「進階任務指派」配置會同時套用至任務和問題。

1. 前往您要指派任務或問題的專案。
1. 按一下左側面板中的&#x200B;**任務**&#x200B;或&#x200B;**問題**，然後按一下清單中任務或問題的名稱。

   >[!TIP]
   >
   >您可以直接在任務或問題清單上進行進階指派。 按一下與任務或問題同列的&#x200B;**工作總攬**&#x200B;欄位，然後按一下清單底部的&#x200B;**進階**，或工作總攬方塊右上角的&#x200B;**人員圖示**，以開啟「進階工作總攬」視窗。 跳到步驟5以繼續建立進階工作分派。
   >![按一下[進階]或[人員]圖示](assets/access-aa-from-lists.png)

1. 按一下任務或問題標題中&#x200B;**工作總攬**&#x200B;欄位中的&#x200B;**指派給**

   或

   如果任務或問題已指派，請按一下其中一個指派的名稱。

1. 按一下&#x200B;**進階**。

   ![按一下[進階]](assets/assignments-from-task-header-0825.png)

1. 在&#x200B;**搜尋人員、角色和團隊**&#x200B;欄位中，開始輸入使用者、角色或團隊的名稱，然後在其出現在下拉式清單中時按一下該名稱。

   >[!NOTE]
   >
   >如果使用者名稱包含特殊字元，您必須在搜尋欄位中包含特殊字元。

1. （選擇性）繼續在&#x200B;**搜尋人員、角色和團隊**&#x200B;方塊中新增受指派人，以將多個資源新增至任務或問題。

   >[!TIP]
   >
   >* 您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
   >
   >
   >* 新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。
   >使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
   >您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱[授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。
   >
   >
   >* 如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
   >   
   >   * 將工作專案重新指派給作用中的資源。
   >   * 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。

1. 請為&#x200B;**受指派人**&#x200B;欄中的每個使用者指定下列資訊：

   * **所有者**：將游標停留在受指派人名稱上，如果要將受指派人標示為任務或問題所有者，請在「所有者」欄位中按一下&#x200B;**設為主要所有者**。 綠色核取方塊表示指定的使用者是任務或問題的主要聯絡人。 Adobe Workfront將您指派給任務或問題的第一個使用者或工作角色標籤為擁有者或主要指派。 團隊不能被指定為任務或問題的主要擁有者。

     >[!IMPORTANT]
     >
     >根據您的Workfront管理員或群組管理員設定專案偏好設定的方式，當您有多個使用者指派至任務時，Workfront可能會使用任務擁有者的排程來計算任務的時間表。 如需有關多個任務受指派人的資訊，請參閱文章[指派任務](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users)中的[對工作角色、團隊和使用者的多個指派的考量事項](../../../manage-work/tasks/assign-tasks/assign-tasks.md)一節。

   * **配置**：當任務的期間型別為「簡單」時，請指定每個使用者或工作角色應指派給任務的小時數。 每位使用者所有指派時數的加總等於分配欄底部&#x200B;**計畫時數**&#x200B;欄位中的數字。 在所有其他情況下，請指定您希望受分派者解決任務或問題的時間百分比（或配置）。

     >[!TIP]
     >   
     >   * 在您手動修改任務的指派分配後，任務的計畫時數可能會相應地更新。 如需詳細資訊，請參閱文章[計畫時數概觀](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations)中的[管理使用者配置時更新任務計畫時數](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md)一節。
     >   * 您無法手動修改問題的指派分配。
     >   * 您無法手動修改指派給任務的專案團隊的分配。

   * **受指派人角色：**&#x200B;選取使用者完成此指派時應使用的角色。  預設會顯示使用者的主要角色。 按一下&#x200B;**受指派人角色**&#x200B;方塊以選取其他角色。 當您先將任務或問題指派給角色，然後新增可以履行該角色的使用者作為第二個指派時，將會篩選建議使用者的清單，以顯示可以履行已指派給任務和問題的角色的使用者。

     ![受指派人的角色](assets/advanced-assignments-select-role.png)

   * **期間型別**：這僅適用於工作。 按一下「持續時間型別」的名稱，然後從下拉式選單中選取「持續時間型別」。 如需有關期間型別的資訊，請參閱[任務期間與期間型別的概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

   * **工期：**&#x200B;當您擁有任務的管理許可權時，可以更新任務的此欄位。

     如需詳細資訊，請參閱[任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。 大量編輯指派資訊時，會出現類似的對話方塊，以指派使用者、時數、配置和任務擁有者。

   * **計畫時數**：當期間型別為計算指派或簡單時，更新計畫時數。 因此，每個資源的配置百分比或時數會平均分配。 當期間型別為已計算的工作或投入比導向時，Workfront會計算計畫時數。 如需詳細資訊，請參閱[任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

1. 按一下「**儲存**」。


