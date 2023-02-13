---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '''篩選：校樣核准報表以忽略先前的校樣版本'
description: 在校樣核准報表上，您可以使用「是目前的檔案版本」篩選條件，僅包含等待您核准的校樣的最新版本。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 篩選：校樣核准報表以忽略先前的校樣版本

在「校樣核准」報表上，您可以使用 **是當前文檔版本** 篩選，僅包含等待您核准的最新版本校樣。

例如，如果您被要求核准具有多個版本的校樣，這個功能就很實用。 當您使用「為當前文檔版本」篩選器運行「校樣批准」報表時，該報表僅列出等待您批准的每個校樣的當前版本，省略了您不再需要使用的早期版本。 

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
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 篩選校樣核准報表以忽略先前的校樣版本

1. 如果您已有「證明核准」報表，請開啟它。

   或

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   若要建立您自己的校樣核准報表，請按一下主功能表 ![](assets/main-menu-icon.png)，然後按一下 **報表** ![](assets/reports-in-main-menu.png). 按一下 **新增報表**. 在顯示的清單中，捲動至並按一下 **證明核准**. 按一下 **儲存+關閉**，鍵入 **報表名稱** （可選），然後按一下 **儲存報表**.

1. 按一下 **報表動作>編輯**.
1. 按一下 **篩選器**，然後按一下 **新增篩選規則**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 按一下 **證明核准**.
1. 在顯示的清單中，按一下 **是當前文檔版本**.
1. 按一下 **儲存+關閉** 在Adobe Workfront的左下角，然後按一下 **儲存報表** 框中。
