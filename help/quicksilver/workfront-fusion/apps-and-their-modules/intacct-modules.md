---
title: Intacct模組
description: Intacct模組
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Intacct模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Intacct的工作流程，並將其連接至多個第三方應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr>
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

要使用Intacct模組，您必須有Intacct帳戶。

## 將Intacct連接到Workfront Fusion

### 授權 [!DNL Workfront Fusion] 在Intacct中進行更改

之前 [!DNL Workfront Fusion] 可連線至 [!DNL Intacct]，您必須授權。

在您的Intacct帳戶中，導覽至 **[!UICONTROL 公司]** 標籤。

1. 按一下 **公司資訊**.
1. 導覽至 **安全性** 標籤。
1. 按一下 [!UICONTROL 編輯] 在右上角
1. 選擇Web服務授權。
1. 按一下加號圖示
1. 輸入AzuquaMPP作為sender_id。
1. （可選）輸入連接的說明

### 在 [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

您可以建立與 [!DNL Intacct] 直接從內部 [!DNL Intacct] 模組。

1. 在任何Intacct模組中，按一下 **[!UICONTROL 新增]** 欄位旁邊。
1. 輸入您的Intacct憑據

   * 公司 ID
   * 使用者 ID
   * 密碼

1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## Intacct模組及其欄位

設定時 [!DNL Intacct] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些欄位，還可能會顯示其他Intacct欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)
* [[!UICONTROL 搜尋記錄]](#search-records)

### [!UICONTROL 進行自訂API呼叫] {#make-a-custom-api-call}

此動作模組可讓您對 [!DNL Intacct] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Intacct] 模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>連接</p> </td> 
   <td> <p>有關將Intacct帳戶連接到 [!DNL Workfront Fusion] 2.0，參見 <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">在Workfront Fusion中設定連線</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">內文XML</td> 
   <td> <p>只在內文中加入XML。 請求會自動包含驗證標題。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜尋記錄]

此搜索模組檢索符合特定搜索條件的記錄清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>連接</p> </td> 
   <td> <p>有關將Intacct帳戶連接到 [!DNL Workfront Fusion] 2.0，參見 <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">在Workfront Fusion中設定連線</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要搜索的記錄類型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>搜尋條件</p> </td> 
   <td> 
    <ul> 
     <li> <p>選擇要搜索的欄位</p> </li> 
     <li> <p>選擇要用於搜索的運算子</p> </li> 
     <li> <p>輸入要搜索的值</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">結果集</td> 
   <td>選擇是要返回所有匹配記錄，還是僅返回第一個匹配記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">限制</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">排序條件</td> 
   <td>選擇要按結果排序的欄位。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">順序</td> 
   <td>選取您要遞增排序或遞減排序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">輸出</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">區分大小寫</td> 
   <td>啟用此選項可讓您的查詢區分大小寫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">查詢私有實體</td> 
   <td>啟用此選項可允許模組搜索專用實體。</td> 
  </tr> 
 </tbody> 
</table>
