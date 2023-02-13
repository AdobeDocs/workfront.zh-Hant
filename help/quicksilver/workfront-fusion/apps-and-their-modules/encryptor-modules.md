---
title: 加密器
description: Adobe Workfront Fusion Encryptor模組允許您加密任何文本資料。 他們目前支援透過AES256和PGP(OpenPGP)進行訊息加密。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 加密器

[!DNL Adobe Workfront Fusion] [!UICONTROL 加密器] 模組可讓您加密任何文字資料。 他們目前支援透過AES256和PGP([!UICONTROL OpenPGP])。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>   <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 使用PGP的消息加密和解密

透過PGP加密和解密時，必須使用密鑰鏈並建立私密或公開密鑰（或兩者）。

如需公開金鑰和私密金鑰的詳細資訊，請參閱 [基本術語， [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). 如需鍵鏈的詳細資訊，請參閱 [中的金鑰 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL 加密器] 模組及其欄位

設定時 [!UICONTROL 加密器] 模組，則會顯示下列欄位。 模組中的粗體標題表示必填欄位。

### 加密PGP訊息

此模組可讓您使用公開和私密金鑰加密訊息。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL私鑰]</td>
        <td>輸入寄件者的私密金鑰。 這可以驗證寄件者的身分。</td>
    </tr>
    <tr>
        <td>[!UICONTROL公鑰]</td>
        <td>輸入收件者的公開金鑰。</td>
    </tr>
    <tr>
        <td>[!UICONTROL消息]</td>
        <td>輸入要加密的消息。</td>
    </tr>

### 解密PGP消息

此模組可讓您使用公開和私密金鑰解密訊息。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL私鑰]</td>
        <td>輸入收件者的私密金鑰。</td>
    </tr>
    <tr>
        <td>[!UICONTROL公鑰]</td>
        <td>輸入收件者的公開金鑰。 這可以驗證寄件者的身分。</td>
    </tr>
    <tr>
        <td>[!UICONTROL消息]</td>
        <td>映射要解密的消息。</td>
    </tr>
</table>
