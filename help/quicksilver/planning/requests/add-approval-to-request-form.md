---
title: 新增核准至請求表單
description: 您可以在Adobe Workfront Planning請求表單中新增核准流程，以便對每個提交的請求啟動核准，然後再建立記錄。
hide: true
hidefromTOC: true
source-git-commit: a999b805016361bdd101a6cd9c61967284a71014
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---


<!--

---
title: Add an Approval to a Request Form
description: You can add an approval process to an Adobe Workfront Planning request form, to initiate an approval for every submitted request, before it creates a record. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

-->

# 新增核准至請求表單

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning請求表單中新增核准流程，以便對每個提交的請求啟動核准，然後再建立記錄。

本文說明工作區管理員如何為與記錄型別關聯的請求表單新增核准。

如需有關在Workfront Planning中建立請求表單的資訊，請參閱[在Adobe Workfront Planning中建立和管理請求表單](/help/quicksilver/planning/requests/create-request-form.md)。

如需有關將請求提交至記錄型別以建立記錄的資訊，請參閱[提交Adobe Workfront Planning請求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。

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
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td>
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
   <p>標準</p>
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
   <ul>
   <li><p>管理工作區的許可權</p></li>
    <li><p>系統管理員可以管理他們未建立的工作區。 </p></li>
    </ul>
   <p>如需有關共用Workfront Planning物件許可權的資訊，請參閱  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">在Adobe Workfront Planning中共用許可權的概觀</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p>  
</td>
  </tr>
 </tbody>
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將核准新增至請求表單的考量事項

* 您可以將一個或多個核准者新增至請求表單。 您只能將使用者新增為核准者。
* 將多位核准者新增至請求表單時，所有核准者都必須先接受請求，才能在Workfront Planning中建立記錄。
* 將核准新增至請求表單為選用。 如果請求表單未與核准相關聯，Workfront Planning會在提交請求時立即建立記錄。

## 新增核准至請求表單

1. 開始建立記錄型別的要求表單，如[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)中所述。
1. 按一下&#x200B;**組態**。

   顯示&#x200B;**組態**&#x200B;區域。

   ![](assets/configuration-tab.png)
1. 在&#x200B;**核准者**&#x200B;欄位中，按一下下拉式圖示，然後在清單中選取一或多個名稱

   或

   開始輸入核准者的名稱，然後在其顯示在清單中時選取它。

   >[!TIP]
   >
   >    如果您新增多個核准者，則在Workfront Planning建立記錄之前，所有核准者都必須核准請求。

1. （選擇性）如果您之前從未共用過請求表單，請按一下&#x200B;**Publish**

   或

   按一下[共用]以共用表單，然後按[複製]連結&#x200B;**。******
1. （選用）使用者使用您共用的連結並提交請求後，Workfront Planning會傳送核准通知及電子郵件給核准者。

   如需核准要求的詳細資訊，請參閱[核准要求](/help/quicksilver/planning/requests/approve-request.md)。
