---
title: 提交Adobe Workfront規劃請求
description: 有人與您從Adobe Workfront Planning的記錄型別頁面共用請求表單的連結後，您可以新增請求以建立與請求表單相關聯記錄型別的記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 1%

---

# 提交Adobe Workfront Planning請求以建立記錄

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

{{planning-important-intro}}

有人與您從Adobe Workfront Planning的記錄型別頁面共用請求表單的連結後，您可以新增請求以建立與請求表單相關聯記錄型別的記錄。

Workfront使用者與外部使用者可以提交請求給Planning記錄型別並建立記錄。<!--double check on the external users-->

本文說明如何提交請求，將新記錄新增至記錄型別。

如需工作區管理員如何建立請求表單並將其與記錄型別關聯的資訊，請參閱[在Adobe Workfront Planning中建立和管理請求表單](/help/quicksilver/planning/requests/create-request-form.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 產品</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront規劃<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td>
   <td>
<p>下列任一Workfront計畫：</p>
<ul><li>選取</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>舊版Workfront計畫不提供Workfront計畫</p>
   </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront規劃計畫*</p></td>
   <td>
<p>任何 </p>  
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p>
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權*</p></td>
   <td>
   <p>外部、貢獻者、輕度或標準授權</p>
   <p>Workfront計畫不適用於舊版Workfront授權</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td>
   <p>如果您是Workfront使用者，可檢視工作區的或更高許可權</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>若要存取Workfront中的Planning區域，您必須被指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p>
   <p> 不過，向Workfront Planning提交請求不需要存取「計畫」區域。 </p>  
</td>
  </tr>
 </tbody>
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

必須先具備下列條件，您才能將請求提交至Workfront Planning請求表單：

* Workfront Planning中必須存在下列專案：

   * 工作區
   * 與請求表單相關聯的記錄型別。 如需詳細資訊，請參閱[在Adobe Workfront Planning中建立請求表單](/help/quicksilver/planning/requests/create-request-form.md)。

* 請求表單必須以您可以存取的方式與連結共用。 存在下列情況：

   * 如果您有Workfront帳戶，連結僅與內部人員共用，而您可以存取工作區。 Workfront以外的人員無法存取內部共用的連結。
   * 如果您沒有Workfront帳戶，連結已和外部人員共用。 Workfront使用者也可以存取與外部人員共用的連結。

* 表單的連結不可過期。

## 提交請求至Workfront Planning的考量事項

* 如果沒有表單的特定連結，您將無法存取Workfront Planning請求的請求表單。
* 將請求提交至Workfront Planning後，便無法編輯請求。
* 每個提交的請求都會針對您所使用表單的相關記錄型別，建立記錄。
* 提交請求表單所建立的記錄，無法與透過任何其他方法新增的記錄區分開來。 如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。

## 向Workfront Planning提交請求

1. 從Workfront Planning記錄型別移至與您共用的連結。

1. 更新表單中可用的欄位。 帶有星號的欄位為必填欄位。

   >[!TIP]
   >
   >   如果Workfront **主旨**&#x200B;欄位可用，它可能不會顯示在Workfront Planning中。 建議您在請求中更新儘可能多的欄位，以便新記錄新增至記錄型別時可識別。

1. 按一下&#x200B;**提交**。

   您的表單已提交，並且新記錄已新增到與表單關聯的記錄型別。
