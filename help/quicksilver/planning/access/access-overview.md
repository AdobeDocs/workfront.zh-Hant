---
title: Adobe Workfront計畫存取許可權總覽
description: 並非組織中的所有使用者都有相同的存取權和許可權來使用Adobe Workfront Planning。 本文說明使用者必須使用Adobe Workfront Planning功能的存取權和許可權。
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 3550d7addcc0bb790f15d141d9470e0b75f940a6
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 2%

---


# Adobe Workfront Planning存取權概觀

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

>[!IMPORTANT]
>
>本文資訊說明Adobe Workfront的額外功能Adobe Workfront Planning。
>
>貴公司必須購買Workfront Planning的額外授權，才能存取其功能。
>
>如需詳細資訊，請聯絡您的客戶經理
>
>如需Workfront Planning的詳細資訊，請參閱[Adobe Workfront Planning概觀](/help/quicksilver/planning/general/planning-overview.md)。

使用Adobe Workfront Planning時，有授權和共用許可權限制。

本文說明使用Workfront Planning功能所需的存取權和設定。

## 存取需求

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

您必須具有下列存取權才能存取Workfront Planning：

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
<p>下列任一Workfront Planning計畫：</p>
<ul><li>計畫</li>
<li>Planning Plus</li>
</ul>
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning的所有功能。</p>
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權*</p></td>
   <td>
   <ul><li><p>標準、光源或貢獻者，用於檢視Workfront Planning資訊</p></li>
   <li><p>標準，建立工作區和檢視</p></li></ul>
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
   <li><p>檢視或更高的工作區許可權、<span class="preview">記錄型別</span>以及您未建立用來存取它們及其物件的檢視。</p></li>
   <li><p>為工作區<span class="preview">和記錄型別</span>貢獻或更高的許可權，而您並未建立這些記錄型別來編輯它們，以及建立、編輯或刪除記錄型別和記錄。</p></li>
   <li><p>為您未建立的檢視貢獻或更高的許可權，以編輯、刪除和共用檢視</p>
   </li>
    <li><p>系統管理員可以管理他們未建立的工作區。 </p></li>
    <li><p>系統管理員無法存取他們未建立的檢視。 </p></li></ul>
   <p>如需有關共用Workfront Planning物件許可權的資訊，請參閱  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">在Adobe Workfront Planning中共用許可權的概觀</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <div class="preview">
<p>標準使用者和系統管理員預設會啟用Planning區域。</p>
<p> 必須為具有輕度或貢獻者授權的使用者指派包含下列區域中Planning選項的版面配置範本：</p>
   <ul><li>主要功能表</li>
   <li>專案、投資組合和方案的左側面板</li>
   </ul>
   <p>如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">建立及管理配置範本</a>。</p>
   </div>
   <p><b>附註</b></p>
   <p>在「生產」環境中，所有使用者（包括系統管理員）都必須指派給包含Planning區域的版面配置範本。</p>
</td>
  </tr>
 </tbody>
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


## 使用版面配置範本共用Planning區域

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

貴組織購買額外的Workfront Planning授權後，系統管理員可以將Planning選項新增至下列區域，方法是修改並指派給版面配置範本：

* 主功能表
* 登陸頁面
* 專案、投資組合和計畫的左側面板
* 圖釘

<div class="preview">

標準使用者和系統管理員預設會在下列區域中啟用Planning區域：

* 主要功能表
* 專案、專案組合或方案的左側面板

</div>

若要新增<span class="preview">或移除Workfront執行個體使用者的</span>個Workfront Planning區域：

1. 以Workfront管理員身分登入&#x200B;**Workfront**。

1. 移至&#x200B;**主功能表** > **設定** > **介面** > **配置範本**，然後開啟或建立配置範本。

   如需有關自訂版面配置範本的資訊，請參閱[建立和管理版面配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

1. 將版面配置範本指派給您要存取Workfront Planning的使用者。

   如需詳細資訊，請參閱[將使用者指派給配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

   所有指派給範本的使用者現在都可以在其主要功能表中存取Workfront Planning 。

   使用者可以開始建立工作區、記錄型別、記錄和欄位。

## 授予存取權

Workfront Planning沒有Workfront存取控制。

擁有任何型別Workfront授權的使用者皆可存取Workfront Planning。

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 授予許可權

您必須授予使用者許可權，讓使用者存取您為其建立的Workfront Planning工作區和檢視。

如需詳細資訊，請參閱[在Adobe Workfront Planning中共用許可權的總覽](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

您的Adobe Workfront授權型別與Workfront Planning許可權搭配使用，可讓您檢視、貢獻或管理Workfront Planning物件。

如需授權型別如何影響Workfront Planning物件許可權等級的資訊，請參閱[使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)。


