---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「群組：指示群組結果應使用文字模式摺疊或展開」
description: 「群組：指示群組結果應使用文字模式摺疊或展開」
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# 群組：指出群組結果應使用文字模式收合或展開

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

您可以使用標準Report Builder來指定群組中的結果在清單或報告中應摺疊還是展開。 依預設，群組中的結果顯示為展開狀態。 如需建立群組的相關資訊，請參閱[在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* 當您在檢視清單時手動調整群組，Adobe Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
>* 從圖表元素存取群組結果後，群組結果一律展開顯示。
>

您也可以指定群組應使用文字模式顯示展開或收合。

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
   <td> <p>請求修改分組 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改群組</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 指示群組結果應使用文字模式收合或展開

1. 移至物件清單。
1. 從&#x200B;**群組**&#x200B;下拉式功能表中，選取&#x200B;**新群組**。

1. 新增群組並按一下&#x200B;**切換到文字模式**。

   或

   如果群組已處於文字模式，請將下列程式碼新增至您要摺疊顯示的群組層級：

   ```
   group.0.iscollapsed=true
   ```

1. （選擇性）如果要展開群組顯示，請將下列程式碼新增至適當的群組層級：

   ```
   group.0.iscollapsed=false
   ```

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存群組**。
