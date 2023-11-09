---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 「執行報告時出現錯誤訊息：『您目前未登入。』」
description: 瞭解「您目前未登入」錯誤訊息。
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 4%

---

# 執行報告時的錯誤訊息：「您目前未登入。」

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計畫、工作</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

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
1. 按一下 **報表動作** > **編輯** > **報表設定**.

1. 在中指定作用中使用者的名稱 **透過以下存取許可權運行此報告：** 欄位。\
   或\
   離開 **透過以下存取許可權運行此報告：** 欄位空白。

1. 按一下 **完成**.
1. 按一下 **儲存+關閉**.\
   執行此報告時，錯誤不應再次出現。
