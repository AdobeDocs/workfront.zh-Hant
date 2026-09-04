---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 複製畫布控制面板
description: 您可以複製畫布控制面板以建立其變體，例如對象特定副本，而無需從頭開始重建。
author: Courtney
feature: Reports and Dashboards
source-git-commit: b66f6931ee2fe83688fb8910861af6e958d1f74f
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 4%

---

# 複製畫布控制面板

{{highlighted-preview-article-level}}

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>如果您對可能的錯誤或技術問題有回饋，請向Workfront支援提交票證。 如需詳細資訊，請參閱[聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform

您可以複製「畫布控制面板」 ，為不同的對象建立它的變體，例如高階主管控制面板的主管層級副本，而不需要從頭重新建立。

## 存取需求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td> 
<p>標準 </p> 
<p>規劃</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td><p>編輯或建立儀表板的存取權</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td><p>檢視儀表板的存取權</p>
  </td> 
  </tr>
</tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先決條件

您必須先建立控制面板，然後才能複製。

如需詳細資訊，請參閱[建立畫布控制面板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)。

## 複製控制面板

>[!NOTE]
>
>共用偏好設定不會複製到新儀表板。 如果Widget具有&#x200B;**以使用者**&#x200B;身分執行設定，則只有在您是指定的使用者或系統管理員時，該設定才會保留在復本上。

若要複製控制面板：

{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。

1. 在「**畫布控制面板**」頁面上，開啟您要複製的控制面板。

1. 在右上角，選取&#x200B;**更多** ![更多](assets/more-icon.png)圖示，然後選取&#x200B;**複製**。
   ![複製儀表板功能表選項](assets/duplicate-dashboard.png)

1. 在「**複製儀表板**」對話方塊中，輸入新儀表板的&#x200B;**名稱**，預設值為來源儀表板的名稱，其後加上「（複製）」。

1. （選擇性）在&#x200B;**儀表板詳細資料**&#x200B;索引標籤上，更新新儀表板的&#x200B;**描述**&#x200B;或&#x200B;**貨幣**。
   ![複製儀表板 — 儀表板詳細資訊標籤](assets/duplicate-details.png)

1. （選擇性）按一下&#x200B;**介面工具集**標籤，然後取消選取您不想要包含在重複儀表板中的任何介面工具集。
   ![複製儀表板 — Widget標籤](assets/copy-widgets.png)

1. （選擇性）按一下&#x200B;**篩選和提示**&#x200B;標籤，然後關閉&#x200B;**複製儀表板篩選器**&#x200B;或&#x200B;**複製儀表板提示**，以將其從重複儀表板中排除。
   ![複製儀表板 — 篩選和提示索引標籤](assets/copy-filters.png)

1. 按一下&#x200B;**複製儀表板**。

隨即顯示確認訊息，內含新控制面板的連結。
