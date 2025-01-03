---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 用於存取Adobe Workfront Fusion的IP位址
description: 除了Adobe Workfront授權，Adobe Workfront Fusion還需要Adobe Workfront Fusion授權。
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 800cf889ff2729fca0c9d75d0ace0ecc1ee53a79
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 用於存取[!DNL Adobe Workfront Fusion]的IP位址

>[!NOTE]
>
>除了[!DNL Adobe Workfront license]之外，[!DNL Adobe Workfront Fusion]還需要[!DNL Adobe Workfront Fusion]授權。

如果您的防火牆或郵件伺服器設定為僅允許存取特定廠商，則必須將特定IP位址新增至其允許清單，以允許您的環境與[!DNL Adobe Workfront Fusion]之間的開放通訊。

您可以將所有Fusion IP位址和網域新增至允許清單，也可以找到Fusion叢集並僅新增該叢集的IP位址和網域。

## 新增所有Fusion IP位址和網域

將下列IP位址新增至允許清單：

* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

此外，如果您的組織使用傳出網路篩選，請將以下網域新增到您的允許清單，讓您的系統能夠存取Workfront Fusion。 這些會用於Webhook。

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## 僅為您的叢集新增Fusion IP位址和網域

### 識別您的資料中心

IP位址會依您儲存資料的位置而有所不同。

如果您透過URL存取Fusion，則可檢查URL以找出您的資料中心。

| URL | 資料中心 |
| --- | --- |
| `https://app.workfrontfusion.com/` | 美國資料中心 |
| `https://app-eu.workfrontfusion.com/` | 歐盟資料中心 |
| `https://app-az.workfrontfusion.com/` | Azure資料中心 |

如果您透過experience.adobe.com存取Fusion，可以檢查瀏覽器中的網路索引標籤，以識別資料中心。

| URL | 資料中心 |
| --- | --- |
| 呼叫`https://fusion.adobe.com` | 美國資料中心 |
| 呼叫`https://eu.fusion.adobe.com` | 歐盟資料中心 |
| 呼叫`https://az.fusion.adobe.com` | Azure資料中心 |

### 為您的資料中心新增IP位址和網域

將下列IP位址新增至您的允許清單，讓[!DNL Workfront Fusion]能夠存取您的系統。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 歐盟資料中心</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 美國資料中心</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li>
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 在Microsoft Azure叢集上</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

此外，如果您的組織使用傳出網路篩選，請將以下網域新增到您的允許清單，讓您的系統能夠存取Workfront Fusion。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 歐盟資料中心</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 美國資料中心</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] 在Microsoft Azure叢集上</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>傳出網路篩選並不常見。 請洽詢您的網路管理員，以瞭解是否需要更新允許清單以符合您的要求。

如需設定組織允許清單的詳細資訊，請參閱[設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。
