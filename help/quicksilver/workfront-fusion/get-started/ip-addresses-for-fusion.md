---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 存取Adobe Workfront Fusion的IP位址
description: Adobe Workfront Fusion除了需要Adobe Workfront授權外，還需要Adobe Workfront Fusion授權。
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# 用於存取的IP位址 [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 要求 [!DNL Adobe Workfront Fusion] 除 [!DNL Adobe Workfront license].

如果您的防火牆或郵件伺服器配置為只允許訪問某些供應商，則必須將某些IP地址添加到允許清單中，以便允許您的環境和 [!DNL Adobe Workfront Fusion].

將下列IP位址新增至您的允許清單以啟用 [!DNL Workfront Fusion] 來存取您的系統。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU資料中心</td> 
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
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

此外，如果貴組織使用傳出網路篩選，請將下列網域新增至允許清單，讓您的系統可存取Workfront Fusion。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU資料中心</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 美國資料中心</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>傳出網路篩選並不常見。 請洽詢您的網路管理員，查看您是否需要更新允許清單以容納。

如需設定組織允許清單的詳細資訊，請參閱 [配置防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
