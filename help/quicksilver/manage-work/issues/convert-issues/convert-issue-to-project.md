---
product-area: projects
navigation-topic: convert-issues
title: 將問題轉換為Adobe Workfront中的專案
description: 將問題轉換為Adobe Workfront中的專案
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 0%

---

# 將問題轉換為Adobe Workfront中的專案

如果在提交問題後需要完成更多工作才能完成問題，您可以將問題轉換為專案。

您可以將問題轉換為新專案，或使用範本將其轉換為專案。 本文說明將問題轉換為專案的兩種方式。

如需轉換問題的一般資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯問題、任務和專案的存取權</p> <p>編輯對財務資料的訪問，以更新從問題轉換的預計財務資訊</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視問題的權限</p> <p>轉換問題後，您就能取得專案的「管理」權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 將問題轉換為專案

您可以將問題轉換為空白專案，或使用範本將問題轉換為專案。

1. 前往專案，然後按一下 **[!UICONTROL 問題]** 中。
1. 在顯示的問題清單中，執行下列其中一項操作：

   * 若要將問題轉換為空白專案，請按一下問題名稱，然後按一下 **[!UICONTROL 更多]** 功能表 ![](assets/more-icon.png) 在問題名稱的右側，按一下 **[!UICONTROL 轉換為空白專案]**.


      或

      在問題清單中選取問題，按一下 **[!UICONTROL 更多]** 功能表 ![](assets/more-icon.png) 在清單頂端，按一下 **[!UICONTROL 轉換為空白專案]**.

      >[!IMPORTANT]
      >
      >只有在系統或群組管理員啟用 [!UICONTROL 不使用範本即可讓使用者建立專案] 的 [!UICONTROL 設定] 的上界。 如需詳細資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


      轉換問題後，您必須手動將任務新增至專案，或將範本附加至專案。

      繼續執行以下步驟3e。

      <!--
     Is this accurate?
     -->

      >[!TIP]
      >   
      >* 如果問題是使用請求隊列建立的，則新項目會繼承請求隊列的組。
      >* 如果問題是通過將其添加到項目的「問題」部分而建立的，則新項目會繼承組（如果問題的項目）。


   * 若要使用範本將問題轉換為專案，請執行下列其中一項操作：

      * 按一下問題名稱，然後按一下 [!UICONTROL **更多**] 功能表 ![](assets/more-icon.png) 問題名稱的右側

         ![](assets/issue-more-menu-expanded-with-convert-to-project-options-nwe-350x213.png)

         或

      * 在問題清單中選取問題，在報表或控制面板中按一下 **更多** 功能表 ![](assets/more-icon.png) 在清單頂端，按一下 **從模板轉換為項目** 並在 **搜尋範本** 框中，然後按一下顯示在清單中的模板名稱。 繼續步驟3。

         <!--      
        (is this accurate?)      
        -->
      >[!TIP]
      >
      >如果您將範本新增至我的最愛清單，可將滑鼠移至 [!UICONTROL **最喜愛的範本**] ，然後按一下您要使用的範本。

      隨即顯示「從範本新增專案」方塊。

      ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

      >[!TIP]
      >
      >如果問題與審批流程相關聯或已與解決對象關聯，則Workfront在「轉換為項目」(Convert to Project)框的頂部顯示警告，通知您將刪除審批，或在轉換期間覆蓋解決對象。 如需詳細資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).


