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
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# 防止詐騙並新增[!DNL Adobe Workfront]個SPF記錄

## 問題

如果使用者沒有收到[!DNL Adobe Workfront]電子郵件通知，您必須將[!DNL Workfront]個SPF記錄新增至防火牆。 您必須與IT團隊合作，才能新增SPF記錄。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
