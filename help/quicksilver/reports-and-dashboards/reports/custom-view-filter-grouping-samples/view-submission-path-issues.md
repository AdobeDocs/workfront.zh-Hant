---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：問題的提交路徑'
description: 您可以在問題報告的檢視中顯示提交問題的路徑。 路徑指示問題最初提交所在的隊列、主題組和隊列主題。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# 查看：問題提交路徑

您可以在問題報告的檢視中顯示提交問題的路徑。 路徑指示問題最初提交所在的隊列、主題組和隊列主題。

![issue_submission_path.png](assets/issue-submission-path-350x66.png)

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

## 檢視問題的提交路徑

1. 前往問題清單。
1. 從 **檢視** 下拉式功能表，選取 **新建視圖**.

1. 在&#x200B;**欄預覽** 按一下 **添加列**.

1. 按一下新欄的標題，然後按一下 **切換到文本模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在&#x200B;**文字模式**&#x200B;框中，並將其替換為以下代碼：

   <pre>displayname=問題路徑<br>linkedname=direct <br>namekey=displayQueueBreadcrumb <br>valuefield=displayQueueBreadcrumb <br>valueformat=HTML<br></pre>

1. 按一下 **保存視圖**.