1. （條件性）如果您選取使用範本將問題轉換為專案，請繼續下列步驟：

   1. 檢閱右側的範本詳細資訊。

      範本詳細資訊包括：

      * 範本持續時間
      * 範本擁有者
      * 包括前三個任務名稱的頂層任務數
      * 模板中所有任務的數量
      * 範本自訂表單的名稱
   1. （可選）將滑鼠移至範本名稱上方，然後按一下我的最愛圖示 ![](assets/favorites-icon-small.png) 將其標示為收藏供將來使用。

      >[!TIP]
      >
      >您最多可以有40個Workfront項目標示為我的最愛。 這包括範本和其他項目。

   1. 按一下 [!UICONTROL **使用範本**] 來選擇模板。

      此 [!UICONTROL 轉換為專案] 框。

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. 如果範本中已填入欄位，則會在 [!UICONTROL 轉換為專案] 框。 您可以編輯預先填入的值，以更符合您的專案。 如需詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* 您的系統或群組管理員可以新增或移除 [!UICONTROL 「轉換為專案」方塊] 更新 [!UICONTROL 版面範本].
      >
      >* 若要更新 [!UICONTROL 金融] 區段 [!UICONTROL 轉換為專案] 框 [!UICONTROL 編輯] 存取 [!UICONTROL 財務資料] 在您的存取層級。 若您有 [!UICONTROL 檢視] 存取 [!UICONTROL 財務資料] 在訪問級別中，模板中的所有財務資訊都會傳輸到新項目，而轉換問題時無法對其進行編輯。 如需詳細資訊，請參閱 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 和 [共用範本](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).


   1. （選用和條件式）按一下 [!UICONTROL **選項**] 在左側面板中，從可用的選項中選取：

      * [!UICONTROL **保留原始問題，並將其解決方案與本項目聯繫起來**]

         取消選取時，會刪除原始問題。

         >[!NOTE]
         >
         >無權存取或刪除問題的使用者在轉換問題時，無法刪除問題，無論此設定的狀態為何。 如需關於問題的存取權和權限的資訊，請參閱：
         >
         >* [授予問題的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
         > 
         >* [共用問題](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


      * [!UICONTROL **允許（用戶名）擁有此項目的訪問權限**]

         如果未選取，則會出現問題 [!UICONTROL 主要連絡人] 無權訪問新任務。

         >[!NOTE]
         >
         >此處可用的選項取決於Workfront管理員為系統中每個人或您的群組設定這些選項的方式。 如需詳細資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
         >
         >
         >或者，如果您組織中的頂層群組已個別設定，此處可用的選項取決於您在步驟6中為新專案選取的群組。 如需詳細資訊，請參閱 [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).
   1. 按一下 [!UICONTROL **自訂Forms**] 並執行下列任一操作：

      * 檢閱附加至範本的自訂表單。 他們會轉到新項目。
      * 請確定所有必填欄位都具備有效資訊。
      * 拖曳自訂表單以重新排清單單 ![](assets/drag-object-icon.png) 你想要的。
      * 按一下 **x** 表徵圖。
      * 如有需要，將自訂表單資訊從問題傳輸至專案。

         >[!TIP]
         >
         >* 如果已將附加至問題的多物件自訂表單設定為搭配問題和專案使用，當您進行轉換時，會保留表單中儲存的所有資訊。
         >
         >* 如果您使用範本進行轉換，且附加至範本的自訂表單包含自訂欄位（亦可在附加至問題的自訂表單中找到），則問題的欄位值會用於新專案。 不過，如果問題上的自訂欄位空白，則會使用範本的值。

   1. 按一下 [!UICONTROL **轉換為專案**].

      >[!TIP]
      >
      >如果您決定刪除原始問題，現在該問題就是專案。
      >   
      >或
      >  
      >如果您決定保留原始問題，問題現在會連結至新專案，專案完成後問題就會完成。
      >
      >有些問題欄位會轉移至專案。 如果您未在先前步驟中變更，則範本中定義的大部分欄位會自動轉移至新建立的專案。 如需詳細資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).




1. （可選）視需要設定任&#x200B;何進一步的項目詳細資訊（項目擁有者、項目日期）和任務。
1. 按一下 [!UICONTROL **轉換為專案**].

   問題現在會轉換為專案。

1. 按一下 [!UICONTROL **前往專案**] 內 [!UICONTROL 成功] 通知。 這會開啟專案頁面。
