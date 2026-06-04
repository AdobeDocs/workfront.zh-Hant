---
product-area: documents
navigation-topic: approvals
title: 建立檔案的核准工作流程範本
description: 您可以建立核准範本以簡化核准流程。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jsEcIKopi-lJOSXQitDnufu3j0AmkWkPmCXtCR0V6nk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 8%

---

# 建立檔案的核准工作流程範本

在Workfront設定區域中，擁有標準授權的使用者可以建立可重複使用的核准範本。 核准範本建立後，即可套用至物件之檔案區域中的資產。
>[!IMPORTANT]
>
>本文內容指的更新檔案核准功能僅適用於特定帳戶。 如需有關標準核准程式的資訊，請參閱[工作核准](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)中列出的文章。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td><p>使用舊版Workfront儲存空間管理核准的任何Workfront套件</p>
<p>使用Adobe雲端儲存空間管理核准的任何Workflow套件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> 
   <p>規劃</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++
ß

## 建立核准範本

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**檢閱和核准** > **核准範本**。
1. 按一下頁面右側的&#x200B;**新範本**。

1. 填寫以下詳細資料：

   <table>
     <tr>
   <td><strong>範本名稱</strong></td>
   <td>新增範本名稱。 </td>
   </tr>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>新增階段名稱。 您可以將名稱變更為描述性更強的名稱，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。</td>
   </tr>
   <tr>
   <td><strong>需要一項決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日前的工作日數</strong></td>
   <td>選擇階段啟動後核准到期的工作日數。</td>
   </tr>
   </table>

1. （選擇性）重複上一步驟，視需要新增其他階段。

   >[!NOTE]
   >
   >如果您新增多個階段，核准工作流程會依階段列出的順序進行。 完成所有必要的決定後，下一個階段會開始，而上一個階段會鎖定。

   ![檔案詳細資料](assets/new-stage.png)

1. 按一下「**儲存**」。

建立範本後，可將其套用至物件之檔案區域中的檔案，以在Workfront中開始正式的稽核和核准流程。



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
