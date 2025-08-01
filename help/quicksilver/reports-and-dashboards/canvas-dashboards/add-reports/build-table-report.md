---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在畫布儀表板中建立表格報告
description: 您可以將表格報表新增至畫布控制面板，以使用表格格式視覺化您的資料。
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: 8b9676c7ef4efcad1294a9aa786aa6fe52d26cc0
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# 在畫布儀表板中建立表格報告

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 如需詳細資訊，請參閱[畫布控制面板Beta版資訊](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)。

您可以將表格報表新增至畫布控制面板，以使用表格格式視覺化您的資料。

![資料表報告範例](assets/table-example-main.png)

+++ 展開以檢視存取需求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td> 
<p>目前：計畫 </p> 
<p>新增：標準</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td><p>編輯報告、儀表板和行事曆的存取權</p>
  </td> 
  </tr>  
</tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先決條件

在建置表格報表之前，您必須先建立儀表板。

## 在畫布儀表板中建立表格報告

有許多組態選項可用來建置表格報告。 在本節中，我們將引導您進行建立資料庫的一般程式。

{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。

1. 按一下右上角的&#x200B;**新儀表板**。

1. 在&#x200B;**建立儀表板**&#x200B;方塊中，輸入儀表板的&#x200B;**名稱**&#x200B;和&#x200B;**描述**。

1. 按一下「**建立**」。

1. 在&#x200B;**新增報告**&#x200B;方塊中，選取&#x200B;**建立報告**。

1. 在左側，選取&#x200B;**表格**。

1. 按一下右上角的&#x200B;**建立報告**。

1. （選擇性）請依照下列步驟設定&#x200B;**詳細資料**&#x200B;區段：

   1. 輸入報告&#x200B;**名稱**。

   1. 輸入報告&#x200B;**描述**。

1. 請依照下列步驟設定&#x200B;**組建資料表**&#x200B;區段：

   1. 在左側面板中，按一下&#x200B;**表格欄** ![建置表格圖示](assets/drilldown-column.png)圖示。

   1. 按一下&#x200B;**新增欄**，然後選取您要在表格中顯示為欄的欄位。 欄會顯示在右側的預覽區段中。

   1. 對要新增的每個欄重複上述步驟。

1. 請依照下列步驟設定&#x200B;**篩選器**&#x200B;區段：

   1. 在左側面板中，按一下&#x200B;**篩選器** ![篩選器圖示](assets/filter-icon.png)圖示。

   1. 選取&#x200B;**編輯篩選器**。

   1. 按一下&#x200B;**新增條件**，然後指定您要篩選的欄位，以及定義欄位必須符合何種條件的修飾元。 欄會顯示在右側的預覽區段中。

1. （選擇性）按一下&#x200B;**新增篩選器群組**&#x200B;以新增另一組篩選准則。 集合之間的預設運運算元為AND。 按一下運運算元以將其變更為OR。

1. 請依照下列步驟設定&#x200B;**向下鑽研群組設定**&#x200B;區段：

   1. 在左側面板中，按一下&#x200B;**群組設定** ![群組設定圖示](assets/drilldown-group-icon.png)圖示。

   1. 按一下「**新增群組**」按鈕，然後選取要建立為群組的欄位。 群組欄會顯示在右側的預覽區段中。

1. 按一下&#x200B;**儲存**&#x200B;以建立報告並將其新增到儀表板。