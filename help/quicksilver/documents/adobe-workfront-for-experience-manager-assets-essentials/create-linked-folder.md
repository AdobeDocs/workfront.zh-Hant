---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: 建立與Experience Manager Assets或Assets Essentials連結的資料夾
description: 在Workfront中，您可以建立與Experience Manager Assets或Assets Essentials連結的資料夾。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 84760d5fe301bd0a44879490fb030bd29821bd41
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# 建立與Experience Manager Assets或Assets Essentials連結的資料夾

在Workfront中，您可以建立與Experience Manager Assets或Assets Essentials連結的資料夾。 由於資料夾已連結，因此新增至資料夾的任何資產都會自動顯示於Workfront和Experience Manger中。 如果資產位於連結的資料夾中，您不必手動傳送資產。

如果從Experience Manager Assets或Assets Essentials內的連結資料夾中刪除或移動資產，Workfront會在「專案>檔案」區域中保留資產副本。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table>
  <tr>
   <td><strong>Adobe Workfront計畫*</strong>
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront授權*</strong>
   </td>
   <td>規劃
   </td>
  </tr>
  <tr>
   <td><strong>產品</strong>
   </td>
   <td>您必須擁有Experience Manager Assetsas a Cloud Service或Assets Essentials，而且您必須以使用者的身分新增到產品中。
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager許可權</strong>
   </td>
   <td>您必須擁有Experience Manger整合中目的地資料夾的寫入許可權。
   </td>
  </tr>
  <tr>
   <td><strong>存取層級設定</strong>
   </td>
   <td>您必須是Workfront管理員才能設定Experience Manager整合。 完成設定後，擁有計畫授權的使用者可以在個別專案上設定連結資料夾。
   </td>
  </tr>
</table>


*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

+++

## 先決條件

開始之前，

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱[設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。


## 建立連結的資料夾

連結資料夾會在Workfront管理員設定整合時，於其指定的位置中建立。 每個整合只能有一個連結資料夾的資料夾位置。

連結資料夾的名稱會根據與其相關聯的Portfolio、方案、專案自動建立，且無法變更。 如果專案未與Portfolio或方案相關聯，則連結的資料夾將顯示專案名稱和建立日期。

若要建立連結資料夾：

1. 前往您想要資料夾的專案。
1. 選取「**新增**」，然後前往管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能沒有特別提及Experience Manager Assets或Assets Essentials。

1. 選取&#x200B;**建立連結的資料夾**。 系統會根據設定整合時指定的位置，自動建立Experience Manager的資料夾。
   ![建立連結資料夾](assets/linked-folder.png)
