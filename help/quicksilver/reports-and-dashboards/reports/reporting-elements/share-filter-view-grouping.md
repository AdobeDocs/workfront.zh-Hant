---
product-area: reporting
navigation-topic: reporting-elements
title: 共用篩選、檢視或分組
description: 您可以與其他使用者共用您有權檢視的篩選器、檢視和群組。
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 1%

---

# 共用篩選、檢視或分組

<!-- Audited: 11/2024 -->

<!--(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)
(NOTE: This is linked from the TOC article in WF Basics > permissions section)-->

當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯物件的存取權。 如需授與物件存取權的詳細資訊，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

除了授予使用者的存取層級之外，您還可以授予他們檢視或編輯您所建立或有權共用之特定物件的許可權。 如需存取層級和許可權的詳細資訊，請參閱[存取層級和許可權如何搭配運作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

您可以與其他使用者共用您有權檢視的篩選器、檢視和群組。

當您共用篩選、檢視或分組時，您可以將該篩選、檢視或分組套用至您的清單。 根據您獲得的存取權，您或許可以修改該區段並與其他使用者共用。

如需如何建立篩選、檢視或群組的相關資訊，請參閱下列文章：

* [篩選器總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* 在Adobe Workfront中[檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>投稿人或以上</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>要求或更高版本</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>檢視或更高許可權存取篩選器、檢視、群組</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td><p>檢視或具有存取許可權更高的許可權可共用檢視、篩選器或群組</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共用篩選、檢視或分組

<!--(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)-->

根據您用來共用篩選器的來源介面：標準或舊版，共用選取清單中的篩選器會有所不同。 如需有關篩選建立介面型別的資訊，請參閱[在Adobe Workfront中建立或編輯篩選器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md)。

您只能在舊版介面中共用檢視和群組。

### 使用標準產生器介面共用篩選器

您可以在標準介面中從專案、任務、問題、投資組合、計畫、使用者、範本或群組清單共用篩選器。 篩選的標準產生器介面不適用於任何其他物件，也不可用於檢視或群組。

使用標準產生器介面共用篩選器：

1. 前往專案、任務或問題的清單。
1. 按一下&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-nwepng.png)。

   ![標準篩選產生器](assets/new-filters-all-filter-types.png)

1. 檢閱下列篩選器清單：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>已新增至最愛</strong></td>
   <td>您標示為我的最愛的篩選器。 當您最愛某個篩選器時，其原始位置會顯示在篩選器名稱下方，且除非您將其移除為最愛，否則會隱藏在原始清單中。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已儲存</strong></td>
   <td>您自行建立和儲存的篩選器。 依預設，此清單會以最近儲存的順序顯示已儲存的篩選器，但您可拖曳篩選器名稱以手動方式重新排序清單。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>系統預設值</strong></td>
   <td>Workfront系統預設篩選器，以及Workfront管理員新增至您的篩選器清單中的篩選器（在系統層級或版面配置範本中）。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>與我共用</strong></td>
   <td>其他人建立並與您共用或全系統共用的篩選器。</td>
   </tr>
   </tbody>
   </table>

1. 將滑鼠停留在您至少可以存取檢視和共用的篩選器上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-icon-spectrum.png)，然後按一下&#x200B;**共用**。

   ![更多功能表選項](assets/new-filters-more-menu-options-with-delete.png)

   篩選器共用方塊隨即顯示。

1. 在&#x200B;**授與**&#x200B;存取權的欄位中，開始輸入您要共用給的使用者、團隊、角色、群組或公司名稱。

   ![篩選器共用方塊](assets/new-filters-share-filter.png)

1. （選擇性）按一下實體名稱旁的向右箭頭，以編輯其對篩選器的許可權，然後啟用&#x200B;**檢視**&#x200B;或&#x200B;**管理**&#x200B;選項。 **檢視**&#x200B;為預設值。

   ![共用許可權](assets/new-filters-sharing-permissions.png)

1. （選用）執行下列任一項作業，來啟用或停用實體的其他許可權：

   1. 按一下&#x200B;**檢視**&#x200B;並停用&#x200B;**共用**&#x200B;選項。 預設為啟用。
   1. 按一下&#x200B;**管理**&#x200B;並停用&#x200B;**共用**&#x200B;或&#x200B;**刪除**&#x200B;選項。 預設為啟用。

      >[!NOTE]
      >
      >如果您啟用「使用刪除功能管理存取權」選項，即使這些使用者並非篩選器擁有者，他們仍可從所有使用者中刪除篩選器。

   >[!TIP]
   >
   >使用者無法取得高於其存取層級的許可權。 如果他們無權在其存取層級中編輯篩選器，則無法取得管理篩選器的許可權。 Workfront會停用這些使用者的「管理」選項，且選項會變暗。

1. 按一下「**共用**」。篩選器會與您指定的實體共用。

   >[!TIP]
   >
   >與群組共用會將篩選的許可權授予群組的成員及所有子群組。

   您共用的篩選器會顯示在這些實體的篩選器面板的&#x200B;**與我共用**&#x200B;區段中。

   ![與我共用的篩選器](assets/new-filters-shared-with-me.png)

### 使用舊版介面共用篩選器、檢視和群組

在舊版介面中共用篩選器、檢視和群組的方式相同。

1. 移至物件清單或報表。
1. （視條件而定）從清單中，按一下&#x200B;**篩選器**、**檢視**&#x200B;或&#x200B;**群組**&#x200B;圖示，然後將滑鼠移至您要共用的篩選器、檢視或群組上，按一下&#x200B;**更多**&#x200B;圖示![更多](assets/more-icon.png)，然後按一下&#x200B;**共用**。

   在報表中，按一下&#x200B;**篩選器**、**檢視**&#x200B;或&#x200B;**群組**&#x200B;下拉式功能表，然後選取您要共用的篩選器、檢視或群組。

1. （視條件而定）如果從報表共用，請再次按一下&#x200B;**篩選器**、**檢視**&#x200B;或&#x200B;**群組**&#x200B;下拉式功能表，然後按一下&#x200B;**共用篩選器**、**共用檢視**&#x200B;或&#x200B;**共用群組**。\
   顯示&#x200B;**篩選器存取權**、**檢視存取權**&#x200B;或&#x200B;**群組存取權**&#x200B;對話方塊。

   ![共用篩選器](assets/share-filter-people-box-nwe-350x458.png)

1. 根據您想要共用給哪些人員，完成下列任一作業：

   **若要與個別使用者、團隊、角色、群組或公司共用：**&#x200B;在提供的欄位中，開始輸入您要與其共用的使用者、團隊、角色、群組或公司的名稱，然後在其出現在下拉式清單中時按一下該名稱。\
   重複此程式，與多個使用者、團隊、角色、群組或公司共用存取權。

   >[!TIP]
   >
   >與群組共用會將篩選、檢視或分組的許可權授予群組的成員及所有子群組。

   **要與系統中的所有使用者共用：**&#x200B;按一下&#x200B;**設定**&#x200B;圖示，然後按一下&#x200B;**讓此在整個系統內可見**。\
   您的管理員必須選取「共用系統範圍」選項，才能使用此選項。 如需詳細資訊，請參閱文章[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)和[共用報告、儀表板和行事曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。

1. （視條件而定）如果您要與個別使用者、團隊、角色、群組或公司共用，請按一下下拉式功能表，以定義您要授與的存取層級。

   您可選取下列選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>檢視它</strong></td> 
      <td> <p>選取此選項可允許共用收件者僅使用共用篩選器、檢視或群組。 選取此選項時，收件者無法對共用專案進行任何修改。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理它</strong></td> 
      <td> <p>選取此選項可允許共用收件者使用和修改共用篩選器、檢視或群組。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>共用</strong></td> 
      <td> <p>按一下<strong>進階設定</strong>，然後選取或清除<strong>共用</strong>選項（視您是否希望收件者能夠與其他人共用而定）。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。

   與您共用篩選、檢視或群組的使用者可以按一下&#x200B;**篩選**、**檢視**&#x200B;或&#x200B;**群組**&#x200B;下拉式功能表或圖示，然後向下捲動至&#x200B;**與我共用**&#x200B;區段來存取它。


