---
title: 使用版面配置範本的品牌Adobe Workfront
user-type: administrator
product-area: system-administration;templates
navigation-topic: layout-templates
description: 身為Adobe Workfront管理員或群組管理員，您可以使用版面配置範本來自訂頂端導覽區域以及[主要]功能表中特定群組、團隊、工作角色和使用者的標誌。 這對於擁有品牌的大型組織中的群組特別有用。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ded9ab1e-c5f4-476b-ac81-0497dbe6b24d
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 使用版面配置範本的品牌Adobe Workfront

<!--Audited: 09/2024-->

{{preview-fast-release-general}}

>[!IMPORTANT]
>
>此頁面上說明的程式僅適用於尚未上線到[!DNL Adobe Experience Cloud]的組織。
>
> 如果您的組織已上線到[!DNL Adobe Experience Cloud]，則無法使用品牌化。

您可以使用版面配置範本來自訂頂端導覽區域和[主要]功能表中特定群組、團隊、工作角色和使用者的標誌。 這對於擁有品牌的大型組織中的群組特別有用。

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

>[!NOTE]
>
>Workfront管理員可在系統層級對整個組織進行相同的品牌自訂，如[品牌化您的Adobe Workfront執行個體](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)中所述。 但版面配置範本中的品牌化會覆寫系統層級的品牌化。

<!-- Maybe add a section about deleting these 2 settings to revert to default branding? -->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。</p>
        <p>若要為群組執行這些動作，您必須是該群組的管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用版面配置範本的品牌Adobe Workfront

1. 開始使用版面配置範本，如[建立和管理版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 按一下![自訂使用者看到的內容](assets/dropdown-arrow.png)下的向下箭頭&#x200B;**向下箭頭**，然後按一下&#x200B;**品牌**。
1. 進行下列任何變更，以使用指派此版面配置範本的使用者品牌影像來自訂Workfront。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>品牌首頁圖示<span style="font-weight: normal;"> （顯示在頂端導覽區域的最左側）</span></p> </td> 
      <td> <p>在<strong>上層導覽區域</strong>區段的<strong>首頁圖示</strong>下，按一下方塊中的任何位置，然後尋找並選取您的標誌影像。 或將影像拖曳至方塊。</p> <p>若要裁切影像，請使用捲動控制項，並將影像拖曳至您想要在指定空間內的位置。</p> <p>建議使用120 x 120影像。 其格式可為下列任一：GIF、JPG、PNG、SVG。</p> <p>此圖示也會顯示在使用者匯出為PDF檔案的報告、清單、控制面板以及傳遞的報告中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>標籤主要功能表<img src="assets/main-menu-icon.png">標誌<span style="font-weight: normal;"> （顯示在主要功能表的右上角）</span></p> </td> 
      <td> <p> <p> <p>在<strong>頂端導覽區域</strong>區段的<strong>主功能表標誌</strong>下，按一下方塊中的任何位置，然後尋找並選取您的標誌影像。 或將影像拖曳至方塊。</p> <p>若要裁切影像，請使用捲動控制項，並將影像拖曳至您想要在指定空間內的位置。</p> <p>建議使用300 x 120畫素的影像。 其格式可為下列任一：GIF、JPG、PNG、SVG。</p> </p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. <span class="preview">在預覽環境中：繼續自訂版面範本。 您可以隨時按一下&#x200B;**套用**&#x200B;以儲存進度。</span>

   <span class="preview">或</span>

   <span class="preview">如果您已完成自訂，請按一下&#x200B;**儲存並關閉**。</span>

1. 在生產環境中：繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下&#x200B;**儲存**。

   >[!TIP]
   >
   >您可以隨時按一下[儲存]來儲存進度，然後再繼續修改範本。****

如需配置範本的詳細資訊，請參閱[建立和管理配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。
