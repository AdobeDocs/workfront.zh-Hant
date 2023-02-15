---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: SOAP模組
description: 您可以使用SOAP模組連線至Adobe Workfront Fusion中的SOAP API。
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# [!UICONTROL SOAP] 模組

您可以使用 [!UICONTROL SOAP] 連接到 [!UICONTROL SOAP] 中的API [!UICONTROL Adobe Workfront融合].

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

## 使用 [!UICONTROL SOAP] 模組

此 [!UICONTROL SOAP] 模組目前處於測試狀態，不支援：

* 重定義元素
* 小數位數限制
* 總位數限制
* 空格限制
* 輸入和輸出消息中的多個部分。 僅支援單部件消息
* 通過 [[!UICONTROL SOAP] 編碼](http://schemas.xmlsoap.org) 結構和元素。

>[!INFO]
>
>**範例:**
>  
>無法正確識別下列項目 [!UICONTROL Workfront融合]:
>
>```
><complexType name="ArrayOfFloat">
>
>   <complexContent>
>
>      <restriction base="soapenc:Array">
>
>         <attribute ref="soapenc:arrayType"
>
>            wsdl:arrayType="xsd:integer[]"/>
>
>      </restriction>
>
>   </complexContent>
>
></complexType>
>```

其中包括 `soapenc:Array`, `soapenc:arrayType` 和 `wsdl:arrayType` 參考，但 [!UICONTROL Workfront融合].

## 因應措施

若 [!UICONTROL SOAP] 模組拒絕處理WSDL檔案或在模組配置中擲回各種錯誤，您可以嘗試使用通用 **[!UICONTROL HTTP] > [!UICONTROL 提出請求]** 模組改為：

1. 在 [!DNL Workfront Fusion]，建立新藍本。
1. 插入 **[!UICONTROL HTTP] > [!UICONTROL 提出請求]** 模組。
1. 開啟模組的設定，並填入下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL方法]</td> 
      <td> <p>[!UICONTROLPOST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL主體類型]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL內容類型]</td> 
      <td> <p>[!UICONTROL XML(application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parse響應]</td> 
      <td>[!UICONTROL已啟用]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. 開啟新的Web瀏覽器窗口或頁簽。
1. 將WSDL URL貼到Web瀏覽器的地址欄中，然後提取XML檔案。

   WSDL URL的結尾通常為 `?wsdl`，但不一定 `http://voip.ms/api/v1/server.wsdl`.

1. 如果WSDL檔案未直接顯示在Web瀏覽器中，請在文本編輯器中開啟下載的檔案。
1. 搜尋 `<service>` 或 `<wsdl:service>` 標籤：

   ![](assets/service-350x65.png)

1. 找到URL後，從 `location` 屬性。
1. 在 [!DNL Workfront Fusion]，將URL貼入HTTP模組的URL欄位中。
1. 開啟 [線上 [!UICONTROL SOAP] 用戶端](https://wsdlbrowser.com/) 頁簽中。
1. 將WSDL URL貼到「WSDL URL」欄位中。
1. 按一下 **[!UICONTROL 瀏覽]**.
1. 從左邊的函式清單中挑選，例如 `getLanguages`.
1. 複製 [!UICONTROL 請求XML] 文本。
1. 在 [!UICONTROL Workfront融合]，將複製的內容貼到模組的URL欄位。
1. 將問號取代為實際值，以提供選取參數的值：

   ![](assets/request-xml-350x172.png)

1. 按一下「 」以關閉模組的設定 **[!UICONTROL 確定]**.
1. 執行情境或模組。
