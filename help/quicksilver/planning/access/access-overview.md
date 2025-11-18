---
title: Adobe Workfront計畫存取許可權總覽
description: 並非組織中的所有使用者都有相同的存取權和許可權來使用Adobe Workfront Planning。 本文說明使用者必須使用Adobe Workfront Planning功能的存取權和許可權。
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 2%

---


# Adobe Workfront Planning存取權概觀

<!--leave the global record type reference in yellow till Jan 2026-->

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

>[!IMPORTANT]
>
>本文資訊說明Adobe Workfront的額外功能Adobe Workfront Planning。
>
>貴公司必須購買其他套件，Workfront Planning才能存取其功能。
>
>如需詳細資訊，請聯絡您的客戶經理
>
>如需Workfront Planning的詳細資訊，請參閱[開始使用Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)。

使用 Adobe Workfront 規劃有授權和分享權限限制。

本文說明你使用前線規劃功能所需的存取權限與設定。

## 存取需求

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

您必須具備以下權限才能使用 Workfront Planning：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
 <tr>
   <td role="rowheader"><p>Adobe Workfront 套件</p></td>
   <td>
   <p>任何Workfront和Planning套件</p>
   <p>任何工作流程和Planning套件</p>

<p><b>附註</b></p>

<p>若要存取可連線的記錄型別：</p>
   <ul><li><p>任何 Workfront 套件和規劃套件</p></li>
   <li><p>任何工作流程與規劃 Prime 和 Ultimate 套件</p></li></ul>

<div class="preview">
   <p>若要存取全域記錄型別：</p>
   <ul><li><p>任何Workfront套件和Planning Plus套件</p></li>
   <li><p>任何Workflow套件和Planning Prime與Ultimate套件</p></li></ul> </td></tr>
   </div>
   <tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
   <p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p>
   <p><b>重要</b></p>
   <p>只有新增至Adobe Identity Management系統(IMS)的使用者才能獲得許可權並新增至Planning欄位。</p>
   <p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <ul><li><p>任一，若要檢視Workfront Planning資訊</p></li>
   <li><p>標準，建立工作區和檢視</p></li></ul>
    </td>
  </tr>
  <tr>
   <td role="rowheader"><p>存取層級配置</p></td>
   <td> <p>Adobe Workfront 規劃沒有存取層級的控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>物件權限</p></td>
   <td>
   <ul>
   <li><p>對於你未建立的工作區、記錄類型和檢視，還要有更高的權限來存取它們及其物件。</p></li>
   <li><p>貢獻或更高的權限到你未建立的工作區和紀錄類型，以便編輯它們，並建立、編輯或刪除記錄類型和紀錄。</p></li>
   <li><p>為您未建立的檢視貢獻或更高的許可權，以編輯、刪除和共用檢視</p>
   </li>
    <li><p>系統管理員可以管理他們未建立的工作區。 </p></li>
    <li><p>系統管理員無法存取他們未建立的檢視。 </p></li></ul>
   <p>關於工作前端規劃物件權限共享的資訊，請參見 
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront 規劃中共享權限的概述</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 
<p>標準使用者與系統管理員預設已啟用規劃區域。</p>
<p> 必須為具有輕度或貢獻者授權的使用者指派包含下列區域中Planning選項的版面配置範本：</p>
   <ul><li>主要功能表</li>
   <li>專案、投資組合和方案的左側面板</li>
   </ul>   
</td>
  </tr>
 </tbody>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


## 使用版面配置範本共用Planning區域

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

標準使用者和系統管理員預設會在下列區域中啟用Planning區域：

* 主要功能表
* 左側面板為專案、作品集或計畫

如果你有其他 Workfront 授權，且需要貢獻 Workfront 規劃工作，系統管理員必須將規劃區域加入你。

管理員可以透過修改並指派你到版面模板，為以下區域新增規劃選項：

* 主選單
* 登陸頁面
* 專案、投資組合和計畫的左側面板
* 圖釘

若要從Workfront例項的使用者中新增或移除Workfront Planning區域：

1. 以Workfront管理員身分登入&#x200B;**Workfront**。

1. 移至&#x200B;**主功能表** > **設定** > **介面** > **配置範本**，然後開啟或建立配置範本。

   如需有關自訂版面配置範本的資訊，請參閱[建立和管理版面配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

1. 將版面配置範本指派給您要存取Workfront Planning的使用者。

   如需詳細資訊，請參閱[將使用者指派給配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

   所有指派給範本的使用者現在都可以在其主要功能表中存取Workfront Planning 。

   使用者可以開始建立工作區、記錄型別、記錄和欄位。

## 指派授權給使用者

您可以在編輯或建立使用者時設定其存取層級時，為其指派授權。

如需詳細資訊，請參閱[編輯使用者的設定檔](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)

## 設定存取層級

Workfront計畫沒有Workfront存取層級控制項。

擁有任何類型的 Workfront 授權的使用者都能存取 Workfront 規劃。

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 授權

你可以在 Workfront 規劃中授予以下實體權限：

* 工作區
* 記錄類型
* 檢視

如需詳細資訊，請參閱[在Adobe Workfront Planning中共用許可權的總覽](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

您的Adobe Workfront授權型別與Workfront Planning許可權搭配使用，可讓您檢視、貢獻或管理Workfront Planning物件。

如需授權型別如何影響Workfront Planning物件許可權等級的資訊，請參閱[使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)。


