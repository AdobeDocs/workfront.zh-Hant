---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 配置防火牆的允許清單
description: 如果防火牆或郵件伺服器配置為僅允許訪問某些供應商，則必須將某些IP地址添加到允許清單中。 這會開啟您的環境與Adobe Workfront伺服器之間的通訊，並允許您的使用者從Workfront傳送訊息，以及搭配Active Directory或LDAP使用SSO。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 13%

---

# 配置防火牆的允許清單

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>若要在貴組織已上線至Adobe Admin Console時設定允許清單，請參閱 [允許Adobe應用程式和服務的網域](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

如果防火牆或郵件伺服器配置為僅允許訪問某些供應商，則必須將某些IP地址添加到允許清單中。 這會開啟您的環境與Adobe Workfront伺服器之間的通訊，並允許下列程式：

* 從Workfront應用程式傳送訊息

   >[!NOTE]
   >
   >如果貴組織的Workfront執行個體已透過Adobe IMS啟用，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

* 在設定自訂檔案整合時使用檔案WebHook
* 使用Workfront事件訂閱

   如需詳細資訊，請參閱 [事件訂閱API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

您還需要開啟某些埠，以便在傳送電子郵件時對其進行加密。

## Workfront允許清單

如果貴組織有企業計畫，您也可以設定兩個Workfront允許清單：

* **電子郵件允許清單**:可讓您控制使用者可將資料儲存在Workfront中的電子郵件位置。 如需詳細資訊，請參閱 [設定您的電子郵件允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **IP允許清單**:將對Workfront的存取限制為您指定的45個IP位址或IP位址範圍，為Workfront應用程式提供額外的安全層。 如需詳細資訊，請參閱 [依IP位址限制Adobe Workfront的存取權](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## 要新增至允許清單的IP位址

防火牆上您必須新增至允許清單的IP位址，視您的生產環境執行所在的叢集而定。 通過查看「設定」>「系統」>「自定義資訊」，可以查找此群集。 如需詳細資訊，請參閱 [配置基本資訊](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md#configuring-basic-info) 在文章中 [配置系統的基本資訊](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

>[!IMPORTANT]
>
>某些Workfront整合在啟用允許清單時無法運作，因為無法以靜態IP位址進行設定。 若要使用下列整合，您必須停用允許清單。
>
>* Workfront for G Suite
>* Workfront for Outlook
>* Workfront for Salesforce


* [允許群集1、2、3、5、7、8和9的IP地址](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [允許群集4的IP地址](#ip-addresses-to-allow-for-cluster-4)
* [允許群集6的IP地址](#ip-addresses-to-allow-for-cluster-6)
* [允許測試驅動器的IP地址](#IP%20Addre2)
* [實作事件訂閱時允許的IP位址](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [允許增強驗證的IP位址](#ip-addresses-to-allow-for-enhanced-authentication)
* [要新增的IP位址以存取Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [要新增的IP位址，以使用Workfront for Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [要新增的IP位址，以使用Workfront Ascent](#ip-addresses-to-add-for-using-workfront-ascent)
* [要為所有叢集新增的URL Workfront](#urls-to-add-for-all-clusters-workfront)

### 允許群集1、2、3、5、7、8和9的IP地址 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

如果您的生產環境位於叢集1、2、3、5或7，則必須允許下列IP位址。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">對於SSO、文檔Webhook或其他功能</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">從Workfront應用程式接收電子郵件的方式</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>如需下列IP位址的相關資訊，請參閱 <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md" class="MCXref xref">Adobe Workfront 21.1版新增電子郵件IP位址</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 允許群集4的IP地址 {#ip-addresses-to-allow-for-cluster-4}

如果您的生產環境位於叢集4，請新增下列IP位址以進行SSO、記錄網頁連結整合，以及從Workfront應用程式接收電子郵件：

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230.232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122

如需下列IP位址的相關資訊，請參閱 [Adobe Workfront 21.1版新增電子郵件IP位址](../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md)

* 23.251.239.98
* 23.251.239.99

### 允許群集6的IP地址 {#ip-addresses-to-allow-for-cluster-6}

如果您的生產環境位於叢集6，請新增下列IP位址。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">從Workfront應用程式接收電子郵件的方式</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">使用AWS電子郵件服務的方式</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 允許測試驅動器的IP地址

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">使用測試驅動器時從Workfront應用程式接收電子郵件的方式</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">用於使用測試驅動器時的SSO和檔案網頁連結整合</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>此位址也必須新增至您的允許清單，您的使用者才能收到Workfront的電子郵件。</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 實作事件訂閱時允許的IP位址  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

針對所有環境，新增下列IP位址以從Workfront事件訂閱接收裝載。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 歐洲客戶</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">適用於歐洲以外地區的客戶</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 允許增強驗證的IP位址 {#ip-addresses-to-allow-for-enhanced-authentication}

新增下列IP位址，以使用增強的驗證來預覽或生產。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">如果您的環境位於群集1、2、3、5、7、8或9上</td> 
   <td> 
    <ul> 
     <li>35.167.74.121</li> 
     <li>35.166.202.113</li> 
     <li>35.160.3.103</li> 
     <li>54.183.64.135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54.183.204.205</li> 
     <li>35.171.156.124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">如果您的環境位於群集4上</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193.66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52.211.56.181</li> 
     <li>52.213.38.246</li> 
     <li>52.213.74.69</li> 
     <li>52.213.216.142</li> 
     <li>35.156.51.163</li> 
     <li>35.157.221.52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52.208.95.174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 要新增的IP位址以存取Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

將下列IP位址新增至您的允許清單，讓Workfront Fusion可存取您的系統。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe WorkfrontEU資料中心</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront美國資料中心</p> </td> 
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
   <td role="rowheader">Adobe WorkfrontEU資料中心</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront美國資料中心</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>傳出網路篩選並不常見。 請洽詢您的網路管理員，查看您是否需要更新允許清單以容納。

### 要新增的IP位址，以使用Workfront for Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

將下列IP位址新增至您的允許清單，以使用Workfront進行Jira整合。

jira.workfront.com域也必須可從公司伺服器訪問。 此網域為必要網域，因為它是Workfront和Jira之間的中間件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 歐洲客戶</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">適用於歐洲以外地區的客戶</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 要新增的IP位址，以使用Workfront Ascent {#ip-addresses-to-add-for-using-workfront-ascent}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">透過Workfront Ascent存取Workfront訓練資源</td> 
   <td> 
    <ul> 
     <li>18.223.140.34</li> 
     <li>3.13.223.30</li> 
     <li>3.13.19.112</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">從Workfront Ascent接收電子郵件通知</td> 
   <td> 
    <ul> 
     <li>23.251.227.75</li> 
     <li>23.251.227.76</li> 
     <li>23.251.227.77</li> 
     <li>23.251.227.78</li> 
     <li>23.251.227.79</li> 
     <li>23.251.227.80</li> 
     <li>23.251.227.81</li> 
     <li>23.251.227.82</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 要新增的網域以存取Workfront

如果您的組織使用傳出網路篩選，請將下列網域新增至您的允許清單，讓您的系統可存取Workfront。

>[!NOTE]
>
>傳出網路篩選並不常見。 請洽詢您的網路管理員，查看您是否需要更新允許清單以容納。

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/

## 要為所有叢集新增的URL Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">允許在您的Workfront環境中顯示說明內容</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">若要允許Workfront Proof在任何叢集上存取Workfront，請將這些項目新增至所有環境</td> 
   <td> 
    <ul> 
     <li>*.workfront.com — 需要在Workfront中檢視校樣</li> 
     <li>*.proofhq.com — 需要在Workfront校樣中檢視校樣</li> 
     <li>*.proofhq.eu — 在Workfront校樣中檢視校樣的必要項目</li> 
    </ul> <p><b>附註</b>:  <p>我們不支援將IP位址新增至您的Workfront校樣允許清單。 在Workfront移至AWS後，變數變得動態。 反之，我們建議您僅允許Workfront校樣網域。</p> <p>如果將這些網域新增至您的允許清單時發生問題，而您需要的是IP位址，請聯絡Workfront客戶支援。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 要新增的IP位址和URL以存取Workfront Proof

您必須將下列IP位址新增至允許清單，才能使用各種函式。

* [用於回呼和網頁擷取校樣](#for-callbacks-and-webcapture-proofs)
* [對於傳出電子郵件](#for-outgoing-email)

### 用於回呼和網頁擷取校樣 {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">產品 — 美國（叢集1、2、3、5和7）</td> 
   <td> 
    <ul> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU（群集4）</td> 
   <td> 
    <ul> 
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>注意</b>:不再支援DNS伺服器選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 對於傳出電子郵件 {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>產品 — 美國（叢集1、2、3、5和7）</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU（群集4）</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 要開啟的埠，以獲得最佳Workfront校樣效能

如果您遇到校樣載入問題或無法在Workfront Proof中運作的問題，請開啟下列連接埠：

* 5671
* 5672
* 15671

## 要開啟的埠，用於加密電子郵件

來自Workfront應用程式的電子郵件會使用連接埠465和587進行加密。 如果您的郵件伺服器不支援加密的電子郵件，則會使用連接埠25來傳送未加密的電子郵件。

## 來自Workfront支援的電子郵件通知

如果您沒有收到Workfront支援的電子郵件，請確定您新增所需的Salesforce IP位址和網域。 如需詳細資訊，請參閱Salesforce說明文章，了解要允許的Salesforce IP位址和網域。
