---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: 建立與Experience Manager Assets或Assets Essentials連結的資料夾
description: 在Workfront中，您可以建立與Experience Manager Assets或Assets Essentials連結的資料夾。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# 建立與Experience Manager Assets或Assets Essentials連結的資料夾

在Workfront中，您可以建立與Experience Manager Assets或Assets Essentials連結的資料夾。 由於資料夾已連結，因此新增至資料夾的任何資產都會自動顯示於Workfront和Experience Manger中。 如果資產位於連結的資料夾中，您不必手動傳送資產。

如果從Experience Manager Assets或Assets Essentials內的連結資料夾中刪除或移動資產，Workfront會在專案>檔案區域中保留資產副本。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table>
  <tr>
   <td><strong>Adobe Workfront封裝</strong>
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront授權</strong>
   </td>
   <td>
   <p>標準</p>
   <p>規劃</p>
   </td>
  </tr>
  <tr>
   <td><strong>其他產品</strong>
   </td>
   <td>您必須擁有Experience Manager Assets as a Cloud Service或Assets Essentials，並且您必須以使用者身分新增到產品中。
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

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱[設定Experience Manager Assets as a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。


## 建立連結的資料夾

連結資料夾會在Workfront管理員設定整合時，於其指定的位置中建立。 每個整合只能有一個連結資料夾的資料夾位置。

連結資料夾的名稱會根據與其相關聯的Portfolio、方案、專案自動建立，且無法變更。 如果專案未與Portfolio或方案相關聯，連結的資料夾將顯示專案名稱和建立日期。

>[!NOTE]
>
>您無法在連結資料夾內建立新檔案或校訂版本。


若要建立連結資料夾：

1. 前往您想要資料夾的專案。
1. 選取「**新增**」，然後前往管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可以選擇任何名稱來進行這項整合，因此可能沒有特別提及Experience Manager Assets或Assets Essentials。

1. 選取&#x200B;**建立連結的資料夾**。 系統會根據設定整合時指定的位置，在Experience Manager中自動建立資料夾。
   ![建立連結資料夾](assets/linked-folder.png)
