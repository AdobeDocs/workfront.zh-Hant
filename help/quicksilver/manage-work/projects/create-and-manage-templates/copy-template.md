---
product-area: templates
navigation-topic: templates-navigation-topic
title: 複製專案範本
description: 除了從頭開始建立專案範本外，您也可以複製現有範本並加以修改。
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: 0d968a3f398c2e7dc4154cd5a16acf35ca7c86f5
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 2%

---

# 複製專案範本

<!--Audited: 5/2025-->

除了從頭開始建立專案範本外，您也可以複製現有範本並在Adobe Workfront中加以修改。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td><p>新增：標準</p> 
   <p>目前：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯範本的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視或更高的範本許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 複製範本的考量事項

下列專案一律會從現有範本複製到新範本：

* 範本任務
* 範本任務預設資訊(任務預設核准流程、任務預設自訂Forms)
* 自訂表單
* 風險
* 佇列設定資訊
* Portfolio與程式
* 核准
* 文件
* 原始範本任務轉移到新範本的天數。 如果需要，您必須變更範本的開始或完成日期（視其排程模式而定）以更新範本任務的日期。

下列專案絕不會從現有範本複製到新範本：

* 計費費率
* 使用者註解

## 複製範本


<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. 前往您要複製的範本。
1. 按一下標題中範本名稱右側的&#x200B;**更多**&#x200B;功能表![更多圖示](assets/qs-more-icon-on-an-object.png)，然後按一下&#x200B;**複製**。

   **複製範本**&#x200B;方塊開啟。

   <!--![Copy template box](assets/copy-template-box.png)-->

1. 在&#x200B;**新範本名稱**&#x200B;欄位中指定範本的名稱。

   依預設，新名稱為`Copy of Original template name`。

1. 如果要將所有來自原始範本的任務和範本指派傳送到新範本，請選取&#x200B;**保留使用者在任務或範本上的指派**&#x200B;選項。 範本任務指派，以及範本擁有者和贊助者會轉移到複製的範本。
1. 按一下[儲存]**以建立範本的復本。**

   新範本會顯示在Workfront的「範本」區域的範本清單中。
