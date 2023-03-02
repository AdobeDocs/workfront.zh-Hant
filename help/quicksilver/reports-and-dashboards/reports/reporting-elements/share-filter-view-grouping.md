---
product-area: reporting
navigation-topic: reporting-elements
title: 共用篩選、檢視或分組
description: 您可以與其他使用者共用您有權檢視的篩選器、檢視和群組。
author: Lisa
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: b56e6591c7da166bd1548420b562b838cc7fe0f2
workflow-type: tm+mt
source-wordcount: '1362'
ht-degree: 1%

---

# 共用篩選、檢視或分組

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

<span class="preview">請注意，在預覽環境中，增強的篩選體驗（先前稱為「測試版」）現在是預設值。 這些增強的篩選現在是「標準」，而舊的篩選體驗是「舊版」。</span>

您的Adobe Workfront管理員在使用者指派存取層級時，授予他們檢視或編輯物件的存取權。 有關授予對象訪問權限的詳細資訊，請參見 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

除了授予用戶的訪問級別之外，您還可以授予他們查看或編輯您建立或有權共用的特定對象的權限。 如需存取層級和權限的詳細資訊，請參閱 [存取層級與權限如何搭配運作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

您可以與其他使用者共用您有權檢視的篩選器、檢視和群組。

與您共用篩選、檢視或分組時，您可以將該篩選、檢視或分組套用至清單。 視您所獲得的存取權而定，您可能可以修改該存取權並與其他使用者共用。

如需如何建立篩選、檢視或分組的相關資訊，請參閱下列文章：

* [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>檢視或更高存取篩選器、檢視、群組</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>檢視或更高權限，具有對檢視、篩選或分組共用的存取權</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 共用篩選、檢視或分組

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

您可以使用下列介面在選取的清單中共用篩選器：

* 標準介面
* 測試版產生器介面

在選取的清單中共用篩選器會因您用來共用篩選器的介面而異。 如需建立篩選器介面類型的相關資訊，請參閱 [在Adobe Workfront中建立或編輯篩選器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

您只能在標準介面中共用檢視和群組。

* [使用標準介面共用篩選器、檢視和群組](#share-with-standard-interface)
* [使用測試版產生器介面共用篩選器](#share-with-beta-builder-interface)

### 使用標準介面共用篩選器、檢視和群組 {#share-with-standard-interface}

在標準介面中共用篩選器、檢視和群組相同。

1. 移至物件清單或報表。
1. （條件性）從清單中按一下 **篩選**, **檢視**，或 **分組** 圖示，然後將游標暫留在您要共用的篩選器、檢視或分組上，按一下 **更多** 圖示 ![更多圖示](assets/more-icon.png)，然後 **共用**.

   在報表中，按一下 **篩選**, **檢視**，或 **分組** 下拉式功能表，然後選取您要共用的篩選、檢視或分組。

1. （條件性）如果從報表共用，請按一下 **篩選**, **檢視**，或 **分組** 再按一下下拉式功能表，然後按一下 **共用篩選**, **共用檢視**，或 **共用分組**.\
   此 **篩選存取**, **檢視存取**，或 **分組訪問** 對話框。

   ![共用篩選器](assets/share-filter-people-box-nwe-350x458.png)

1. 視您要與誰共用而定，完成下列其中一項：

   **若要與個別使用者、團隊、角色、群組或公司共用：** 在提供的欄位中，開始輸入您要共用的使用者、團隊、角色、群組或公司的名稱，然後在下拉式清單中出現名稱時按一下名稱。\
   重複此程式，與多個使用者、團隊、角色、群組或公司共用存取權。

   >[!TIP]
   >
   >與組共用為組和所有子組的成員提供篩選、查看或分組的權限。


   **要與系統中的所有用戶共用，請執行以下操作：** 按一下 **設定** 圖示，然後按一下 **使此可見系統範圍**.\
   您的管理員必須選擇「共用系統」選項，此選項才可用。 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) 和 [共用報表、控制面板和日曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. （條件性）如果您要與個別使用者、團隊、角色、群組或公司共用，請按一下下拉式功能表，以定義您要授與的存取層級。

   您可以選取下列選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>檢視它</strong></td> 
      <td> <p>選擇此選項可僅允許共用收件者使用共用篩選器、視圖或分組。 選取此選項時，收件者無法對共用項目進行任何修改。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理它</strong></td> 
      <td> <p>選擇此選項可允許共用收件者使用和修改共用篩選器、視圖或分組。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>共用</strong></td> 
      <td> <p>按一下 <strong>進階設定</strong>，然後選取或清除 <strong>共用</strong> 選項，取決於您是否希望收件者能與其他人共用。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。

   您與其共用篩選器、檢視或分組的使用者可按一下 **篩選**, **檢視**，或 **分組** 下拉菜單或表徵圖，並向下滾動到 **與我共用** 區段。

### 使用測試版產生器介面共用篩選器 {#share-with-beta-builder-interface}

從專案、工作或問題清單共用篩選器時，您可以使用測試版產生器介面（而非標準介面）來共用篩選器。

測試版產生器介面不適用於Workfront中的任何其他物件。

建立報表時，您無法在測試版產生器介面中建立篩選器。

使用測試版產生器介面共用篩選器：

1. 移至專案、工作或問題清單。
1. 按一下 **篩選** 圖示 ![篩選圖示](assets/filter-nwepng.png)，然後啟用 **測試版設定** ![測試版設定](assets/beta-toggle-white-on-existing-filters.png) 存取測試版產生器。 預設為停用。

   接下來，視需要同意測試版協定。

   這會開啟測試版篩選產生器介面。

   >[!TIP]
   >
   >啟用測試版產生器時，產生器介面的標題會變為藍色。 啟用測試版產生器介面後，Workfront會在所有可用區域中持續啟用它。

   ![測試版篩選產生器](assets/new-filters-all-filter-types.png)

1. 檢閱下列篩選器清單：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>已新增至最愛</strong></td>
   <td>您標示為我的最愛的篩選器。 當您收藏某個篩選器時，其原始位置顯示在篩選器名稱下方，並且它將從原始清單中隱藏，除非您將其作為收藏刪除。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已儲存</strong></td>
   <td>您建立並儲存自己的篩選器。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>系統預設值</strong></td>
   <td>Workfront系統預設篩選器，以及Workfront管理員新增至篩選器清單的篩選器（在系統層級或您的配置範本中）。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>與我共用</strong></td>
   <td>其他人建立並與您共用的篩選器，或是在全系統內共用的篩選器。</td>
   </tr>
   </tbody>
   </table>

1. 將滑鼠指標暫留在您至少可存取檢視和共用的篩選器上，然後按一下 **更多** 功能表 ![更多功能表](assets/more-icon-spectrum.png)，然後按一下 **共用**.

   ![更多功能表選項](assets/new-filters-more-menu-options-with-delete.png)

   篩選器共用方塊隨即顯示。

1. 啟用「查看系統範圍」設定。 這可授予Workfront中任何人檢視篩選器的權限。

   >[!IMPORTANT]
   >
   >請小心使用此設定。 為所有使用者新增許多篩選器會讓篩選器體驗雜亂，並加大尋找篩選器的難度。

   或開始在 **授予** 欄位。

   ![篩選器共用方塊](assets/new-filters-share-filter.png)

1. （選用）按一下實體名稱旁的右鍵箭頭，以編輯其對篩選器的權限，然後啟用 **檢視** 或 **管理** 選項。 **檢視** 為預設值。

   ![共用權限](assets/new-filters-sharing-permissions.png)

1. （可選）執行下列任一操作，以啟用或停用實體的其他權限：

   1. 按一下 **檢視** 並停用 **共用** 選項。 預設會啟用。
   1. 按一下 **管理** 並禁用 **共用** 或 **刪除** 選項。 預設會啟用。

      >[!NOTE]
      >
      >如果您使用「刪除」選項啟用「管理存取權」，即使這些使用者不擁有篩選器，他們仍可從所有使用者中刪除篩選器。
   >[!TIP]
   >
   >使用者的權限無法高於其存取層級。 如果使用者在存取層級沒有編輯篩選器的存取權，就無法取得管理篩選器的權限。 Workfront會停用這些使用者的「管理」選項，且選項會呈現灰色。

1. 按一下 **共用**. 篩選器會與您指定的實體共用。

   >[!TIP]
   >
   >與群組共用為群組成員和所有子組的成員授予篩選器的權限。

   您共用的篩選器會顯示在 **與我共用** 的子欄位。

   ![與我共用的篩選器](assets/new-filters-shared-with-me.png)

