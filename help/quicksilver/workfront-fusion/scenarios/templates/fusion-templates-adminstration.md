---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion範本管理
description: 如果您是管理員，則擁有檢視、修改、重新命名、發佈、核准和刪除其他人建立的範本的許可權。 您可以從「 」執行下列動作 [!UICONTROL 範本] 中的頁面 [!DNL Adobe Workfront Fusion Administration] 區域。
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 範本管理

如果您是管理員，則擁有檢視、修改、重新命名、發佈、核准和刪除其他人建立的範本的許可權。 您可以從「 」執行下列動作 [!UICONTROL 範本] 中的頁面 [!DNL Adobe Workfront Fusion Administration] 區域。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
    <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 若為工作自動化與整合]，[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是組織的Workfront Fusion管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 檢視 [!DNL Workfront Fusion] 作為管理員的範本

若要檢視所有已建立範本及其狀態的表格：

1. 按一下 **[!UICONTROL 管理]** 在左側導覽面板中開啟 [!UICONTROL 管理] 區域。
1. 按一下 **[!UICONTROL 範本]** ，位於左側導覽面板中。

有三個與範本發佈狀態相關的欄。 欄中的核取記號表示以下內容：

* **[!UICONTROL 已發佈]**：這些範本目前顯示在 [!UICONTROL 團隊範本] 標籤中選取「 」。
* **[!UICONTROL 已要求核准]**：這些範本正等待您的核准。 它們目前顯示在 [!UICONTROL 團隊範本] 標籤中選取「 」。
* **[!UICONTROL 已核准]**：這些範本已核准。 它們目前顯示在 [!UICONTROL 公用範本] 標籤中選取「 」。

>[!NOTE]
>
>同時含有核取記號的範本 [!UICONTROL 已要求核准] 欄和 [!UICONTROL 已核准] 欄已核准並公開，但有較新版本的欄等待您的核准。

## 編輯 [!DNL Workfront Fusion] 作為管理員的範本

1. 按一下 **[!UICONTROL 管理]** 在左側導覽面板中開啟 [!UICONTROL 管理] 區域。
1. 按一下 **[!UICONTROL 範本]** ，位於左側導覽面板中。
1. 按一下 **[!UICONTROL 詳細資訊]** 位於要編輯的範本右側。

您現在可以編輯範本，類似於以非管理員使用者的身分編輯範本。 不過，在 [!UICONTROL 選項] 右上角有一個額外選項，即為您提供SVG程式碼的SVG圖表。 此外，發佈程式與標準使用者的情況相同，如需詳細資訊，請參閱發佈和共用範本區段。

如需可編輯之特定範本選項的相關資訊，請參閱 [在中建立新範本 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

如需有關發佈範本的資訊，請參閱 [發佈和共用 [!DNL Adobe Workfront Fusion] 範本](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## 核准或不核准 [!DNL Workfront Fusion] 範本

核准範本後，它會顯示在 [!UICONTROL 公用範本] 標籤內的所有使用者都可使用。 不核准範本會將其從 [!UICONTROL 公用範本] 標籤並設為僅供建立該標籤的團隊使用。

1. 按一下 **[!UICONTROL 管理]** 在左側導覽面板中開啟 [!UICONTROL 管理] 區域。
1. 按一下 **[!UICONTROL 範本]** ，位於左側導覽面板中。
1. 若要核准範本，請按一下 **[!UICONTROL 核准]** 範本右側。
1. 如果您想要取消核准範本，請按一下 **[!UICONTROL 不核准]** 範本右側。

>[!NOTE]
>
>如果您正在核准先前已核准然後編輯的範本，則您的第二次核准將會覆寫原始範本。

## 將案例復製為範本

作為管理員，您能夠將案例復製為範本。

如需複製案例作為範本的說明，請參閱 [從情境建立範本](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) 在 [在中建立新範本 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
