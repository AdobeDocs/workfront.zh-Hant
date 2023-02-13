---
product-area: projects
navigation-topic: manage-issues
title: 移動問題
description: 您可以在專案和任務之間移動問題。
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# 移動問題

您可以在下列物件之間移動問題：

* 從專案到其他專案
* 從同一項目或另一個項目中的任務到另一個任務
* 從任務到項目或到另一個項目
* 從項目到同一項目中的任務或另一個項目中的任務

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
   <td> <p>要求或更高版本</p> <p>檢閱或更高授權，以移動專案的「問題」區段中的問題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯問題的存取權</p> <p>查看或更高程度地訪問項目和任務</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取層級問題的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予問題的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理問題的權限</p> <p>將權限貢獻至您要移動問題的項目，並提供新增問題的功能。</p> <p> 如需授予問題權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題 </a></p> <p>如需要求其他權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 移動問題的考量事項

移動包含檔案或與請求佇列相關聯的問題時，請考量下列事項：

* **當問題與請求佇列相關聯時：** 將問題移至另一個物件且問題與請求佇列相關聯時，移動的問題不再與第一個問題源自的原始佇列相關聯。
* **將文檔附加到問題時：** 將問題移到另一個對象時，如果問題附加了文檔，則文檔、其版本和校樣也會移到新問題。 與文檔關聯的任何批准都不會移動。
* **將問題連結到文檔或資料夾時：** 當您移動文檔或資料夾連結到第三方服務(如Google Drive)的問題時，指向文檔的連結將隨問題一起移動。

## 在清單中移動問題

您可以從問題清單或問題報表中移動一或多個問題。

1. 前往包含您要移動之問題或問題的專案。

   或

   前往問題報告。

1. 如果您選取前往專案，請按一下 **問題** 中。
1. 選取您要移動的問題，然後按一下 **更多功能表** 在問題清單頂端，按一下 **移至**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. 繼續移動問題，如 [移動單一問題](#move-a-single-issue) 從步驟2開始。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## 移動單一問題 {#move-a-single-issue}

您可以在檢視問題時移動一個問題。

### 在「預覽」環境中移動單一期刊

1. 前往您要複製的問題，按一下 **更多** 功能表 ![](assets/more-icon.png)在問題名稱的右側，然後選取 **移動** 到。

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   此 **移動問題** 框。

   ![](assets/move-issue-box-nwe-350x280.png)

1. 在 **選擇目標項目** 區段，指定您要移動問題的專案名稱。 預設會顯示目前專案的名稱。

   >[!TIP]
   >
   >清單中只會顯示100個專案。

1. （有條件）按一下 **請求存取** 如果您無權將問題移至專案。
1. （條件性）如果您有權將問題新增至目標專案的其中一項工作，請繼續移動所選目標專案的問題，而不要求存取權。

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >如果所選專案處於待核准、已完成或已結束狀態，當Workfront管理員防止為這些專案新增問題時，則會顯示類似的訊息。 如需詳細資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. （選用）在 **選項** 部分，取消選擇下表中列出的任何項，以從移動的問題中刪除它們。 預設會選取所有選項。

   >[!IMPORTANT]
   >
   >取消選取「選項」清單中的項目會導致資料遺失。 將刪除現有問題中的資訊，且無法恢復。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全選</td> 
      <td>取消選取此選項，將問題移至新位置時的所有資訊從問題中移除。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指派</td> 
      <td>移除指派給問題的使用者、工作角色或團隊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進度</td> 
      <td>移除問題的完成百分比（如果有）。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>文件</p></td> 
      <td> <p>刪除文檔頁簽中的所有內容，包括文檔版本、連結的文檔和資料夾。

   <b>附註</b>

   如果您選擇不隨問題移動文檔，則這些文檔將被刪除並放入資源回收筒30天。 管理員可以還原這些檔案，並會在移動的問題上還原。

   如果問題在移動後被刪除，則還原的文檔將放置在還原這些文檔的管理員用戶頁面的「文檔」區域中。
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">權限</td> 
      <td>刪除與問題共用的實體。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新</td> 
      <td>從問題的「更新」部分刪除注釋。</td> 
     </tr> 
    </tbody> 
   </table>


1. （選用）在 **選擇任務** 部分，選擇要移動問題的任務。
1. 按一下 **移動問題** 或 **移動問題**，在清單中選取了多個問題。

   移動的問題會新增至指定的專案。




