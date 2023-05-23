---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分組：指示是否應使用文本模式折疊或展開分組結果'
description: '分組：指示是否應使用文本模式折疊或展開分組結果'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# 分組：指示是否應使用文本模式折疊或展開分組結果

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

您可以使用標準報表生成器指示分組中的結果是否應在清單或報表中顯示折疊或展開。 預設情況下，結果會展開分組顯示。 有關建立分組的資訊，請參閱 [在Adobe Workfront建立分組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* 當您在查看清單時手動調整分組時，Adobe Workfront會記住您的手動首選項，直到您註銷。 當您重新登錄時，會根據此設定顯示清單。
>* 從圖表元素訪問分組結果後，始終顯示已展開的分組結果。
>


還可以指示分組應使用文本模式顯示展開還是折疊。

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
   <td> <p>請求修改分組 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改分組</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 指示是否應使用文本模式折疊或展開分組結果

1. 轉到對象清單。
1. 從 **分組**&#x200B;下拉菜單，選擇 **新建分組**。

1. 添加分組並按一下 **切換到文本模式**。

   或

   如果分組已處於文本模式，請將以下代碼添加到要顯示折疊的分組級別：

   ```
   group.0.iscollapsed=true
   ```

1. （可選）如果要顯示擴展的分組，請將以下代碼添加到相應的分組層：

   ```
   group.0.iscollapsed=false
   ```

1. 按一下 **完成**，則 **保存分組**。
