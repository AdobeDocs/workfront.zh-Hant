---
product-area: documents
navigation-topic: approvals
title: 設定AI檢閱者的品牌
description: 設定AI檢閱者的品牌
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
source-git-commit: 07b401c70dfd209d13c34cf62844f334f3260af1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 5%

---

# 設定AI檢閱者的品牌

>[!IMPORTANT]
>
>此功能目前處於Beta測試階段。

AI稽核者在稽核程式期間使用品牌指南來評估內容。 您可以上傳包含品牌方針的PDF檔案或手動輸入品牌元素，在Workfront中建立品牌。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是系統管理員。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console許可權*</td> 
   <td> <p>您必須使用GenStudio Brand Manager。</p>
    <p>注意：若要選取GenStudio Brand Manager，您必須遵循<a href="https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/intro/configure-brand-permissions">指派品牌許可權</a>中概述的步驟。</p>
   </td> 
  </tr> 
 </tbody> 
</table>





如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 先決條件

* 貴組織必須已移轉至Adobe IMS (Identity Management系統)。
* 您的Workfront執行個體必須已啟用統一核准。
* 您的組織必須有GenStudio Foundation。
* Adobe必須有已簽署的Adobe Gen AI合約檔案。
如需簽署合約的詳細資訊，請參閱[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。


## 使用PDF建立品牌

{{step-1-to-setup}}

1. 在左側面板中，移至&#x200B;**檢閱和核准** > **品牌**。
1. 按一下熒幕右上角的&#x200B;**新增品牌**。
1. 為品牌命名。
1. 按一下「上傳PDF」以上傳品牌檔案。
   ![上傳品牌PDF](assets/upload-PDF.png)
1. 按一下「**繼續**」。
1. 上傳一或多個包含品牌准則的PDF檔案，然後按一下[新增品牌]。****
1. 上傳檔案後，請檢閱擷取的品牌元素，以確保其符合您的品牌方針。

   >[!IMPORTANT]
   >
   >准則是使用您的檔案和產生式AI技術產生的，可能不準確。 請檢閱擷取的准則，找出缺少或不正確的詳細資料，並在發佈此品牌之前加以編輯。

1. 完成時，按一下&#x200B;**發佈**，讓AI檢閱者可以使用品牌。

## 手動建立品牌

{{step-1-to-setup}}

1. 在左側面板中，移至&#x200B;**檢閱和核准** > **品牌**。
1. 按一下熒幕右上角的&#x200B;**新增品牌**。
1. 為品牌命名。
1. 按一下&#x200B;**手動新增**&#x200B;以建立具有個別元素的品牌。
1. 視需要填寫品牌詳細資訊。 您可以新增下列元素：

   <table>
    <tr>
        <td>使用時機</td>
        <td>讓行銷人員知道何時該使用此品牌。</td>
    </tr>
    <tr>
        <td>語音准則</td>
        <td>提供品牌語調和風格的指引。</td>
    </tr>
    <tr>
        <td>影像指導方針</td>
        <td>指定符合品牌識別的影像型別。</td>
    </tr>
    <tr>
        <td>頻道准則</td>
        <td>概述品牌通訊的適當管道。</td>
    </tr>
    <tr>
        <td>標誌</td>
        <td>包含與品牌相關的官方標誌。</td>
    </tr>
    <tr>
        <td>顏色</td>
        <td>指定品牌的調色盤。</td>
    </tr>
    </table>

   ![手動新增品牌元素](assets/brand-elements.png)


1. 完成時，按一下&#x200B;**發佈**，讓AI檢閱者可以使用品牌。
