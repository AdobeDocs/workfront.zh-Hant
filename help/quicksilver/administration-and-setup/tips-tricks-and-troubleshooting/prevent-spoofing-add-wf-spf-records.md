---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 防止詐騙並新增 [!DNL Adobe Workfront] SPF記錄
description: 如果使用者沒有收到 [!DNL Adobe Workfront] 電子郵件通知，您必須將 [!DNL Workfront] SPF記錄新增至防火牆。 您必須與IT團隊合作，才能新增SPF記錄。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
TQID: https://experienceleague.adobe.com/6VnF205aiahPEWdP2kPk-YXF8UfPwSJ0-yJ6nGq3-FM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 292
ht-degree: 5%

---

# 防止詐騙並新增[!DNL Adobe Workfront]個SPF記錄

## 問題

如果使用者沒有收到[!DNL Adobe Workfront]電子郵件通知，您必須將[!DNL Workfront]個SPF記錄新增至防火牆。 您必須與IT團隊合作，才能新增SPF記錄。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解決方案

如果您已經將IP位址新增至生產環境的允許清單（如[設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)中所述），而且使用者仍然沒有收到電子郵件：

1. 將下列SPF記錄新增至防火牆：

   *spf.workfront.com*

   這會自動將所有[!DNL Workfront]個IP位址新增至防火牆上的允許清單，並允許所有垃圾郵件篩選器（使用SPF記錄）驗證[!DNL Workfront]伺服器是否為您網域的有效寄件者。

   >[!NOTE]
   >
   > SPF記錄是DNS區域檔案中的TXT記錄。 我們不支援修改您的DNS區域檔案。

1. 您必須指定需要設定的SPF記錄型別。 以下是有效的SPF記錄型別：

   * 全部(https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * 存在(https://dmarcian.com/spf-syntax-table/#exists)
   * 包含(https://dmarcian.com/spf-syntax-table/#include)

   例如，「v=spf1 a mx include： spf.workfront.com -all」

如果因為公司原則而無法將SPF記錄新增至防火牆，請與您的[!DNL Workfront]支援代表合作。
