---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Grouping：指出應使用文字模式收合或展開群組結果
description: 群組：指出群組結果應使用文字模式收合或展開
author: Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# 群組：指出群組結果應使用文字模式收合或展開

<!--Audited: 10/2024-->

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

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>修改篩選器的貢獻者或請求 </p>
   <p>要修改報告的標準或計畫</p>
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

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 指示群組結果應使用文字模式收合或展開

1. 移至物件清單。
1. 從&#x200B;**群組**&#x200B;下拉式功能表中，選取&#x200B;**新群組**。

1. 新增群組，然後按一下&#x200B;**切換到文字模式**。

   或

   如果群組已處於文字模式，請將下列程式碼新增至您要摺疊顯示的群組層級：

   `group.0.iscollapsed=true`

1. （選擇性）如果要展開群組顯示，請將下列程式碼新增至適當的群組層級：

   `group.0.iscollapsed=false`

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存群組**。
1. （選擇性）更新群組的名稱，然後按一下&#x200B;**儲存群組**。
