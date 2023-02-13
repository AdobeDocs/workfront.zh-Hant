---
product-area: resource-management
navigation-topic: resource-planning
title: 與連結共用資源計畫員用戶視圖
description: Adobe Workfront可以為資源規劃器的「用戶視圖」生成唯一URL，您可以將該URL作為外部頁嵌入到控制面板中，或在新瀏覽器頁簽中單獨開啟它。 與可能沒有直接訪問資源區域的用戶共用資源規劃器資訊時，此方法很有幫助。
author: Alina
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 與連結共用資源計畫員用戶視圖

Adobe Workfront可以為資源規劃器的「用戶視圖」生成唯一URL，您可以將該URL作為外部頁嵌入到控制面板中，或在新瀏覽器頁簽中單獨開啟它。 與可能沒有直接訪問資源區域的用戶共用資源規劃器資訊時，此方法很有幫助。

![](assets/rp-user-view-with-link-highlight-350x49.png)

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看或更高程度地訪問資源管理、項目和用戶</p> <p>查看對財務資料的訪問以查看成本資訊 </p> <p><b>注意</b> 如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看要在資源計畫器中顯示的項目的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。


為資源計畫員的用戶視圖生成唯一URL時，請考慮以下事項：

* 您只能為「使用者檢視」取得唯一URL。 專案或角色檢視中不存在產生URL的選項。
* 您可以與其他使用者共用URL，包括「工作」和「檢閱」授權使用者。\
   他們必須有權查看其他用戶，才能從您與他們共用的URL查看資源計畫員中的資訊。
* 當您與其他使用者共用URL時，會儲存下列資訊：

   * 時段的類型（周、月、季）。
   * 您套用的篩選。
   * 顯示類型（小時數或FTE）。

要在資源計畫員的「用戶視圖」中獲取唯一URL，並與其他用戶共用它：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **資源**.
1. 在中，選取 **按用戶查看**.
1. （可選）選擇要在資源計畫員中查看資訊的時間範圍。 從以下項目中選取：

   * 週
   * 月
   * 季度

1. （可選）選擇是否要按 **FTE** 或 **小時**.\
   ![RP_hours_or_fte_in_user_view.png](assets/rp-hours-or-fte-in-user-view.png)

1. （可選）將篩選器應用於資源計畫器。\
   如需套用篩選器的相關資訊，請參閱 [在資源計畫器中篩選資訊](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

1. 按一下 **超連結** 表徵圖。\
   ![RP_Storm_generate_URL_with_copy_URL_link.png](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. 按一下 **複製URL**.\
   這會將「用戶視圖」中資源規劃器的唯一URL複製到剪貼簿。

1. （選用）執行下列其中一項作業：  

   * 將URL貼到其他應用程式中，以將其傳送給其他使用者。\
      用戶必須登錄到Workfront，才能在「用戶」視圖中查看資源規劃器。
   * 開啟新的瀏覽器頁簽或窗口並貼上您複製的連結，然後按一下鍵盤上的Enter以在新的頁簽或窗口中開啟資源計畫器。
   * 執行下列動作：

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. 前往 **報表**>**控制面板**>**新控制面板**>**新增外部頁面。**

      1. 在 **URL** 欄位。
      1. 按一下 **儲存**，然後 **儲存+關閉**.\
         這會將URL嵌入控制面板中，資源計畫員的「用戶」視圖將顯示在單獨的控制面板中。

1. （可選）如果將URL嵌入到控制面板中，請考慮將其添加到佈局模板，或與可能沒有資源管理區域訪問權限的其他用戶共用它。\
   如需將控制面板新增至配置範本的相關資訊，請參閱 [建立和管理版面範本](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) .\
   如需共用控制面板的相關資訊，請參閱 [共用控制面板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) .\
   查看共用URL時，用戶可以查看具有您最初應用於資源規劃器的設定的資訊。 使用者必須登入Workfront才能檢視共用URL。\
   ![user_view_dashoard_from_unique_url.png](assets/user-view-dashoard-from-unique-url-350x85.png)
