---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion範本管理
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 8163f9f12bb27bbc8adfde34fc1e1f0f8c8be7f9
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]範本管理

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [核准或不核准公用索引標籤的範本](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/approve-templates.html)
>* [編輯範本](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/edit-templates.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

如果您是管理員，則擁有檢視、修改、重新命名、發佈、核准和刪除其他人建立的範本的許可權。 您可以從[!DNL Adobe Workfront Fusion Administration]區域的[!UICONTROL 範本]頁面執行這些動作。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
    <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是組織的Workfront Fusion管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 以[!DNL Workfront Fusion]管理員身分檢視[!DNL Workfront Fusion]範本

若要檢視所有已建立範本及其狀態的表格：

1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 管理]**&#x200B;以開啟[!UICONTROL 管理]區域。

   >[!NOTE]
   >
   >只有Workfront Fusion管理員能看見「管理」區域。

1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 範本]**。

有三個與範本發佈狀態相關的欄。 欄中的核取記號表示以下內容：

* **[!UICONTROL 已發佈]**：這些範本目前顯示在使用者介面的[!UICONTROL 團隊範本]索引標籤中。
* **[!UICONTROL 已要求核准]**：這些範本正等待您的核准。 它們目前顯示在使用者介面的[!UICONTROL 團隊範本]索引標籤中。
* **[!UICONTROL 已核准]**：這些範本已核准。 這些範本目前顯示在標準使用者介面的[!UICONTROL 公用範本]標籤中。

>[!NOTE]
>
>在[!UICONTROL 已要求核准]資料行和[!UICONTROL 已核准]資料行中同時具有核取記號的範本已核准並公開，但仍有較新版本的範本等待您的核准。

## 以管理員身分編輯[!DNL Workfront Fusion]範本

1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 管理]**&#x200B;以開啟[!UICONTROL 管理]區域。
1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 範本]**。
1. 按一下您要編輯的範本右邊的&#x200B;**[!UICONTROL 詳細資料]**。

您現在可以編輯範本，類似於以非管理員使用者的身分編輯範本。 但是，在右上角的[!UICONTROL 選項]中，有一個額外的選項 — 提供SVG程式碼的SVG圖表。 此外，發佈程式與標準使用者相同，請參閱發佈和共用範本一節以取得詳細資訊。

如需您可以編輯的特定範本選項相關資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)中建立新範本。

如需有關發佈範本的資訊，請參閱[Publish和共用 [!DNL Adobe Workfront Fusion] 範本](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md)。

## 核准或不核准[!DNL Workfront Fusion]範本

核准範本後，範本會顯示在[!UICONTROL 公用範本]標籤中，且可供所有使用者使用。 不核准範本會將其從[!UICONTROL 公用範本]標籤中移除，使其僅供建立該範本的團隊使用。

1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 管理]**&#x200B;以開啟[!UICONTROL 管理]區域。
1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 範本]**。
1. 若要核准範本，請按一下範本右側的&#x200B;**[!UICONTROL 核准]**。
1. 如果您要取消核准範本，請按一下範本右側的&#x200B;**[!UICONTROL 取消核准]**。

>[!NOTE]
>
>如果您核准先前已核准然後編輯的範本，則您的第二次核准將會覆寫原始範本。

## 將案例復製為範本

身為管理員，您可以複製案例作為範本。

如需將案例復製為範本的說明，請參閱[在 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)中建立新範本[從案例建立範本](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario)
