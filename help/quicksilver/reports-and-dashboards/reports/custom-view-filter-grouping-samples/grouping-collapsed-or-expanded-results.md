---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分組：指示是否應使用文本模式收合或展開分組的結果'
description: '分組：指示是否應使用文本模式收合或展開分組的結果'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# 分組：指示是否應使用文本模式收合或展開分組的結果

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

您可以使用標準報告建立工具，指出分組中的結果是否應顯示在清單或報告中折疊或展開。 預設情況下，會展開分組顯示。 如需建立分組的相關資訊，請參閱 [在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* 當您在檢視清單時手動調整分組時，Adobe Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
>* 從圖表元素存取群組後，其結果一律會顯示為已展開。
>


您也可以指出群組應使用文字模式顯示展開或收合。

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

## 指示是否應使用文本模式收合或展開分組的結果

1. 轉到對象清單。
1. 從 **分組**&#x200B;下拉式功能表，選取 **新分組**.

1. 新增分組並按一下 **切換到文本模式**.

   或

   如果分組已處於文本模式，請將以下代碼添加到要顯示折疊的分組級別：

   ```
   group.0.iscollapsed=true
   ```

1. （選用）如果您希望分組顯示展開，請將下列程式碼新增至適當的分組層級：

   ```
   group.0.iscollapsed=false
   ```

1. 按一下 **完成**，然後 **儲存分組**.
