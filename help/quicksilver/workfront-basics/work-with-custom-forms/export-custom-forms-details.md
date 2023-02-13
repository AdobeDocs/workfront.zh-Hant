---
title: 匯出自訂表單和物件詳細資訊
description: 匯出自訂表單和物件詳細資訊
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# 匯出自訂表單和物件詳細資訊

您可以從物件的「詳細資訊」區段將「概述」和自訂表單資訊匯出至PDF檔案。 然後，您可以列印PDF或與其他使用者共用。

下列物件支援此功能：

* 專案
* 任務
* 問題
* 專案組合
* 計劃

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>系統不會顯示您的Workfront或群組管理員使用配置範本移除的「詳細資訊」區段欄位。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront授權*</p> </td> 
   <td> <p>請求或更高版本</p> <p>審核項目和任務的或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>訪問級別配置*</strong> </td> 
   <td> <p>查看項目、任務和問題的或更高版本</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>物件權限</p> </td> 
   <td> <p>查看要導出其表單的項目、任務或問題的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，您必須具備下列所有條件：

1. 為要從中導出的特定對象建立自定義表單。
1. 將自訂表單附加至物件

   或

   擁有正確的存取權，可附加自訂表單並編輯表單上的資訊。

如需建立自訂表單的相關資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

有關將表單附加到對象的資訊，請參見 [將自訂表單新增至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 匯出詳細資訊區段中的資訊

從對象的「詳細資訊」部分導出資訊對於支援該資訊的所有對象都是相同的。

1. 轉到您至少具有「查看」權限的項目、任務、產品組合、方案或問題。
1. 按一下 **「詳細資訊」項** ，例如 **任務詳細資訊**.
1. （選用）如果物件沒有附加自訂表單，請開始在 **新增自訂表單欄位**，然後在清單中出現時按一下。

   最多可以新增10個表單。

1. （選用）更新詳細資訊區段中的資訊，然後按一下 **儲存變更**.
1. 按一下 **匯出** 下拉式功能表，選取 **概述**，或您要匯出的表單，然後按一下 **匯出**.

   您也可以選取 **全選** 如果要匯出「概述」區域和所有自訂表單。

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >可能存在下列情況：
   >
   >   
   >   
   >   * 當您的群組或Workfront管理員取消選取「概述」區域中的所有欄位，且物件已附加自訂表單時，「概述」區段不會顯示。
   >   * 當您的群組或Workfront管理員取消選取「概述」區域中的所有欄位，且物件未附加自訂表單時，「匯出」下拉式功能表將不會顯示。
   >   * 當物件未附加自訂表單時，您只能匯出「概述」區域。
   >   * 邏輯後面且表單上未顯示的自訂欄位不會匯出。 如需將邏輯新增至自訂表單的詳細資訊，請參閱 [新增顯示邏輯並略過邏輯至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).


   PDF檔案會產生並下載至您的電腦。 PDF檔案包含下列資訊：

   * 表單所附加的對象的名稱
   * 導出PDF的用戶名
   * 生產PDF的日期和時間
   * 導出的表單的名稱
   * 表單上已填欄位的資訊
