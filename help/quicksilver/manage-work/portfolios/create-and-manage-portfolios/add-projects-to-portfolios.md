---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: 將專案新增至Portfolio
description: 我們建議您在啟動專案時，將專案新增至專案組合。 不過，您可以在產品組合期限內的任何時間將其新增至產品組合。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UkUQdW12tLqRjh5zmbwtjNfRxFwc-Uhj2gGwjmDyKb8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 689
ht-degree: 2%

---

# 將專案新增至投資組合

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

我們建議您在啟動專案時，將專案新增至專案組合。 不過，您可以在產品組合期限內的任何時間將其新增至產品組合。

將專案新增至投資組合時，請考量下列事項：

* 您只能將一個投資組合與一個專案建立關聯。
* 專案會保留在投資組合中，直到被移除或與另一個投資組合相關聯為止。
* 投資組合可包含不限數量的專案。

>[!CAUTION]
>
>在大量子物件中使用繼承的許可權時，可能無法正確套用。
>   
>為協助避免繼承許可權問題，我們建議以下事項：
>
>* 限制單一父項（投資組合或方案）下的子物件（專案）數量。 我們建議每個投資組合或計畫不超過10,000個專案。
>
>* 在較低層級的物件上套用許可權，以降低繼承深度。
>
>  例如，直接在專案層級套用許可權，而不是依賴從專案組合繼承到方案，然後繼承到專案的許可權。
>
>* 分割計畫以包含較少的專案，這會降低許可權的複雜性。
>


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td> 
   <td> <p>任何</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>標準</p> 
   <p>[!UICONTROL 計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[!UICONTROL Edit]存取權投資組合</p> <p>[!UICONTROL Edit]專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>投資組合的[!UICONTROL Manage]許可權</p> <p>[!UICONTROL Manage]專案的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## 將專案新增至投資組合

1. 前往投資組合，然後按一下左側面板中的&#x200B;**[!UICONTROL 專案]**。

   ![Portfolio與專案](assets/qs-portfolio-with-projects-350x90.png)

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
      <td> <p>新增專案。 </p> <p>如需建立專案的詳細資訊，請參閱<a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">建立專案</a>。 </p> </td> 
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
      <td> <p>請求核准專案。</p> <p>如需請求專案的詳細資訊，請參閱<a href="../../../manage-work/projects/create-projects/request-project.md">請求專案</a>。 </p> </td> 
     </tr> 
          <tr> 
      <td role="rowheader">[!UICONTROL 現有專案]</td> 
      <td> <p>新增已建立的專案。</p> </td> 
     </tr>
    </tbody> 
   </table>

   <!-- update screen shot for both kinds of storages??-->

   ![新專案下拉式清單](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. （視條件而定）如果您選取新增現有專案，**新增專案**&#x200B;方塊就會開啟。<!--check this after UI changes-->

   ![新增現有專案](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. 開始在&#x200B;**[!UICONTROL 將專案新增至此投資組合]**&#x200B;欄位中輸入專案名稱，然後當專案出現在清單中時按一下它們。 <!--check this after UI changes-->

   您可以新增多個專案。

   >[!NOTE]
   >
   >當您的組織使用舊版Workfront和Adobe雲端儲存空間存放檔案時，會出現以下情況：
   >
   >
   >* 當您將Adobe雲端儲存空間專案新增至舊版Workfront儲存空間產品組合，且該產品組合沒有附加任何檔案時，該產品組合會轉換為Adobe雲端儲存空間產品組合。
   >* 當您將Adobe雲端儲存空間專案新增至舊版Workfront儲存產品組合，且該產品組合已附加檔案，則產品組合檔案儲存空間仍會保留在Workfront儲存空間中。 不過，舊版Workfront儲存體圖示![舊版Workfront儲存體圖示](assets/legacy-storage-project-icon.png)已從產品組合中移除。
   >* 您無法將舊版Workfront儲存空間專案新增到Adobe雲端儲存空間產品組合。
   >
   >如需詳細資訊，請參閱[專案和相關物件的檔案管理概觀](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)。
   >
   >並非所有Workfront執行個體都有兩種檔案儲存型別。

1. （選擇性）如果您決定不將其新增至投資組合，請按一下專案名稱右側的&#x200B;**X**&#x200B;圖示，將其從清單中移除。

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. 按一下&#x200B;**[!UICONTROL 新增專案]**。<!--check this after UI changes-->

   您選取的一或多個專案現在與投資組合相關聯。
