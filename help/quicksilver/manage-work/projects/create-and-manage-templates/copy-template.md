---
product-area: templates
navigation-topic: templates-navigation-topic
title: 複製專案範本
description: 您可以複製現有範本，並視需要加以變更，而不用從頭開始建立新專案範本。
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# 複製專案範本

您可以複製現有範本，並視需要加以變更，而不用從頭開始建立新專案範本。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯範本的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視或更高的範本許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。


## 複製範本的考量事項

下列專案一律會從現有專案複製到新專案：

* 範本任務
* 範本任務預設資訊(任務預設核准流程、任務預設自訂Forms)
* 自訂表單
* 風險
* 佇列設定資訊
* Portfolio與計畫
* 核准
* 文件
* 原始範本任務轉移到新範本的天數。 如果需要，您必須變更範本的開始或完成日期（視其排程模式而定）以更新範本任務的日期。

下列專案絕不會從現有專案複製到新專案：

* 收費率
* 使用者註解

## 複製範本

1. 前往您要複製的範本。
1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png)，然後按一下 **複製**.
1. 在中指定範本的名稱 **新範本名稱** 欄位。

   依預設，新名稱為 **副本 `<original template name>`.**

1. 選取您是否要 **保留使用者在任務或範本中的指派**：選取此選項可將所有任務和範本指派從原始範本傳送到新範本。
1. 按一下 **儲存** 以建立範本的復本。
