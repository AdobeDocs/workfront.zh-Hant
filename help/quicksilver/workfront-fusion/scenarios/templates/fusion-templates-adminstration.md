---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion範本管理
description: 如果您是管理員，則您有權檢視、修改、重新命名、發佈、核准和刪除其他人建立的範本。 您可以從 [!UICONTROL 範本] 頁面 [!DNL Adobe Workfront Fusion Administration] 的上界。
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 範本管理

如果您是管理員，則您有權檢視、修改、重新命名、發佈、核准和刪除其他人建立的範本。 您可以從 [!UICONTROL 範本] 頁面 [!DNL Adobe Workfront Fusion Administration] 的上界。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
    <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化） </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是貴組織的Workfront Fusion管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 檢視 [!DNL Workfront Fusion] 模板作為管理員

要查看所有已建立模板及其狀態的表，請執行以下操作：

1. 按一下 **[!UICONTROL 管理]** ，開啟 [!UICONTROL 管理] 的上界。
1. 按一下 **[!UICONTROL 範本]** ，即可取得Advertising Cloud的說明。

有三欄與範本發佈狀態相關。 欄中的勾選記號表示下列項目：

* **[!UICONTROL 已發佈]**:這些範本目前會顯示在 [!UICONTROL 團隊範本] 頁簽。
* **[!UICONTROL 請求批准]**:這些範本正在等待您的批准。 它們目前顯示在 [!UICONTROL 團隊範本] 頁簽。
* **[!UICONTROL 已核准]**:這些範本已獲得核准。 它們目前顯示在 [!UICONTROL 公用範本] 標籤。

>[!NOTE]
>
>在 [!UICONTROL 請求批准] 欄和 [!UICONTROL 已核准] 欄已獲得批准並公開，但有較新版本的欄正在等待您的批准。

## 編輯 [!DNL Workfront Fusion] 模板作為管理員

1. 按一下 **[!UICONTROL 管理]** ，開啟 [!UICONTROL 管理] 的上界。
1. 按一下 **[!UICONTROL 範本]** ，即可取得Advertising Cloud的說明。
1. 按一下 **[!UICONTROL 詳細資料]** ，即可編輯。

您現在可以編輯範本，類似於以非管理員使用者身分編輯範本。 不過，在 [!UICONTROL 選項] 右上角有另一個選項，即提供SVG程式碼的SVG圖表。 此外，發佈程式與標準使用者的情況相同，如需詳細資訊，請參閱發佈和共用範本區段。

如需可編輯之特定範本選項的相關資訊，請參閱 [在中建立新範本 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

如需發佈範本的詳細資訊，請參閱 [發佈與共用 [!DNL Adobe Workfront Fusion] 範本](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## 批准或不批准 [!DNL Workfront Fusion] 範本

核准範本會使其顯示在 [!UICONTROL 公用範本] 標籤，所有使用者皆可使用。 不批准範本會將其從 [!UICONTROL 公用範本] 標籤，並使其僅供建立它的團隊使用。

1. 按一下 **[!UICONTROL 管理]** ，開啟 [!UICONTROL 管理] 的上界。
1. 按一下 **[!UICONTROL 範本]** ，即可取得Advertising Cloud的說明。
1. 如果要核准範本，請按一下 **[!UICONTROL 核准]** 的URL。
1. 如果您想不批准範本，請按一下 **[!UICONTROL 不批准]** 的URL。

>[!NOTE]
>
>如果您核准先前核准並編輯的範本，您的第二次核准將覆寫原始範本。

## 將案例複製為範本

身為管理員，您可以將案例複製為範本。

如需將案例複製為範本的指示，請參閱 [在中建立新範本 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create)in [在中建立新範本 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
