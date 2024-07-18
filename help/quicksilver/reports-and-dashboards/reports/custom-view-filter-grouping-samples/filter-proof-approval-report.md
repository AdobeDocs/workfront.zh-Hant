---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 「篩選：校訂核准報告，忽略先前的校訂版本」
description: 在校訂核准報告中，您可以使用目前檔案版本篩選器以僅包含等待您核准的最新版校訂。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 篩選器：校訂核准報告以省略先前的校訂版本

在校訂核准報告中，您可以使用&#x200B;**為目前檔案版本**&#x200B;篩選器來僅包含等待您核准的目前版本的校訂。

如果您被要求核准具有多個版本的校樣，這將很有用。 當您使用目前檔案版本篩選器執行校訂核准報告時，該報告僅列出等待您核准的每個校訂的最新版本，並省略您不再需要處理的舊版本。 

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 篩選校訂核准報告以省略先前的校訂版本

1. 如果您已經有校訂核准報告，請開啟它。

   或

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   若要建立您自己的校訂核准報告，請按一下主功能表![](assets/main-menu-icon.png)，然後按一下&#x200B;**報告** ![](assets/reports-in-main-menu.png)。 按一下&#x200B;**新報告**。 在出現的清單中，捲動至&#x200B;**校訂核准**&#x200B;並按一下。 按一下&#x200B;**儲存+關閉**，輸入&#x200B;**報告名稱** （選擇性），然後按一下&#x200B;**儲存報告**。

1. 按一下&#x200B;**報告動作>編輯**。
1. 按一下&#x200B;**篩選器**，然後按一下&#x200B;**新增篩選器規則**。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 按一下&#x200B;**校訂核准**。
1. 在出現的清單中，按一下&#x200B;**目前檔案版本**。
1. 按一下Adobe Workfront左下角的&#x200B;**儲存+關閉**，然後在出現的方塊中按一下&#x200B;**儲存報表**。
