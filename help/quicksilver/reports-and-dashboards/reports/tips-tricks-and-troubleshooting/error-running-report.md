---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 執行報告時的錯誤訊息：「您目前未登入。」
description: 瞭解「您目前未登入」錯誤訊息。
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 6%

---

# 執行報告時的錯誤訊息：「您目前未登入。」

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
     <p>標準</p>
     <p>工作或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 問題

執行報表或在控制面板中顯示報表時，系統傳回下列錯誤：\
*請再試一次。您目前未登入。*

報表中未顯示任何結果。

## 原因

報表目前設定為以停用使用者的身分執行。

## 解決方案

您必須擁有報表的管理許可權才能變更報表設定。\
若要調整報表並檢視結果：

1. 移至報表。
1. 按一下&#x200B;**報告動作** > **編輯** > **報告設定**。

1. 在&#x200B;**執行此報告的存取許可權欄位中，指定作用中使用者的名稱：**。\
   或\
   將&#x200B;**以**&#x200B;欄位的存取許可權執行此報告，請保留空白。

1. 按一下「**完成**」。
1. 按一下「**儲存並關閉**」。\
   執行此報告時，錯誤不應再次出現。
