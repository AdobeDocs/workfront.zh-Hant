---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '篩選：證明批准報告以忽略以前的證明版本'
description: 在「證明批准」報表上，您可以使用「當前文檔版本」篩選器僅包括等待批准的校樣的當前版本。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 篩選器：驗證批准報表以忽略以前的驗證版本

在「證明批准」報表上，您可以使用 **是當前文檔版本** 篩選，以僅包括等待您批准的校樣的當前版本。

例如，如果您被要求批准具有多個版本的校樣，則此功能非常有用。 使用「當前文檔版本」過濾器運行「驗證批准」報表時，此報表只列出等待您批准的每個驗證的當前版本，而省略了您不再需要處理的早期版本。 

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改篩選器</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 篩選證明批准報告以忽略以前的證明版本

1. 如果您已經有「證明批准」報告，請開啟它。

   或

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   要建立自己的校樣批准報告，請按一下主菜單 ![](assets/main-menu-icon.png)，然後按一下 **報告** ![](assets/reports-in-main-menu.png)。 按一下 **新建報表**。 在顯示的清單中，滾動到並按一下 **證明批准**。 按一下 **保存+關閉**&#x200B;的子菜單。 **報表名稱** （可選），然後按一下 **保存報告**。

1. 按一下 **報告操作>編輯**。
1. 按一下 **篩選器**，然後按一下 **添加篩選器規則**。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 按一下 **證明批准**。
1. 在顯示的清單中，按一下 **是當前文檔版本**。
1. 按一下 **保存+關閉** 在Adobe Workfront的左下角，然後按一下 **保存報告** 的子菜單。
