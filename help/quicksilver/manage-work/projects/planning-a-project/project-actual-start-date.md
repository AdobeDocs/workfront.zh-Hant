---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 專案實際開始日期概要
description: Adobe Workfront中的專案、任務和問題有實際開始日期。 對於任務和問題，這是標籤為進行中的日期。 對於專案而言，這是將專案上的第一個任務標示為進行中或完成的日期。
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/DWzx7-PW4nb78Q-XuI0AUjcCOFFap-f3qunguTclLpE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 530
ht-degree: 3%

---

# 專案實際開始日期概要

Adobe Workfront中的專案、任務和問題有實際開始日期。 對於任務和問題，這是標籤為進行中的日期。 對於專案而言，這是將專案上的第一個任務標示為進行中或完成的日期。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>淺色或更高</p> 
   <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視或更高專案存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或更高的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Workfront中實際開始日期的相關考量事項

* 實際開始日期位於專案、任務和問題的詳細資訊區段。
* 建立專案、任務或問題時，系統不會填入這些專案的實際開始日期。
* 實際開始日期會在專案、任務或問題上的工作實際開始時填入。
* 如果專案上的工作尚未開始，則實際開始日期不會顯示在專案詳細資訊標籤上。

  如果任務和問題詳細資訊標籤上的工作尚未開始，則實際開始日期在它們上顯示空白。

* 您可以手動修改任務或問題的實際開始日期，但無法修改專案的實際開始日期。

## 關於專案實際開始日期的考量事項

* 發生下列任何情況時，Workfront會自動設定專案的實際日期：

   * 任務受指派人會將任務的狀態從&#x200B;*New*&#x200B;變更為不等於&#x200B;*New*&#x200B;的任何其他狀態。

   * 任務受指派人變更任務的完成百分比。

     >[!IMPORTANT]
     >
     >將專案標籤為目前時，不會填入專案實際開始日期。 實際工作必須在填入專案的實際開始日期之前開始專案任務。

     在這些情況下，專案的「實際開始日期」會設定為專案上最早任務發生這些動作的日期和時間。 這表示專案實際在此日期和時間開始。

## 找出專案的實際開始日期

您可以在下列區域中找出專案的「實際開始日期」：

* 在專案的詳細資訊區段中。
* 在專案報告或檢視中，當您在報告中新增專案物件的&#x200B;**實際開始日期**&#x200B;時。

  如需有關建立報告的資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

若要在專案的詳細資訊區段中找出實際開始日期：

{{step1-to-projects}}

1. 按一下您要檢視其實際開始日期的專案。
1. 按一下左側面板中的&#x200B;**專案詳細資料**，然後移至&#x200B;**概觀**&#x200B;區段。

   ![強調的專案實際開始日期](assets/nwe-project-actual-start-date--highlighted-350x367.png)

   **實際開始日期**&#x200B;會與其他專案日期一起顯示。


