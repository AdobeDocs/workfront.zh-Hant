---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作負載平衡器中篩選資訊
description: 為了有效地找到工作專案並專注於您管理的使用者或專案，我們強烈建議您在工作負載平衡器中使用篩選器。
author: Lisa
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: fc82ce4b5abb2cd7411d62ac8bb428bc5337386f
workflow-type: tm+mt
source-wordcount: '2458'
ht-degree: 0%

---

# 在工作負載平衡器中篩選資訊

<!-- Audited: 6/2025 -->

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

身為資源管理員，您可以使用工作負載平衡器來檢視和管理使用者的工作負載。 如需有關工作負載平衡器的更多一般資訊，請參閱以下文章：

* [工作負載平衡器總覽](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>為了有效地找到工作專案並專注於您管理的使用者或專案，我們強烈建議您在工作負載平衡器中使用篩選器。 這可讓您在開始管理資源的指派之前，顯示正確的資訊。
>
>當您在儲存並套用新篩選器後離開工作負載平衡器時，即使您登出並重新登入，仍會套用篩選器。

本文包含有關工作負載平衡器中的篩選器的資訊。 如需Workfront中篩選器的相關資訊，請參閱[篩選器概觀](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>目前：計畫（在資源區域使用工作負載平衡器時）</p>
       <p>或</p>
       <p>工作（使用團隊或專案的工作負載平衡器時）</p></td>
  </tr>
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視以下專案或更高存取權：</p> 
    <ul> 
     <li>資源管理</li> 
     <li>專案</li> 
     <li>任務</li> 
     <li>問題</li>
     <li>篩選器、檢視和群組</li>
    </ul>
    <p>建立或編輯篩選器時，編輯對篩選器、檢視和群組的存取權 </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案、任務和問題的許可權或更高</p>
   <p>管理您要編輯或刪除之篩選器的許可權</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 工作負載平衡器中的篩選器概觀

在工作負載平衡器中使用篩選器時，請考慮以下事項：

* 根據您從何處存取工作負載平衡器，Workfront可能已經在為您篩選資訊。 如需詳細資訊，請參閱本文中的下列章節： [工作負載平衡器中預先套用的篩選器](#pre-applied-filters-in-the-workload-balancer)。
* 您可以建立並套用篩選器而不儲存它，也可以儲存篩選器以供稍後重複使用。
* 當您套用篩選器而不儲存時，可以透過重新整理頁面將其還原為原始清單。
* 您可以檢視您建立的篩選器，或其他使用者建立並與您共用的篩選器。
* 當您刪除或編輯共用篩選器時，也會為您共用該篩選器的所有人刪除或編輯該篩選器。
* 當您在工作負載平衡器在一個區域中建立篩選器，它們在其他區域中無法使用。

  例如，在資源區域中建立的篩選器在專案或團隊的工作負載平衡器中不可用。

  如需尋找工作負載平衡器的位置相關資訊，請參閱[尋找工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

* 如果專案也符合工作負載平衡器畫面上顯示的時間軸中的日期，您只能檢視符合所選篩選器的專案。

## 在工作負載平衡器中預先套用的篩選器 {#pre-applied-filters-in-the-workload-balancer}

工作負載平衡器在2個不同的區域顯示資訊：

* **未指派的工作區域**：尚未指派給使用者的工作專案。
* **指派的工作區域**：指派給使用者的工作專案。

  如需有關每個區域中所顯示內容的資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

>[!IMPORTANT]
>
>工作負載平衡器的每個區域都有自己的篩選器集，這些篩選器會相互獨立運作。 您必須同時設定兩個篩選器，以指出要在每個區域檢視哪些資訊。

工作負載平衡器顯示使用者及其工作專案。
指派給使用者的工作專案僅在專案日期與畫面上顯示的時間範圍相符時顯示。

根據您存取「工作負載平衡器」的位置，「未指派」和「已指派」區域已依特定條件篩選，如下表所述：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>您存取工作負載平衡器的Workfront區域</strong></td> 
   <td><b>預設顯示在[未指派的工作]區域中的專案</b> </td> 
   <td><b>預設顯示在指派的工作區域中的專案</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">資源區域</td> 
   <td>預設不會顯示任何專案。 您必須自訂篩選器才能檢視此區域中的工作專案。</td> 
   <td>屬於您任何團隊及其工作專案的使用者。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">團隊</td> 
   <td>指派給團隊或團隊與工作角色的工作專案。 </td> 
   <td> <p>屬於所選團隊及其工作專案的使用者。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">專案</td> 
   <td> <p>取消指派的工作專案或指派給所選專案中團隊或工作角色的專案會顯示在此區域中。</p> </td> 
   <td> <p>已選取<b>此專案的工作專案</b>系統預設篩選器時，指派給選定專案上至少一個工作專案的使用者及其專案上的工作專案。 </p>

<p>取消選取<b>此專案的工作專案</b>系統預設篩選器時，專案的已指派工作區域會顯示指派給選定專案上至少一個專案的使用者的所有工作專案。  <br><br>預設會取消選取此篩選器。</p>

<p> <b>注意</b>：您可以在專案的工作負載平衡器中啟用<b>顯示所有使用者</b>選項，以顯示系統中的所有使用者。 如需詳細資訊，請參閱<a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">瀏覽工作負載平衡器</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## 建立工作負載平衡器篩選器

無論您從何處存取工作負載平衡器，為工作負載平衡器中的未指派工作和指派的工作區域建立篩選器的程式都是相同的。 如需有關尋找工作負載平衡器的資訊，請參閱[尋找工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

您可以從頭開始建立篩選器，或編輯其中一個預先定義的篩選器。 如需您可以編輯的現有篩選器相關資訊，請參閱本文中「工作負載平衡器」的[編輯現有篩選器](#edit-an-existing-filter-in-the-workload-balancer)區段。

1. 前往工作負載平衡器。

   如需有關存取工作負載平衡器的資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

1. 在&#x200B;**未指派的工作**&#x200B;或&#x200B;**已指派的工作**&#x200B;區域的右上角，按一下&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-icon.png)。 **篩選器**&#x200B;方塊會顯示在右側，而您建立篩選的區域名稱會顯示在標題中。

   ![篩選器清單](assets/filters-list.png)

1. （選擇性和條件性）如果您存取&#x200B;**資源**&#x200B;區域的工作負載平衡器，預先定義的預設篩選器可能已套用至&#x200B;**指派的工作**&#x200B;區域。 您可以編輯並儲存預設篩選的復本。

   >[!TIP]
   >
   >預設篩選器會顯示屬於您任何團隊的使用者及其工作專案。 您可以編輯此篩選的復本。

   如果您從專案存取[!UICONTROL 工作負載平衡器]，可能已經套用&#x200B;**此專案的工作專案**&#x200B;篩選器。 這只會顯示指派給此專案中使用者的工作專案。 您可以複製並儲存此篩選的復本。

   依預設，專案的[!UICONTROL 工作負載平衡器]會顯示指派給專案中所有使用者的所有工作專案。


1. 按一下&#x200B;**新增篩選器**。

1. 若要建立篩選器，請執行下列動作：

   1. 在第一個下拉式功能表中選取欄位名稱，或按一下下拉式功能表底部的&#x200B;**瀏覽欄位**，以輸入預設不會顯示的欄位名稱。

      >[!IMPORTANT]
      >
      >當參考自訂欄位時，您必須輸入欄位名稱，而不是欄位標籤。 欄位標籤會顯示在附加至物件的自訂表單上。 如需標籤與自訂欄位名稱之間差異的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

   1. （視條件而定）如果您按一下&#x200B;**瀏覽欄位**，請在&#x200B;**搜尋**&#x200B;欄位中輸入欄位名稱，並在該欄位顯示在清單中時選取它。

      ![搜尋欄位](assets/new-filters-search-for-a-field.png)

      >[!TIP]
      >
      >您可以從下列區段中選取欄位：
      >
      >* **最近的選擇**：您最近篩選的欄位。
      >* **建議**：最常使用的欄位。


   1. 從第二個下拉式功能表中選取修飾元。 如需Workfront篩選修飾元的資訊，請參閱[篩選和條件修飾元](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。
   1. 選取或輸入您要篩選的欄位值。

      >[!NOTE]
      >
      > 當您想要顯示特定投資組合中的工作物件時，可以套用以下篩選器： Portfolio ID等於&lt; PORTFOLIO NAME >。
      >
      >![Portfolio名稱篩選器陳述式](assets/portfolio-name-filter.png)
      >
      >若要排除狀態為「保留」的專案，您必須套用下列篩選：專案：狀態不等於保留。 這可防止工作項在工作負載平衡器中顯示「保留」專案中的工作項。
      >
      >![專案狀態篩選器陳述式](assets/project-status-filter.png)

   1. （選擇性）按一下&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete.png)以移除篩選條件。

1. （選擇性）按一下&#x200B;**新增篩選器**&#x200B;以新增其他篩選器條件，然後重複步驟4中的動作。

   <!--(NOTE: ensure this stays correct)-->

1. 按一下&#x200B;**套用**，將篩選結果套用至選取的工作負載平衡器區域而不儲存。 左邊的工作專案清單會更新。

   >[!IMPORTANT]
   >
   >當您新增的所有篩選器陳述式同時為true時，結果會顯示在工作負載平衡器中。

   篩選器會保留到您重新整理頁面為止，而&#x200B;**套用**&#x200B;按鈕會以&#x200B;**另存新檔**&#x200B;按鈕取代。

1. 按一下&#x200B;**另存新檔**，儲存篩選器以供日後使用。

   >[!TIP]
   >
   >隨時按一下&#x200B;**取消**&#x200B;即可返回篩選建立區域。

1. 在&#x200B;**未命名的篩選器**&#x200B;欄位中，輸入新的篩選器名稱。
1. （選擇性）從&#x200B;**圖示**&#x200B;下拉式功能表中選取新篩選的圖示。

   ![選取圖示](assets/new-filters-select-icon.png)

1. （選擇性）新增篩選器&#x200B;**描述**。 說明會顯示在篩選器清單中的篩選器名稱下。
1. 按一下「**儲存**」。儲存的篩選器會顯示在篩選器方塊的&#x200B;**我的篩選器**&#x200B;區域中。

   如需有關套用已儲存篩選的資訊，請參閱本文的[刪除工作負載平衡器](#delete-a-saved-filter-in-the-workload-balancer)中已儲存的篩選。

1. （視條件而定）將滑鼠移至&#x200B;**未指派的工作**&#x200B;或&#x200B;**已指派的工作**&#x200B;區域的右上角&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-icon.png)上方，以顯示目前套用之篩選器名稱或數量的工具提示。

   ![篩選器圖示與篩選器名稱](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## 複製篩選器

您可以複製並編輯篩選器以建立新篩選器。

1. 前往工作負載平衡器。

   如需有關存取工作負載平衡器的資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

1. 在&#x200B;**未指派的工作**&#x200B;或&#x200B;**已指派的工作**&#x200B;區域的右上角，按一下&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-icon.png)。  **篩選器**&#x200B;方塊會顯示在右側，而您要複製篩選的區域名稱會顯示在標題中。

1. 將滑鼠停留在現有的篩選器上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu-edit-filter.png)。
1. 按一下&#x200B;**複製**。

   >[!TIP]
   >
   > 編輯篩選器時，您可以按一下「**編輯篩選器**」方塊左下角的「**更多**」功能表「![更多」功能表「](assets/more-menu-edit-filter.png)」，然後按一下「**複製**」。

1. 針對複製的篩選條件編輯下列資訊：

   * 姓名
   * 圖示
   * 說明
   * 任何欄位、修飾元或值。

1. （選擇性）按一下&#x200B;**新增篩選器**，將更多陳述式新增至重複的篩選器。
1. 按一下「儲存」**&#x200B;**，將重複的篩選器儲存在&#x200B;**「我的篩選器」**&#x200B;區域中。 原始濾鏡保持不變，而複製的濾鏡會儲存為新濾鏡。

## 在工作負載平衡器中編輯現有篩選器 {#edit-an-existing-filter-in-the-workload-balancer}

您可以在工作負載平衡器中編輯儲存的篩選器。

>[!TIP]
>
>當您編輯與其他人共用的篩選器時，他們也會看到您所做的變更。

1. 前往工作負載平衡器。

   如需有關存取工作負載平衡器的資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

1. 在&#x200B;**未指派**&#x200B;或&#x200B;**已指派的工作**&#x200B;區域的右上角，按一下&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-icon.png) 。 篩選器產生器會顯示在右側。

1. 將游標移至您要編輯的篩選器上，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯篩選器圖示](assets/wb-edit-filter-icon.png)。

1. 執行下列其中一項：

   * 修改任何篩選器陳述式。
   * 按一下&#x200B;**新增篩選器**&#x200B;以新增篩選器陳述式。
   * 按一下&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete.png)以移除現有的篩選陳述式。

1. （選擇性）按一下&#x200B;**套用**。 結果更新在工作負載平衡器左側，以說明您對篩選器進行的變更。

1. 按一下「**儲存**」。結果會在左側的工作負載平衡器中更新，並且篩選器會更新為您選擇的新資訊。

## 刪除工作負載平衡器中儲存的篩選器 {#delete-a-saved-filter-in-the-workload-balancer}

刪除篩選器前，請先考量下列事項：

* 您無法復原已刪除的篩選器。
* 您無法刪除預先定義的篩選器。
* 您無法刪除未儲存的篩選器。 在登出並再次登入Workfront後，它們會自動移除。
* 刪除共用篩選器時，也會刪除與其共用之所有使用者的篩選器。
* 刪除所有儲存的篩選器後，工作負載平衡器會根據原始預設值顯示。

>[!NOTE]
>
>當您刪除與其他人共用的篩選器時，也會為他們刪除該篩選器。

1. 前往工作負載平衡器。

   如需有關存取工作負載平衡器的資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

1. 在&#x200B;**未指派的工作**&#x200B;或&#x200B;**已指派的工作**&#x200B;區域的右上角，按一下&#x200B;**篩選圖示** ![篩選圖示](assets/filter-icon.png)。 **篩選器**&#x200B;方塊會顯示在右側。

1. 將滑鼠移到篩選器上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu-edit-filter.png)，然後按一下&#x200B;**刪除**。

   >[!TIP]
   >
   >編輯篩選器時，您可以按一下「**編輯篩選器**」方塊左下角的「**更多**」功能表「![更多」功能表「](assets/more-menu-edit-filter.png)」，然後按一下「**刪除**」。

1. （選擇性）按一下&#x200B;**取消**&#x200B;以取消刪除並返回篩選器清單。
1. 按一下&#x200B;**刪除**&#x200B;以確認刪除。 篩選會為您及所有擁有其許可權的使用者刪除。

## 在工作負載平衡器共用篩選器

您可以共用您建立或其他使用者與您共用的篩選器。

在工作負載平衡器中共用篩選器時，請考慮下列事項：

* 您可以與作用中使用者、團隊、角色和公司共用篩選器，或讓您的Workfront執行個體中的每個人看見這些篩選器。
* 您在資源區域中共用的篩選器在專案或團隊的工作負載平衡器中不可見。
* 您和其他人共用的工作負載平衡器篩選器在Workfront的其他區域中不可見。

若要共用篩選器：

1. 前往工作負載平衡器。

   如需有關存取工作負載平衡器的資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

1. 在&#x200B;**未指派的工作**&#x200B;或&#x200B;**已指派的工作**&#x200B;區域的右上角，按一下&#x200B;**篩選圖示** ![篩選圖示](assets/filter-icon.png)。 **篩選器**&#x200B;方塊會顯示在右側。

1. 將滑鼠停留在篩選器上，然後按一下&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu-edit-filter.png)。

1. 按一下「**共用**」。顯示&#x200B;**篩選器共用**&#x200B;方塊。

   >[!TIP]
   >
   > 編輯篩選器時，您可以按一下&#x200B;**編輯篩選器**&#x200B;方塊左下角的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu-edit-filter.png)，然後按一下&#x200B;**共用**。

1. 在&#x200B;**授與**&#x200B;存取權的欄位中，輸入您要共用篩選器的使用者、團隊、角色、群組或公司名稱，然後在它們出現時選取它們。

1. （選擇性）若要編輯實體的篩選許可權，請按一下其名稱旁邊的右箭頭，然後選取&#x200B;**檢視**&#x200B;或&#x200B;**管理**。

   ![篩選器許可權](assets/access-level-additional-settings.png)

1. （選用）執行下列任一項作業，來啟用或停用實體的其他許可權：

   1. 按一下&#x200B;**檢視**&#x200B;並停用&#x200B;**共用**&#x200B;選項。 這預設為啟用。

   1. 按一下&#x200B;**管理**&#x200B;並啟用&#x200B;**共用**&#x200B;或&#x200B;**刪除**&#x200B;選項。

   >[!TIP]
   >
   >使用者無法收到高於其存取層級的許可權。 如果他們無權在其存取層級中編輯篩選器，則無法取得管理篩選器的許可權。 Workfront會停用這些使用者的「管理」選項。

1. 按一下「**共用**」。篩選器與您指定的實體共用，且共用篩選器顯示在&#x200B;**篩選器**&#x200B;方塊的&#x200B;**與我共用**&#x200B;區域。

   ![與我共用](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![Filter icon](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![Favorites icon](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
