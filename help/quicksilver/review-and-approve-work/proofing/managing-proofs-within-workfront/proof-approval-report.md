---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 使用校訂核准報告
description: 您可以使用校訂核准報告來檢視有關您環境中校訂的資訊。
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
TQID: https://experienceleague.adobe.com/ZU6Ej5QhI7v9zoAxurBz1YsFVIuVIh2a8tR2h6vYL18
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a2241fa21f51f8146c1f3725d2ba2235f8458ab4
workflow-type: tm+mt
source-wordcount: 310
ht-degree: 6%

---

# 使用校訂核准報告

您可以使用校訂核准報告來檢視有關您環境中校訂的資訊。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront套件</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront授權</p> </td> 
   <td> 
   <p>標準</p>
   <p>規劃</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>存取層級組態</strong> </td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li> <p>建立報告、儀表板和行事曆</p> </li> 
     <li> <p>建立篩選器、檢視和群組</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用校訂核准報告

{{step1-to-reports}}

1. 按一下&#x200B;**新報告**，然後捲動以選取&#x200B;**校訂核准**。

   ![校訂核准報告](assets/proof-approval-report.png)

1. （選用）新增任何其他欄位。
1. 按一下「**儲存並關閉**」。

## 其他欄位

您可以將下列欄位新增到校訂核准報告中：

* **決定日期**：顯示核准者對校訂做出決定的日期。 您也可以在校樣的列印摘要上找到此日期。
* **核准者階段**：顯示目前的階段資訊。
* **工作流程範本**：顯示附加到校訂的任何工作流程範本。 如果沒有附加範本，欄為空白。
* **等待決定**：顯示true表示最新版本尚未符合決定，若下列專案為true：

   * 校訂尚未封存
   * 核准者所在的階段為作用中
   * 校訂正在等候核准

* **校訂截止日期**：顯示校訂的截止日期。 每個階段都必須指派截止日期，才能填入此欄位。 欄位會顯示最近啟用階段的截止日期。

## 關於核准者決定欄位

「核准者決定」欄位會顯示收件者對校訂所做的決定。 在某些情況下，此欄位顯示連字型大小(-)而不是決定值，這表示收件者不再處於校訂上的決策角色。 如需詳細資訊，請參閱[核准者決定在校訂核准報告](../tips-tricks-and-troubleshooting/approver-decision-shows-hyphen.md)中顯示連字型大小。

 
