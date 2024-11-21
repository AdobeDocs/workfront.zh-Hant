---
title: 加密程式
description: Adobe Workfront Fusion Encryptor模組可讓您加密任何文字資料。 目前支援透過AES256和PGP (OpenPGP)進行訊息加密。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 加密程式

[!DNL Adobe Workfront Fusion] [!UICONTROL 加密程式]模組可讓您加密任何文字資料。 它們目前支援透過AES256和PGP ([!UICONTROL OpenPGP])進行訊息加密。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，貴組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 使用PGP的訊息加密與解密

透過PGP加密和解密時，必須使用金鑰鏈並建立私密或公開金鑰（或兩者）。

如需公開和私密金鑰的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md)中的[基本術語。 如需金鑰鏈的相關詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md)中的[金鑰。

## [!UICONTROL 加密程式]模組及其欄位

當您設定[!UICONTROL 加密程式]模組時，會顯示下列欄位。 模組中的粗體標題表示必填欄位。

### 加密PGP訊息

此模組可讓您使用公開和私密金鑰來加密訊息。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL私密金鑰]</td>
        <td>輸入寄件者的私密金鑰。 這可以驗證寄件者的身分。</td>
    </tr>
    <tr>
        <td>[！UICONTROL公開金鑰]</td>
        <td>輸入收件者的公開金鑰。</td>
    </tr>
    <tr>
        <td>[！UICONTROL訊息]</td>
        <td>輸入您要加密的訊息。</td>
    </tr>

### 解密PGP訊息

此模組可讓您使用公開和私密金鑰解密訊息。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL私密金鑰]</td>
        <td>輸入收件者的私密金鑰。</td>
    </tr>
    <tr>
        <td>[！UICONTROL公開金鑰]</td>
        <td>輸入收件者的公開金鑰。 這可以驗證寄件者的身分。</td>
    </tr>
    <tr>
        <td>[！UICONTROL訊息]</td>
        <td>對應您要解密的訊息。</td>
    </tr>
</table>
