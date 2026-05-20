---
product-area: programs;projects
navigation-topic: create and manage programs
title: 將專案新增至計畫
description: 您可以將專案新增至投資組合中的方案，藉此組織專案。 一個計畫內可以有多個專案，但您只能將一個計畫與專案建立關聯。 將專案新增至計畫時，會自動將其同時新增至計畫的投資組合。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1fecc4d1-4c24-495c-98f5-824e13967369
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 9a35246858141a3b69ec85be3372c7a8d9497d6e
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 2%

---

# 將專案新增至方案

<!--Audited: 05/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

您可以將專案新增至投資組合中的方案，藉此組織專案。 一個計畫內可以有多個專案，但您只能將一個計畫與專案建立關聯。

您必須先在此投資組合中建立投資組合和計畫，才能將專案新增到計畫。

將專案新增至計畫時，會自動將其同時新增至計畫的投資組合。

如需關於建立投資組合的資訊，請參閱[建立投資組合](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)。

如需有關建立程式的資訊，請參閱[建立程式](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>[!UICONTROL 標準]</p> 
   <p>[!UICONTROL 計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級</td> 
   <td> <p>[!UICONTROL Edit]對程式或更高版本的存取權</p> <p>[!UICONTROL Edit]專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>[!UICONTROL Manage]程式許可權</p> <p>[!UICONTROL Manage]專案的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access to Programs or higher</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the program</p> <p>[!UICONTROL Manage] permissions to the projects</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

## 將專案新增至現有計畫

1. 前往計畫。

   按一下左側面板中的&#x200B;**[!UICONTROL 專案]**。

1. 按一下&#x200B;**[!UICONTROL 新增專案]**，然後選取新增專案的方法。

   >[!TIP]
   >
   >當您在[!UICONTROL 里程碑]檢視中檢視專案清單時，無法新增專案。

   從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody>

   <tr> 
      <td role="rowheader">[!UICONTROL 新專案]</td> 
      <td> <p>從頭開始新增專案。 </p> <p>如需從頭開始建立專案的詳細資訊，請參閱<a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">建立專案</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 新專案（舊版儲存空間）]</td> 
      <td> <p>新增Workfront儲存專案。 </p>
      <p>只有當您的組織同時使用Workfront和Adobe雲端檔案儲存時，才會顯示選項。 您的Workfront執行個體可能沒有這兩種型別的儲存空間。</p>
      <p>如需建立專案的詳細資訊，請參閱<a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">建立專案</a>。 </p> </td> 
      </tr> 
      <tr> 
      <td role="rowheader">[!UICONTROL 從範本新增專案]</td> 
      <td> <p>使用現有範本新增專案。 </p> <p>如需從範本建立專案的詳細資訊，請參閱<a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">使用範本建立專案</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 匯入[!DNL MS Project]] </td> 
      <td> <p>新增您先前從[!DNL MS Project]匯出且儲存在電腦上的專案。 </p> <p>如需有關從[!DNL Microsoft Project]匯入以建立新專案的詳細資訊，請參閱<a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">從[!DNL Microsoft Project]</a>匯入專案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 請求專案]</td> 
      <td> <p>在您可以開始處理新專案之前，先請求核准該專案。</p> <p>如需請求專案的詳細資訊，請參閱<a href="../../../manage-work/projects/create-projects/request-project.md">請求專案</a>。 </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL 現有專案]</td> 
      <td> <p>新增已建立的專案。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （視條件而定）若您選取&#x200B;**[!UICONTROL 現有專案]**，則會開啟&#x200B;**新增專案**&#x200B;方塊。<!--check at unshimming-->

   ![將現有專案新增至方案方塊](assets/add-projects-to-programs-box.png)<!--check at unshimming-->

1. 請執行下列動作：

   1. 在&#x200B;**[!UICONTROL 新增專案]**&#x200B;方塊中，在&#x200B;**將專案新增至此方案**&#x200B;欄位中輸入專案名稱，然後當專案顯示在清單中時選取它。<!--check casing on links and buttons-->

      您可以新增多個專案。

      >[!NOTE]
      >
      >當您的組織使用舊版Workfront和Adobe雲端儲存空間存放檔案時，會出現以下情況：
      >
      >
      >* 當您將Adobe雲端儲存空間專案新增至舊版Workfront儲存空間方案，且方案沒有附加任何檔案時，方案及其產品組合會轉換為Adobe雲端儲存空間物件。
      >* 當您將Adobe雲端儲存空間專案新增至舊版Workfront儲存空間方案，且方案或產品組合已附加檔案時，方案或產品組合檔案儲存空間仍會保留在Workfront儲存空間中。 不過，舊版Workfront儲存圖示![舊版Workfront儲存圖示](assets/legacy-storage-project-icon.png)已從方案或產品組合中移除（移動專案前已附加檔案的專案）。
      >* 您無法將舊版Workfront儲存空間專案新增到Adobe雲端儲存空間方案。
      >
      >如需詳細資訊，請參閱[專案和相關物件的檔案管理概觀](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)。
      >
      >並非所有Workfront執行個體都有兩種檔案儲存型別。

   1. （選擇性）如果您決定不將專案新增至程式，請按一下專案名稱旁的&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete-icon.png)。

   1. 按一下&#x200B;**[!UICONTROL 新增專案]**。<!--check at unshimming-->

      專案顯示在方案的&#x200B;**[!UICONTROL 專案]**&#x200B;標籤中，現在與方案和方案的個別投資組合相關聯。
