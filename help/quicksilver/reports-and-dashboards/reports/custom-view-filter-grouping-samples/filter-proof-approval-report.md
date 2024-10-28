---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 「篩選：校訂核准報告以省略先前的校訂版本」
description: 在校訂核准報告中，您可以使用目前檔案版本篩選器以僅包含等待您核准的最新版校訂。
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# 篩選器：校訂核准報告以省略先前的校訂版本

<!--Audited: 10/2024-->

在校訂核准報告中，您可以使用&#x200B;**為目前檔案版本**&#x200B;篩選器來僅包含等待您核准的目前版本的校訂。

如果您被要求核准具有多個版本的校樣，這將很有用。 當您使用目前檔案版本篩選器執行校訂核准報告時，該報告僅列出等待您核准的每個校訂的最新版本，並省略您不再需要處理的舊版本。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 篩選校訂核准報告以省略先前的校訂版本

您可以為校訂核准報告建立篩選器。

1. 如果您已經有校訂核准報告，請開啟它。

   或

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   若要建立您自己的校訂核准報告，請按一下右上角的&#x200B;**主功能表**&#x200B;圖示![](assets/main-menu-icon.png)或左上角的&#x200B;**主功能表**&#x200B;圖示![](assets/lines-main-menu.png) （如果可用），然後按一下&#x200B;**報告** ![](assets/reports-in-main-menu.png)。

1. 按一下&#x200B;**新報告**。 物件型別清單隨即顯示。
1. 按一下清單中的&#x200B;**校訂核准**。
Report Builder隨即開啟。
1. 按一下&#x200B;**篩選器**，然後按一下&#x200B;**新增篩選器規則**。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 按一下&#x200B;**設定您報告的篩選規則**&#x200B;方塊內部，然後從清單中選取&#x200B;**校訂核准**。
1. 在&#x200B;**校訂核准**&#x200B;物件下的清單中，按一下&#x200B;**為目前檔案版本**。
1. 選擇等於作為篩選修飾元，然後選取True。
1. 按一下Adobe Workfront左下角的&#x200B;**儲存+關閉**，然後在出現的方塊中按一下&#x200B;**套用**。

   如果任何校訂核准符合此篩選條件，則校訂核准報告僅顯示與任何檔案當前版本關聯的校訂。
