---
title: 匯出自訂表單和物件詳細資料
description: 匯出自訂表單和物件詳細資料
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 1%

---

# 匯出自訂表單和物件詳細資料

您可以將物件的「詳細資訊」區段中的「概述」和自訂表單資訊匯出至PDF檔案。 然後，您可以列印或與其他使用者共用PDF。

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
>您的Workfront或群組管理員使用版面配置範本移除的「詳細資訊」區段中的欄位不會顯示。

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
   <td> <p>要求或更高版本的問題</p> <p>專案和任務的檢閱或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>存取層級設定*</strong> </td> 
   <td> <p>專案、任務和問題的檢視或以上版本</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>物件許可權</p> </td> 
   <td> <p>檢視或更高許可權至您要匯出其表單的專案、任務或問題</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 先決條件

開始之前，您必須具備下列所有條件：

1. 為您要從中匯出它的特定物件建立自訂表單。
1. 將自訂表單附加至物件

   或

   具有附加自訂表單和編輯表單上資訊的正確存取權。

如需建立自訂表單的相關資訊，請參閱[使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

如需將表單附加至物件的相關資訊，請參閱[將自訂表單新增至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

## 匯出「詳細資訊」段落中的資訊

從物件的「詳細資訊」區段匯出資訊時，所有支援該資訊的物件都是相同的。

1. 前往您至少擁有「檢視」許可權的專案、任務、專案組合、方案或問題。
1. 按一下左側面板上的&#x200B;**「詳細資料」專案**，例如&#x200B;**任務詳細資料**。
1. （選擇性）如果沒有自訂表單附加到物件，請在&#x200B;**新增自訂表單欄位**&#x200B;中開始輸入自訂表單的名稱，然後當它出現在清單中時按一下它。

   您最多可以新增10個表單。

1. （選擇性）更新[詳細資料]區段中的資訊，然後按一下[儲存變更]。****
1. 按一下右上角的&#x200B;**匯出**&#x200B;下拉式功能表，選取&#x200B;**概述**&#x200B;或您要匯出的表單，然後按一下&#x200B;**匯出**。

   如果您要匯出[概述]區域與所有自訂表格，您也可以選取&#x200B;**全選**。

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >可能存在下列情況：
   >
   >   
   >   
   >   * 當您的群組或Workfront管理員取消選取總覽區域中的所有欄位，並且物件有附加的自訂表單時，總覽區段不顯示。
   >   * 當您的群組或Workfront管理員取消選取總覽區域中的所有欄位，並且物件沒有附加自訂表單時，匯出下拉選單不可見。
   >   * 當物件沒有附加自訂表單時，您只能匯出概述區域。
   >   * 邏輯落後且在表單上不可見的自訂欄位不會匯出。 如需將邏輯新增至自訂表單的相關資訊，請參閱[新增顯示邏輯並略過邏輯至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)。
   >   
   >

   會產生PDF檔案並下載至您的電腦。 PDF檔案包含下列資訊：

   * 表單附加到的物件名稱
   * 匯出PDF的使用者名稱
   * 產生PDF的日期和時間
   * 您匯出的表單名稱
   * 表單上填寫欄位中的資訊
