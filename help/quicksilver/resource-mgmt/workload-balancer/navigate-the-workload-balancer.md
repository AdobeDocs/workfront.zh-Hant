---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 導航工作負載平衡器
description: 使用工作負載平衡器了解資源的可用性，並將工作分配給用戶。 本文將使用可用於更新視圖的表徵圖和設定，引導您完成工作負載平衡器的更新和導航。
author: Alina
feature: Resource Management
exl-id: 60dabfc5-6a2e-4368-9dac-db48d0307895
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '4050'
ht-degree: 0%

---

# 導航工作負載平衡器

使用Adobe Workfront中的工作負載平衡器，根據用戶的可用性為用戶分配工作。 本文介紹如何使用設定和選項來導航工作負載平衡器，並顯示與您相關的資訊。 此處列出的其他文章介紹了如何使用工作負載平衡器管理資源及其分配以正常工作。

工作負載平衡器可用於Adobe Workfront的多個區域。 在所有區域中導覽都類似。

有關工作負載平衡器所在位置的詳細資訊，請參見 [找到工作負載平衡器](https://experienceleague.adobe.com/docs/workfront/using/manage-resources/the-workload-balancer/locate-workload-balancer.html?lang=en).


## 存取需求

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
<td><p>Current license: Standard </p>
    Or 
<p>Legacy license:</p>
    <ul>
    <li><p>Plan, when using the Workload Balancer for a team or in the Resourcing area </p></li>
    <li><p>Work, when using the Workload Balancer of a project </p></li>
    </ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>在使用團隊或「資源配置」區域中的工作負載平衡器時進行計畫 </p>
   <p>使用項目的工作負載平衡器時工作 </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視或更高存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案、工作和問題的權限或更高權限 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。


## 在工作負載平衡器中查看項的考量事項

查看工作負載平衡器時，請考慮以下事項：

* 工作負載平衡器將根據工作項的分配在兩個不同的區域中顯示工作項。 工作項和用戶顯示在以下區域：

   * **未分配的工作**:沒有分配或僅分配給作業角色或團隊的項目。
   * **已分配的工作**:指派給至少一個使用者的項目。 指派的項目會顯示在指派的使用者名稱下方。

   >[!NOTE]
   >
   >* 分配給職務角色的項目或分配給作為主要受託人的用戶的團隊不會顯示在「未分配的工作」區域中。
   >
   >* 分配給用戶的項目和作業角色，其中作業角色被選擇為項目的主要受分配者時，「未分配的工作」區域中將顯示該項目。
   >* 分配給多個用戶的項目將顯示在「已分配的工作」區域中所有用戶的名稱下。


* 當專案在一段時間內沒有任務時，專案層級的長條會變成灰色。

   ![](assets/wb-break-in-project-timeline-with-no-tasks-highlight-350x80.png)

* 當您沒有查看特定項目的權限時，這些項目會顯示為 **無法訪問的工作項** 或 **無法訪問的項目**.

   ![](assets/balancer-inaccessible-items-and-projects-highlighted-350x108.png)

* 工作項的名稱顯示在左側，其時間軸顯示在右側。
* 每個工作項的總計計畫小時數顯示在工作項名稱的右側，以及表示工作項時間表的欄的左側。
* 每個項目的「計畫時數」合計顯示在項目名稱的右側和表示項目時間表的欄的左側。

   項目的「計畫小時數」資訊是「工作負載平衡器」中列出的所有項的「計畫小時數」合計，而不是項目的「計畫小時數」合計。

有關在工作負載平衡器中查看資訊的詳細資訊，另請參閱以下文章：

* [找到工作負載平衡器](../workload-balancer/locate-workload-balancer.md)
* [篩選工作負載平衡器中的資訊](../workload-balancer/filter-information-workload-balancer.md)
* [使用連結共用工作負載平衡器](../workload-balancer/share-link-for-workload-balancer.md)
* [使用「摘要」更新工作負載平衡器中的工作項](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)

有關使用工作負載平衡器管理資源的資訊，另請參閱以下文章：

* [工作負載平衡器中分配工作的概述](https://experienceleague.adobe.com/docs/workfront/using/manage-resources/the-workload-balancer/assign-work-in-workload-balancer.html?lang=en)
* [在工作負載平衡器中管理用戶分配](https://experienceleague.adobe.com/docs/workfront/using/manage-resources/the-workload-balancer/manage-user-allocations-workload-balancer.html?lang=en)


## 在「資源配置」區域中導航多個項目的工作負載平衡器

在您訪問工作負載平衡器的所有區域中，導航都類似。

以下子部分介紹如何在工作負載平衡器中查看多個項目的資訊。

您可以調整工作負載平衡器中的一些設定和選項，以顯示在對您最有意義的時間範圍內需要關注的資訊。

選擇要應用到視圖的設定後，工作負載平衡器會在每次從任何瀏覽器或設備訪問時記住這些設定。

### 訪問資源區中多個項目的工作負載平衡器

要導航多個項目的工作負載平衡器，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **資源**.
1. 按一下 **工作負載平衡器** 中。

   ![](assets/nwe-balancer-global.png)

   工作負載平衡器在以下兩個區域顯示從當前周開始的工作分配資訊：

   * 此 **未分配的工作** 區域顯示以下工作項：

      * 指派給角色、團隊或未指派的工作項目（任務和問題）會在您套用篩選器後顯示。
預設情況下，「未分配的工作」區域不顯示任何工作項。 建議您使用篩選器來顯示此區域的相關資訊。

         如需使用篩選器的相關資訊，請參閱 [篩選工作負載平衡器中的資訊](../workload-balancer/filter-information-workload-balancer.md).

      * 只有在啟用「依專案分組」設定時，才會顯示專案。 如需詳細資訊，請參閱 [自訂檢視](#customize-the-view) 這篇文章。
   * 此 **已分配的工作** 區域顯示以下工作項：

      * 預設情況下，系統中所有活動用戶都顯示在此區域。 建議您使用篩選器來限制此區域的資訊量。 如果將用戶分配給項目，則工作項目也會以其名稱顯示。

      * 指派給至少一個使用者的任務和問題會顯示在使用者名稱下方。

         在「已分配的工作」區域中，用戶名下的工作項按以下標準按以下順序排序：

         1. 計劃開始日期（最舊優先）
         1. 計畫完成日期（最舊優先）
         1. 按項目字母順序（僅當前兩個條件對多個工作項相同時）

            >[!TIP]
            >
            >* 您可以從「依」設定中選取選項，以自訂專案排序。
            >
            >* 只有在啟用「依專案分組」設定時，才會顯示專案。

            > 
            >如需自訂設定的詳細資訊，請參閱 [自訂檢視](#customize-the-view) 這篇文章。


1. （選用）按一下 **篩選** 圖示 ![](assets/filter-icon.png) 在 **已分配的工作** 區域，然後選取 **預設篩選** 在 **建議** 框中。

   套用預設篩選時，會顯示屬於您任何團隊的使用者及其工作項目。 您可以編輯此篩選器的復本。

   >[!TIP]
   >
   >預設篩選器僅在資源區的工作負載平衡器中可用。

1. 繼續執行以下步驟以導航工作負載平衡器：

   * [在工作負載平衡器中選擇時間範圍](#select-a-time-frame-in-the-workload-balancer)
   * [自訂檢視](#customize-the-view)
   * [分配工作項並調整用戶分配](#assign-work-items-and-adjust-user-allocations)
   * [在圖表中查看分配](#view-allocations-in-a-chart)

### 在工作負載平衡器中選擇時間範圍

1. 訪問 **資源** 區域，如一節中所述 [訪問資源區中多個項目的工作負載平衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) 這篇文章。

   工作負載平衡器顯示從當周開始的工作分配資訊。

1. 使用水準捲動查看超出螢幕限制的工作項的時間軸。
1. 按一下 **後退** 表徵圖 ![](assets/back-and-forward-icons.png) 在左上角以導覽時間軸，然後按一下 **今天** 返回當周。
1. 按一下 **時間範圍下拉式選單** 在工具列上，然後按一下您要顯示的期間的開始日期。 依預設，日曆上選取的第一週是您導覽至的一週。

   ![](assets/calendar-date-picker-wb.png)

1. 從以下選項中選擇要在工作負載平衡器中一次顯示的周數：
   * 1 週
   * 2 週
   * 4 週. 這是預設設定。
   * 6 週
   * 3 個月

   ![](assets/3-months-12-weeks-drop-down-wb.png)

1. 在工具列中按一下下列其中一個選項，即可依不同時間範圍顯示資訊：
   * **日**:預設情況下，按日顯示從今天日期開始的四周資訊。
   * **周**:按周顯示4週的資訊。
   * **月**:依月份顯示三個月的資訊。

1. 按以下各節所述繼續導航工作負載平衡器。

### 自訂檢視

1. 訪問 **資源** 區域，如一節中所述 [訪問資源區中多個項目的工作負載平衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) 這篇文章。

   工作項的名稱在左側列出，並由工作負載平衡器右側的條形表示。 長條表示工作項的時間軸。

1. （可選和建議）在「未分配」和「已分配」工作區中使用篩選器，以僅顯示與您相關的工作項或用戶。

   如需詳細資訊，請參閱 [篩選工作負載平衡器中的資訊](../workload-balancer/filter-information-workload-balancer.md).

   依預設，藍色長條代表專案和任務的時間軸，而長條代表問題。

   當您選取顏色主題以符合專案時，可以變更專案和工作的長條顏色。 如需詳細資訊，請繼續閱讀此程式。

   「分配的工作」區域中的工作項目按以下標準按以下順序按項目排序：
   1. 計劃開始日期（最舊優先）
   1. 計畫完成日期（最舊優先）
   1. 按項目字母順序（僅當前兩個條件對多個工作項相同時）

1. 按一下 **右箭頭** 「未分配」或「已分配」區域的左側，以展開項目名稱下（在「未分配」區域）和用戶名下（在「已分配」區域）的所有項。

   >[!TIP]
   >
   >僅當啟用「按項目分組」設定時，才會在「未分配」區域的項目名稱下列出工作項。


1. 按一下 **向下箭頭** 在「未分配」或「已分配」區域的左側，折疊項目名稱下（在「未分配」區域）和用戶名下（在「已分配」區域）的所有項。

1. 拖放 **分離線** 在左面板和時間軸區域之間，以調整左面板的大小。

   ![](assets/separation-line-between-left-panel-and-timeline-highlighted-nwe-350x174.png)

1. 按一下 **設定** 圖示 ![](assets/settings-gear-icon.png).

   「設定」面板會顯示在右側。

   ![](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   從下面列出的選項中選擇，以更新您在工作負載平衡器中查看的資訊，然後按一下 **X圖示** 在「設定」方塊的右上方，以關閉它。

   * **按項目分組**:選中此選項後，「未分配」和「已分配」工作區中的項目將按項目分組。 預設會選取此選項。

   * **包括來自問題的小時數**:選中此選項後，分配給用戶的問題將顯示在「已分配的工作」區域的用戶名下，而未分配給用戶的問題將顯示在「未分配的工作」區域中。 從問題開始的計畫小時數會計入項目和「已分配工作」區域中用戶的計畫小時數。
   * **顯示預計日期**:選擇此選項時，除了計畫時間線外，還會顯示工作項的預計時間線。 請注意下列事項：
      * 項目、任務和問題的預計時間軸顯示為任務、問題和項目欄上方的深藍線。
      * 即使您更新顏色主題，計畫時間軸外的投影時間軸仍以淺藍色顯示，如下所述。
      * 您無權查看的項目的投影時間線以淺灰色顯示，下面有一行。
      * 當任務或問題在到期計畫完成日期之前完成時，系統會完成剩餘天數的分配編號，不會計入用戶的分配。 只有在同時啟用「顯示預計日期」設定和「顯示分配」圖示時，才會顯示此選項。

      >[!TIP]
      >
      >請注意，當工作項的計畫時間表或預計時間表（不一定同時發生）在選定的時間範圍內時，工作項將顯示在工作負載平衡器中。

   * **顯示已完成的工作**:啟用此功能後，已完成的任務和問題將顯示在「已分配的工作」區域中。 預設會啟用。

      完成任務或問題列後，右上角會顯示綠色的核取標籤圖示。 項目的所選時間範圍的任務或問題完成時，將顯示同一表徵圖。
   * **顯示剩餘時間**:啟用此功能後，Workfront會顯示使用者根據其排程可供工作的每日時間，與使用者在「已指派工作」區域中被分配的小時數之間的差異。 預設會停用，而配置的時間預設會顯示。
   * 在 **選擇顏色主題** 部分，選擇項目和任務欄所需的顏色。

      >[!TIP]
      >
      >選擇顏色主題的設定不會影響問題欄的顏色。 問題一律會以紅色列顯示。

      從以下項目中選取：
      * **預設**:所有專案及其工作項目的長條會以藍色顯示。
      * **專案**:與每個專案及其工作相關聯的列會根據專案名稱而變更。 屬於專案的所有工作會以符合專案顏色的列顯示。 專案列會以較淺的陰影顯示，以區分它們與工作。 選擇不顯示分配時，項目欄也包含項目表徵圖。
      * **專案狀態**:與每個項目及其工作項相關聯的條將更改為項目狀態的顏色。

         項目狀態是與項目組關聯的項目狀態。 如果組沒有特定於組的狀態，則工作項條的顏色為系統級項目狀態的顏色。 系統和自訂狀態都會顯示。 有關組狀態的資訊，請參閱 [建立或編輯群組狀態](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
   * 在 **在** ，請從以下項中選擇：
      * **小時**:將分配的時間顯示為小時。 這是預設值。
      * **百分比**:以可用總時間的百分比顯示已分配時間
   * 在 **排序偏好設定** 節，選擇要如何在工作負載平衡器中排序項。 從下列選項中選取：
      * **按主要角色對用戶進行排序**:用戶在「已分配的工作」區域中按其主要角色的字母順序顯示。
      * **依字母排序使用者**:用戶在「已分配的工作」區域中按字母順序顯示其名字。
      * **依排序專案**:從下拉菜單中選擇一個項目欄位，以按「未分配」或「已分配」工作區中的欄位按字母順序排序項目。

   >[!TIP]
   >
   >只有啟用「依專案分組」設定時，才可依專案排序。 否則，此設定會呈暗灰色。

1. （可選和條件性）當您將顏色主題變更為「專案狀態」時，將滑鼠指標暫留在左側的專案名稱上，即可檢視專案的狀態。

   ![](assets/hover-over-project-status-tooltip-350x115.png)

### 分配工作項並調整用戶分配

1. 訪問資源區中的工作負載平衡器，如一節中所述 [訪問資源區中多個項目的工作負載平衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) 這篇文章。
1. 按一下 **顯示分配表徵圖** ![](assets/show-allocations-icon-small.png) 查看工作項的每日或每週計畫小時數。

   這將用「未分配」和「已分配」工作區中的每日或每週計畫小時數量替換工作項欄中的名稱。 預設會停用此設定。

   顯示超額分配的天數會以紅色顯示。

   >[!TIP]
   >
   >* 「顯示分配」選項只會影響項目、任務、問題和不可訪問項的顯示內容。 使用者的「每日計畫時數」預設會顯示，且無法隱藏。
   >* 您必須啟用「按項目分組」設定，以顯示項目的每日計畫時數。
   >* 按周查看工作負載平衡器時，顯示的小時數為每週計畫小時數。



1. （選用）將滑鼠指標暫留在使用者行中已分配的時間上，以了解使用者的容量和配置。 容量是用戶根據其時間表的可用性。

   ![](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. （選用）按一下 **隱藏分配表徵圖** ![](assets/show-allocations-icon-small.png) 在工作項的欄中顯示任務和問題的名稱。
1. 按一下 **更多功能表** 圖示 ![](assets/more-icon.png) 在任務或問題名稱的右側，然後按一下以下選項之一。

   ![](assets/more-menu-right-of-task-350x104.png)

   * **將此項指派給**，然後開始鍵入要在 **搜索人員、角色或團隊** 欄位。

      您也可以使用下列捷徑來指派工作或問題：

      * 在Windows中：按住CTRL鍵並按一下任務或問題欄。
      * 在Mac:按住CMD鍵並按一下任務或問題欄。

      有關在工作負載平衡器中為用戶分配工作項的詳細資訊，請參見 [工作負載平衡器中分配工作的概述](../workload-balancer/assign-work-in-workload-balancer.md).

      >[!TIP]
      >
      >如果您的Workfront或組管理員在您的環境中啟用了委託，請使用「指配」頁簽將用戶分配給該任務或問題。 有關委派工作的資訊，請參見 [管理任務和問題委派](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **編輯分配**，然後編輯使用者的每日或每週分配。 有關管理用戶分配的資訊，請參閱 [在工作負載平衡器中管理用戶分配](../workload-balancer/manage-user-allocations-workload-balancer.md).

   * **開啟摘要**. 將開啟右側的「摘要」面板，然後按一下「工作總攬」欄位，然後開始鍵入 **搜索人員、角色或團隊** 欄位來指派項目。 如需詳細資訊，請參閱 [顯示有關任務和問題的更多資訊](#display-more-information-about-tasks-and-issues) 這篇文章。


1. （可選）按兩下工作項目欄內使用者的每日或每週分配，以編輯已分配的小時數，然後按一下 **儲存** 圖示 ![](assets/save-allocations-wb.png) 保存分配或 **取消** 圖示  ![](assets/cancel-allocations-wb.png) 刪除您調整的分配。

   >[!TIP]
   >
   >「儲存」和「取消」圖示會顯示在任務或問題時間軸列的結尾處。
   >
   >![](assets/cancel-and-save-icon-on-adjust-allocation-bar-wb-highlighted.png)

   有關管理用戶分配的資訊，請參閱 [在工作負載平衡器中管理用戶分配](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. 按一下 **大量指派** 來大量指派工作項目。

   如需詳細資訊，請參閱 [使用工作負載平衡器批量分配工作](../workload-balancer/assign-work-in-workload-balancer-in-bulk.md).
1. 從拖曳項目 **未分配的工作** 區域或來自使用者，並將它們拖放至其他使用者以指派。

   如需詳細資訊，請參閱 [通過拖放來分配工作負載平衡器中的工作](../workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).


### 在圖表中查看分配

您可以在圖表中查看分配，而不是以每日或每週數字查看分配。

1. 訪問資源區中的工作負載平衡器，如一節中所述 [訪問資源區中多個項目的工作負載平衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) 這篇文章。
1. 按一下 **圖表圖示** ![](assets/user-allocation-chart-icon.png) 以圖表格式顯示用戶配置。

   用戶被過度分配的天數顯示為紅色塊，用戶被分配不足的天數或容量顯示為藍色塊。

   區塊的大小表示分配的量：框越大，則分配給該日或周的工作項的時間就越多。

   ![](assets/user-allocation-chart-350x237.png)



### 顯示有關任務和問題的更多資訊

您可以在工作負載平衡器中查看有關任務和問題的詳細資訊。


1. 訪問資源區中的工作負載平衡器，如一節中所述 [訪問資源區中多個項目的工作負載平衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) 這篇文章。
1. 要在「摘要」面板中查看更多資訊，請執行以下操作之一：

   * 按一下任務或問題的欄以開啟右側的「摘要」面板。
   * 按一下 **開啟摘要** 圖示 ![](assets/summary-panel-icon.png)，然後按一下任務或問題的列以開啟「摘要」面板。
   * 按一下 **更多** 功能表，然後按一下 **開啟摘要**.

   有關在工作負載平衡器的摘要中更新任務資訊的資訊，請參見 [使用「摘要」更新工作負載平衡器中的工作項](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

1. 將滑鼠指標暫留在任務或問題的名稱上，以檢視其相關資訊。 任務或問題上方會顯示一個方塊，其中包含下列資訊：

   * 任務或問題的名稱。
   * 專案的名稱。
   * 計畫的開始和完成日期。
   * 計畫小時數。
   * 對於任務，為前置編號。
   * 對於任務，框的上角指示任務是否準備好工作的指示器。

   ![](assets/task-bar-hover-over-detail-wb.png)

1. 按一下左側工作項的名稱以訪問它。 工作項目會在新的瀏覽器標籤中開啟。


### 全螢幕顯示工作負載平衡器

1. 訪問資源區中的工作負載平衡器，如一節中所述 [訪問資源區中多個項目的工作負載平衡器](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) 這篇文章。

1. 按一下 **全螢幕** 圖示 ![](assets/full-screen.png) 以全螢幕顯示工作負載平衡器。

   工作負載平衡器佔據整個螢幕。 瀏覽器視窗和標籤會從檢視中排除。

1. 按一下 **全螢幕退出** 圖示 ![](assets/exit-full-screen.png) 返回預設螢幕並在瀏覽器頁簽內查看工作負載平衡器。


## 導航團隊的工作負載平衡器

導航團隊的工作負載平衡器與導航多個項目的工作負載平衡器類似。 如需詳細資訊，請參閱 [導航多個項目的工作負載平衡器](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) 這篇文章。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下 **團隊**.
預設會顯示您的「首頁團隊」頁面。
1. 按一下 **工作負載平衡器** 中。 預設情況下，應顯示組的工作負載平衡器。

   ![](assets/nwe-balancer-team-350x172.png)

   組的工作負載平衡器預設顯示以下資訊：

   * 在 **未分配的工作** 區域：分配給團隊或團隊和作業角色的工作項，以及未分配給用戶的工作項。
   * 在 **已分配的工作** 區域：分配給用戶的工作項將顯示在用戶名下。

1. 按照 [在「資源配置」區域中導航多個項目的工作負載平衡器](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) 本文的一節。

## 導航單個項目的工作負載平衡器

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下 **專案**.
1. 按一下專案名稱以開啟專案頁面。
1. 按一下 **工作負載平衡器** 中。 您可能必須按一下 **顯示更多**，然後 **工作負載平衡器**.

   ![](assets/nwe-balancer-project-350x152.png)

   項目的工作負載平衡器預設顯示以下資訊：

   * 在 **未分配的工作** 區域：指派給角色或團隊且未指派給使用者的專案工作項目。
   * 在 **已分配的工作** 區域：指派給至少一個使用者的專案上的工作項目。

   建議您使用篩選條件，只顯示對您而言重要的使用者。

   例如，您可以考慮只顯示屬於您的團隊或群組的使用者。 如需詳細資訊，請參閱 [篩選工作負載平衡器中的資訊](../workload-balancer/filter-information-workload-balancer.md).

1. （選用）按一下 **篩選** 圖示 ![](assets/filter-icon.png) 在「已分配的工作」(Assigned Work)區域中，並選擇 **此項目的工作項** 選項 **建議** 的下一頁。 預設會取消選取此篩選器。

   選取此選項時，只會顯示所選專案中指派給使用者的項目。

   未選取選項時，會顯示專案上指派給使用者的所有項目，而無論項目屬於哪個專案。

1. （可選，建議使用）在「已分配的工作」區域中套用篩選器，以顯示對您來說很重要但可能未指派給專案項目的使用者，然後按一下 **顯示所有用戶** 圖示 ![](assets/show-all-users-icon-project-workload-balancer.png).

   透過顯示所有使用者，您可以顯示Workfront中尚未指派給專案工作或其他角色的所有使用者。

   您可以先套用篩選，減少顯示的使用者人數。

   例如，您可能想要先篩選屬於您的團隊或群組的使用者，然後顯示所有這些使用者。

   如需如何建立篩選器的相關資訊，請參閱 [篩選工作負載平衡器中的資訊](../workload-balancer/filter-information-workload-balancer.md).

   >[!NOTE]
   >
   > 「顯示所有用戶」選項僅對項目的工作負載平衡器可用。


1. （選用）按一下 **顯示角色分配** 圖示 ![](assets/show-role-allocation-icon.png).

   「角色分配」面板隨即顯示。

   您可以查看與項目上的任務職責關聯的計畫小時數資訊，以及與從方案計畫器連結到項目的方案關聯的計畫職責相關的任務職責。

   如需詳細資訊，請參閱 [協調項目和舉措之間資源分配的概覽](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).


   >[!NOTE]
   >
   >如果您的組織尚未為Workfront方案計畫員購買許可證，則無法查看方案任務職責資訊。 在這種情況下，您只能查看與項目上的職務角色關聯的計畫小時數。 如需詳細資訊，請參閱 [使用方案計畫員所需的訪問權限](../../scenario-planner/access-needed-to-use-sp.md).


1. 繼續導航項目的工作負載平衡器，如 [導航多個項目的工作負載平衡器](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) 本文的一節。

<!--old content below - this used to be a one-large-procedure article - outdated, and rewrote it above with several smaller procedures: 

# Navigate the Workload Balancer

<!-drafted note for 22.4 release: remove all production/ preview references at Prod release>

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

Use the Workload Balancer to understand the availability of your resources as well as to assign work to your users. This article walks you through using the icons and settings available to update the view for and navigate the Workload Balancer.

>[!NOTE]
>
>The Workload Balancer is a resource scheduling tool that will eventually replace the current resource scheduling tools which are currently deprecated. 
>
>For more information about removing the resource scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).
>
>We recommend that you use the Workload Balancer for scheduling your resources.

The Workload Balancer is available in multiple areas of Adobe Workfront. Navigating it is similar in all areas. This article describes how to navigate the Workload Balancer for multiple projects in the Resourcing area. For more information about where the Workload Balancer is located, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

For information about managing resources using the Workload Balancer, also consider reading the following articles:

* [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
* [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, when using the Workload Balancer in all areas in the Production environment</p>
   <p><span class="preview">Work, when using the Workload Balancer of a project, in the Preview environment</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for viewing items in the Workload Balancer

Consider the following when viewing the Workload Balancer:

* Projects display in the Workload Balancer only when the Group by Project setting is enabled. This setting is enabled by default.
* Mousing over a task or an issue displays the following additional information about the task or issue:

  * Project name

  * Task or issue name

  * Parent task

  * Planned Start and Completion Dates

  * Number of Planned Hours

  * Ready to start or Not ready status

  ![task-pop-up-with-additional-info-in-workload-balancer](assets/task-pop-up-with-additional-info-in-global-wb.png)

* When a project has no tasks during a period of time, the bar at the project level becomes a dimmed color.

  ![](assets/wb-break-in-project-timeline-with-no-tasks-highlight-350x80.png)

* When you don't have permissions to see certain items, they display as **Inaccessible work items** or **Inaccessible projects**.

  ![](assets/balancer-inaccessible-items-and-projects-highlighted-350x108.png)

* The names of the work items display on the left and within the timeline selected on the right. 
* The total of Planned Hours for each work item displays to the right of the name of the work items on the left. 
* The total of the Planned Hours for each project displays to the right of the name of the project on the left.

  The Planned Hours information for the project is a total of Planned Hours from all items listed in the Workload Balancer, and not a total of Planned Hours on the project.

## Overview of the Unassigned Work and Assigned Work areas

The Workload Balancer displays work items in two separate areas, depending on their assignments.

The two areas of the Workload Balancer display the following information:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Unassigned Work</td> 
   <td> <p>This area displays tasks <span class="preview">and issues</span> unassigned to users. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>This area does not display any work items by default. We recommend using filters to display relevant information for you in this area.</p> <p>After you apply a filter, this area displays the following work items:</p> 
    <ul> 
     <li>unassigned</li> 
     <li>assigned to a team </li> 
     <li>assigned to a job role</li> 
     <li> <p>assigned to a team and a role at the same time</p> </li> 
    </ul> <p>Tip: Items assigned to a user as the primary assignee do not display in the Unassigned Work area. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assigned Work</td> 
   <td> <p> All active users in the system display in this area by default. We recommend using filters to limit the amount of information in this area.  </p> <p>Both tasks and issues display in the Assigned Work area. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>The work items that the users are assigned to display under their names. </p> <p>If a work item is assigned to multiple users, the item displays under each assigned user. </p> </td> 
  </tr> 
 </tbody> 
</table>

For information about applying a filter in the Workload Balancer, see [Filter information in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

![](assets/balancer-empty-unassiged-area-350x179.png)

## Navigate the Workload Balancer

You can update the view in the Workload Balancer to display exactly the information you need to focus on in the time frame that makes the most sense to you.

After selecting the settings you want to apply to your view, the Workload Balancer remembers these settings every time you access it from any browser or device.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Resourcing**.
1. Click **Workload Balancer** in the left panel.

   The Workload Balancer displays work assignment information starting with the current week. The names of work items are listed on the left side as well as represented by bars on the right side of the of the Workload Balancer within their respective timelines. By default, blue bars represent the timelines of projects and tasks and maroon bars represent issues.

   >[!TIP]
   >
   >You can change the color of the bars for projects and tasks when you select your color scheme to match the project. For more information, continue reading this procedure.

   The work items that display under the name of users in the Workload Balancer are sorted by the following criteria, in this order:

   1. Planned Start Date (oldest first)
   1. Planned Completion Date (oldest first)
   1. Alphabetical by project (only when the first two criteria are identical for multiple work items)

1. Click the right-pointing arrow to the left of the Unassigned or Assigned areas to expand all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Click the down-pointing arrow to the left of the Unassigned or Assigned areas to collapse all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Use the horizontal scroll to navigate the timelines of work items that extends beyond the limits of the screen. 
1. Use the vertical scroll to display additional users and work items. 
1. Drag and drop the separation line between the left panel and the timeline areas to adjust the size of the left panel.

   ![](assets/separation-line-between-left-panel-and-timeline-highlighted-nwe-350x174.png)

1. Click the **Filter icon** ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or the **Assigned Work** areas to select the type of information to display in the Workload Balancer.

   For information about filtering information in the Workload Balancer, see [Manage filters in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md). 

1. Click the right-pointing arrow next to **Unassigned Work** to expand this area or the down-pointing arrow to collapse it.

   >[!TIP]
   >
   >No items display in this area by default. You must apply a filter to view unassigned work items.

1. Drag and drop the separation line between the **Unassigned Work** and **Assigned Work** areas to adjust their size.

   ![](assets/modern-scheduler-separation-line-between-areas-350x278.png)

1. Click the back or forward icons ![](assets/back-and-forward-icons.png) to navigate the timeline, then click **Today** to return to the current week. 

1. Click the **time frame drop-down menu** on the toolbar, then click the beginning date of the period you want to display. By default, the first week selected on the calendar is the week you navigated to.

   ![](assets/calendar-date-picker-wb.png)


1. Click one of the following options in the toolbar to display information by different time frames:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Day</td> 
      <td>Displays information by day for four weeks starting with today's date, by default. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Week</td> 
      <td>Displays information by week for four weeks. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Month</td> 
      <td> <p><span>Displays information by month for three months.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Select the number of weeks you want to display at one time in the Workload Balancer from the following options:

   * 1 week
   * 2 weeks
   * 4 weeks. This is the default setting.
   * 6 weeks
   * 3 months
   ![](assets/3-months-12-weeks-drop-down-wb.png)     

1. Click the **Settings** icon ![](assets/settings-gear-icon.png).

   The Settings panel displays.

   ![](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   Select from the options listed below to update the information you view in the Workload Balancer, then click the **X icon** in the upper-right of the Settings box to close it.

   * **Group by Project**: When this is selected, the items in the Unassigned and Assigned Work areas are grouped by project. This is selected by default.

     ![](assets/group-by-project-350x530.png)

   * **Include hours from issues**: When this is selected, issues assigned to users display under the user's name in the Assigned Work area <span class="preview">and issues that are not assigned to users display in the Unassigned Work area</span>. The Planned Hours from the issues count towards the Planned Hours for the project and for the user in the Assigned Work area. 

        ![](assets/issue-on-workload-balancer-350x20.png)

   
      * **Show Projected Dates**: When this is selected, the projected timeline of work items displays in addition to the planned timeline. Notice the following:

         * The projected timeline of project, tasks, and issues displays as a dark blue line above the task, issue, and project bars.
         * The projected timeline that is outside of the planned timeline displays in light blue, even when you update the color theme, as described below.
         * The projected timeline for the items that you have no access to view displays in light gray with a line underneath.
         * When a task or issue completes before the due Planned Completion Date the allocation numbers for the remaining days are struck through and do not count towards the user's allocation. This displays only when both the Show Projected Dates setting and the Show allocation icon are enabled.

         ![](assets/task-issue-projected-timelines-350x91.png)

         >[!TIP]
         >
         >Notice that work items display in the Workload Balancer when either their planned or the projected timelines (not necessarily both at the same time) occur during the timeframe selected.

   * **Show completed work**: When this is enabled, tasks and issues that are completed display in the Assigned Work area. This is enabled by default.

     A green checkmark icon ![](assets/green-checkmark-icon.png) displays to the upper-right corner of a task or issue bar when they are completed. The same icon displays for a project when the tasks or issues for the selected time frame of the project are completed. 
   
   * **Show remaining time**: When this is enabled, Workfront displays the difference between the daily time for which the user is available to work based on their schedules and the hours for which they are allocated in the Assigned Work area for the users. This is disabled by default and allocated time displays by default.

   * In the **Select color theme** section, select the color that you want for the project and task bars.  

      >[!NOTE]
      >
      >The setting for selecting the color theme  does not affect the color of the issue bars. Issues always display in a maroon-color bar. 


      Select from the following:

      * **Default**: The bars for all projects and their work items display in blue.  
      * **Project**: The bars associated with each project and its tasks change according to the name of the project. All tasks that belong to the project display in bars that match the color of the project. The project bars display in a lighter shade to distinguish them from the tasks. The project bars also include a project icon when choosing not to display allocations.
      * **Project Status**: The bars associated with each project and its work items change to the color of the status of the project.

        >[!TIP]
        >
        >* The project status is that associated with the Group of the project. If the Group does not have group-specific statuses, the color of the work item bars is that of the system-level project status. Both system as well as custom statuses display. For information about group statuses, see [Create or edit a group status](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
        
   * In the **Display user allocation in** section, select from the following:

      * **Hours**: Displays allocated time as hours. This is the default. 
      * **Percentage**: Displays allocated time as a percentage of the total available time

   * In the **Sorting preferences** section, select how you want the items to be sorted in the Workload Balancer. Select from the following options: 

      * **Sort users by Primary Role**: Users display in the alphabetical order of their Primary Roles in the Assigned Work area.

      * **Sort users alphabetically**: Users display in the alphabetical order of their first names in the Assigned Work area.

      * **Sort projects by**: Select a project field from the drop-down menu to sort projects alphabetically by that field in the Unassigned or Assigned Work areas. 

      >[!TIP]
      >
      >You can sort by projects only when the Group by Project setting is enabled. Otherwise, this setting is dimmed.


1. (Optional and conditional) If you changed the color theme to Project Status, hover over the name of a project on the left to view the status of the project.

   ![](assets/hover-over-project-status-tooltip-350x115.png)

1. <span class="preview">(Conditional and recommended) In the Workload Balancer of a project, apply a filter in the Assigned Work area to display users that are important to you but might not be assigned to items on the project, then click the **Show all users** icon ![](assets/show-all-users-icon-project-workload-balancer.png). This displays other users in the system that are not yet assigned on the project. For information about how to build a filter, see [Manage filters in the Workload Balancer](../workload-balancer/filter-information-workload-balancer.md).</span>

 
   >[!TIP]
   >
   ><span class="preview">The Show all users icon is available only for the Workload Balancer of a project.</span> 

1. Click the **Chart icon** ![](assets/user-allocation-chart-icon.png) to display the user allocation in a chart format. Days where the user is overallocated display as red blocks, and days where the user is underallocated or at capacity display as blue blocks. The size of the blocks indicates the amount of the allocation: the larger the box, the more time the user is allocated to work items for that day or week.

   ![](assets/user-allocation-chart-350x237.png)

1. Click the **Show allocations icon** ![](assets/show-allocations-icon-small.png) to view the daily or weekly Planned Hours for work items.

   This replaces the name in the bars of the work items with the amount of daily or weekly Planned Hours in the Unassigned and Assigned Work areas. This setting is disabled by default.

   >[!TIP]
   >
   >* The Show allocations setting only affects what displays for projects, tasks, issues and inaccessible items. Daily Planned Hours for users display by default and cannot be hidden.
   >* You must enable the Group by Project setting to display daily Planned Hours for projects. 
   >* When you view the Workload Balancer by week, the hours displayed are the weekly Planned Hours. 

   Days that show overallocations display in red. 

1. (Optional) Hover over the allocated time in the user line to understand what the capacity and allocation of the user. The capacity is the availability of the user according to their schedule.

   ![](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Optional) Click the **Hide allocations icon** ![](assets/show-allocations-icon-small.png) to display the name of the tasks in the bars of the work items. 
1. Click the **More menu** icon ![](assets/more-icon.png) to the right of a task or issue name, then click one of options below. 

   ![](assets/more-menu-right-of-task-350x104.png)

      * **Assign this to**, then start typing the name of a user, role, or team you want to assign the work item to in the **Search people, role, or teams** field.
    
      >[!TIP]
      >
      >You can also use the following shortcuts to assign tasks or issues:
      >
      >* In Windows: CTRL+click the task or issue bar.
      >* In Mac: CMD+click the task or issue bar.

      For more information about assigning work items to users in the Workload Balancer, see [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md). 

      >[!TIP]
      >
      >If your Workfront or group administrator enabled delegations in your environment, use the Assignments tab to assign users to the task or issue. For information about delegating work, see [Manage task and issue delegation](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Edit allocations**, then edit the daily or weekly allocations for the user. For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

1. Click the bar of a task or issue to open the Summary panel on the right

   Or

   Click **Open Summary** icon ![](assets/summary-panel-icon.png), then click the bar of a task or issue to open the Summary panel

   Or

   Click the **More** menu ![](assets/more-icon.png) to the right of a task or issue, then click **Open Summary**.

   For information about updating task information in the Summary in the Workload Balancer, see [Update work items in the Workload Balancer using the Summary](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

    The Summary panel opens on the right. 

1. Click **Bulk Assignments** to assign work items in bulk.

   For more information, see [Assign work in bulk using the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md). 

1. Click the **Full screen** icon ![](assets/full-screen.png) to display the Workload Balancer in full screen, then click the **Exit full screen** icon ![](assets/exit-full-screen.png) to return to the default screen. 
1. (Optional) Double-click a daily or weekly allocation for a user inside the bar of a work item to edit the number of allocated hours, then click the **Save** icon ![](assets/save-allocations-wb.png) to save the allocations or the **Cancel** icon ![](assets/cancel-allocations-wb.png) to remove the allocations you adjusted.

   >[!TIP]
   >
   >The Save and Cancel icons display towards the end of a task or an issue's timeline bar.

   For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md). 

1. Click the name of a work item on the left to access it. 
1. Click the **Shareable link icon** ![](assets/wb-shearable-link-icon-small.png) to copy the direct URL for the Workload Balancer to your clipboard. 
1. (Optional) Share the link with any user who does not have direct access to the Workload Balancer.

   For information about sharing the Workload Balancer with a link, see [Share the Workload Balancer with a link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md). 

1. (Conditional) From the Workload Balancer of a project, click the **Show role allocations** icon ![](assets/show-role-allocation-icon.png).

   The Role Allocation panel displays. You can view information about Planned Hours associated with job roles on the project and job roles associated with initiatives from the Scenario Planner. For more information, see [Overview of reconciling resource allocations between projects and initiatives](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

   >[!TIP]
   >
   >You cannot view initiative job role information if your organization has not purchased a license for the Workfront Scenario Planner. In this case, you can only view the planned hours associated with job roles on the project. For more information, see [Access needed to use the Scenario Planner](../../scenario-planner/access-needed-to-use-sp.md).

-->