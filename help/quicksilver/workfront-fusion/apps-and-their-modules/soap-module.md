---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: soap模組
description: 您可以使用SOAP模組來連線到Adobe Workfront Fusion中的SOAP API。
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 1%

---

# [!UICONTROL SOAP] 模組

您可以使用 [!UICONTROL SOAP] 要連線的模組 [!UICONTROL SOAP] 中的API [!UICONTROL Adobe Workfront Fusion].

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 使用 [!UICONTROL SOAP] 模組

此 [!UICONTROL SOAP] 模組目前為測試版，不支援：

* 重新定義元素
* 分數數字限制
* 總位數限制
* 空白字元限制
* 輸入和輸出訊息中有多個部分。 僅支援單一零件訊息
* 自訂XML結構描述元素是在的說明下定義的 [[!UICONTROL SOAP] 編碼](http://schemas.xmlsoap.org) 結構描述和元素。

>[!INFO]
>
>**範例:**
>  
>下列專案無法正確辨識 [!UICONTROL Workfront Fusion]：
>
>```
><complexType name="ArrayOfFloat">
>
>   
>  <complexContent>
>
>      
>     <restriction base="soapenc:Array">
>
>         
>        <attribute ref="soapenc:arrayType"
>
>            
>           wsdl:arrayType="xsd:integer[]"/>
>
>      
>     </restriction>
>
>   
>  </complexContent>
>
>
></complexType>
>```

其中包括 `soapenc:Array`， `soapenc:arrayType` 和 `wsdl:arrayType` 尚未支援的參考資料 [!UICONTROL Workfront Fusion].

## 因應措施

如果 [!UICONTROL SOAP] 模組拒絕處理WSDL檔案，或在模組設定中擲回各種錯誤，您可以嘗試使用universal **[!UICONTROL HTTP] > [!UICONTROL 提出要求]** 而改用模組：

1. 在 [!DNL Workfront Fusion]，建立新情境。
1. 插入 **[!UICONTROL HTTP] > [!UICONTROL 提出要求]** 模組。
1. 開啟模組的設定，並填寫下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL方法]</td> 
      <td> <p>[！UICONTROLPOST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL主體型別]</td> 
      <td> <p>[！UICONTROL Raw]</p> </td> [！UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL內容型別]</td> 
      <td> <p>[！UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL剖析回應]</td> 
      <td>[！UICONTROL已啟用]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. 開啟新的Web瀏覽器視窗或標籤。
1. 將WSDL URL貼入網頁瀏覽器的位址列，並擷取XML檔案。

   WSDL URL的結尾通常是 `?wsdl`，但不一定，例如 `http://voip.ms/api/v1/server.wsdl`.

1. 如果WSDL檔案沒有直接顯示在網頁瀏覽器中，請在文字編輯器中開啟下載的檔案。
1. 搜尋 `<service>` 或 `<wsdl:service>` 標籤：

   ![](assets/service-350x65.png)

1. 找到後，從以下位置複製URL： `location` 屬性。
1. 在 [!DNL Workfront Fusion]，將URL貼入HTTP模組的URL欄位中。
1. 開啟 [線上 [!UICONTROL SOAP] 使用者端](https://wsdlbrowser.com/) 在新的網頁瀏覽器視窗/標籤中。
1. 將WSDL URL貼入WSDL URL欄位。
1. 按一下 **[!UICONTROL 瀏覽]**.
1. 從左側的函式清單中選取，例如 `getLanguages`.
1. 複製的內容 [!UICONTROL 請求XML] 文字區域。
1. 在 [!UICONTROL Workfront Fusion]，將複製的內容貼至模組的URL欄位。
1. 將問號取代為實際值，以提供所選引數的值：

   ![](assets/request-xml-350x172.png)

1. 按一下以關閉模組的設定 **[!UICONTROL 確定]**.
1. 執行案例或模組。
