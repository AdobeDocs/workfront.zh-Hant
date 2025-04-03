---
product-area: resource-management
navigation-topic: resource-planning
title: 使用連結共用資源規劃工具使用者檢視
description: Adobe Workfront可以為資源規劃工具的使用者檢視產生唯一的URL，您可將該URL作為外部頁面嵌入到儀表板中，或在新的瀏覽器標籤中單獨將其開啟。 當與可能沒有資源區域的直接存取許可權的使用者共用資源規劃工具資訊時，這會很有幫助。
author: Lisa
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: af0f1b9baef20c5910b13a52207531887a8524c5
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# 使用連結共用資源規劃工具使用者檢視

Adobe Workfront可以為資源規劃工具的使用者檢視產生唯一的URL，您可將該URL作為外部頁面嵌入到儀表板中，或在新的瀏覽器標籤中單獨將其開啟。 當與可能沒有資源區域的直接存取許可權的使用者共用資源規劃工具資訊時，這會很有幫助。

![具有連結的使用者檢視](assets/rp-user-view-with-link-highlight-350x49.png)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
    <td><p>新增：任何</p>
       <p>或</p>
       <p>目前：Pro或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視或更高的資源管理、專案和使用者存取權</p> <p>檢視財務資料的存取權以檢視成本資訊</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視或更高許可權給您要在資源規劃工具中顯示的專案</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

為資源規劃工具的使用者檢視產生唯一URL時，請考量下列事項：

* 您只能取得使用者檢視的唯一URL。 專案或角色檢視中不存在產生URL的選項。
* 您可以與其他使用者共用URL，包括「工作」和「檢閱」授權使用者。\
  他們必須有權檢視其他使用者，才能從您與他們共用的URL檢視資源規劃工具中的資訊。
* 當您與其他使用者共用URL時，會儲存下列資訊：

   * 時間週期型別（周、月、季）。
   * 您套用的篩選器。
   * 顯示型別（時數或FTE）。

若要在資源規劃工具的使用者檢視中取得唯一URL並與其他使用者共用：

{{step1-to-resourcing}}

1. 選取&#x200B;**依使用者檢視**。
1. （選擇性）選取您要在資源規劃工具中檢視資訊的時間範圍。 從下列選項中選取：

   * 週
   * 月
   * 季度

1. （選擇性）選取您要依&#x200B;**FTE**&#x200B;或&#x200B;**小時**&#x200B;檢視資訊。\
   ![選取FTE或時數](assets/rp-hours-or-fte-in-user-view.png)

1. （選用）將篩選器套用至資源規劃工具。\
   如需套用篩選的詳細資訊，請參閱[資源規劃工具中的篩選資訊](../../resource-mgmt/resource-planning/filter-resource-planner.md) 。

1. 按一下&#x200B;**超連結**&#x200B;圖示。\
   ![超連結圖示和URL](assets/rp-generate-url-from-link-icon.png)

1. 按一下&#x200B;**複製URL**。\
   這會將使用者檢視中資源規劃工具的唯一URL複製到剪貼簿。

1. （可選）執行下列任一項作業：

   * 將URL貼到另一個應用程式中，以傳送給另一個使用者。\
     使用者必須登入Workfront才能在使用者檢視中檢視資源規劃工具。
   * 開啟新的瀏覽器標籤或視窗，並貼上您複製的連結，然後在鍵盤上按一下Enter以在新標籤或視窗中開啟「資源規劃工具」。
   * 執行下列動作：

     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. 移至&#x200B;**報告**>**儀表板**>**新儀表板**>**新增外部頁面。**

      1. 在&#x200B;**URL**&#x200B;欄位中貼上您複製到剪貼簿的連結。
      1. 按一下&#x200B;**儲存**，然後按一下&#x200B;**儲存+關閉**。\
         這會將URL內嵌到儀表板中，並且資源規劃工具的使用者檢視會顯示在單獨的儀表板中。

1. （可選）如果您將URL內嵌到儀表板中，請考慮將其新增到版面配置範本，或與其他可能沒有資源管理區域存取權的使用者共用。\
   如需將儀表板新增到版面配置範本的相關資訊，請參閱[建立和管理版面配置範本](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) 。\
   如需關於共用儀表板的資訊，請參閱[共用儀表板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) 。\
   檢視共用URL時，使用者可以看到包含您最初套用至資源規劃工具之設定的資訊。 使用者必須登入Workfront才能檢視共用URL。\
   ![已顯示資源規劃工具之範例儀表板](assets/user-view-dashoard-from-unique-url-350x85.png)
