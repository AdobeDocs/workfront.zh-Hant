---
product-area: user-management
navigation-topic: configure-your-user-profile
title: 建立自訂區段
description: 您在 [!DNL Workfront] 依預設，Web應用程式通常會顯示在左側面板的區段中。 每個區段包含 [!DNL Workfront] 區域或對象。
author: Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 3%

---

# 建立自訂區段

## [!DNL Adobe Workfront] 區段

您在 [!DNL Workfront] 依預設，網頁應用程式通常會顯示在左側面板區段中。 每個區段包含 [!DNL Workfront] 區域或對象。\
如需的預設區域相關資訊，請參閱 [!DNL Workfront]，請參閱文章 [關於預設值 [!DNL Adobe Workfront] 配置](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

除了 [!DNL Workfront] 依預設，您可以新增控制面板，在其中顯示與工作流程相關的資訊。 無法將控制面板添加到所有區域和對象。

下表列出 [!DNL Workfront] 左側面板中包含區段的區域和對象，以及可自定義的區段和對象：

| **[!DNL Workfront]區域或對象** | **預設系統部分** | **自訂區段** |
|---|---|---|
| [!UICONTROL 專案] 區域 | ✓ | ✓ |
| [!UICONTROL 團隊] | ✓ |   |
| [!UICONTROL 請求] 區域 | ✓ |   |
| [!UICONTROL 工時單] 區域 | ✓ |   |
| [!UICONTROL 專案組合] | ✓ | ✓ |
| [!UICONTROL 方案] | ✓ | ✓ |
| [!UICONTROL 專案] | ✓ | ✓ |
| [!UICONTROL 任務] | ✓ |  ✓ |
| [!UICONTROL 問題] |  ✓ |  ✓ |
| [!UICONTROL 使用者] |  ✓ |  ✓ |
| [!UICONTROL 文件] |  ✓ |  ✓ |

{style=&quot;table-layout:auto&quot;}

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td>[!UICONTROL Reviewer]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td>查看對對象類型的訪問</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請連絡您的 [!DNL Workfront] 管理員。

## 在 [!DNL Workfront] 對象或區域

您必須先建立控制面板，並在其上顯示所有資訊，才能新增控制面板。 您也可以建立外部頁面。\
如需有關建立控制面板的詳細資訊，請參閱文章 [建立控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
如需有關建立外部頁面的詳細資訊，請參閱文章 [在控制面板中內嵌外部網頁](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

建置控制面板或外部頁面後，您可以將它們新增至左側面板。

1. 轉到 [!DNL Workfront] 可在左側面板中新增自訂區段的區域或物件。\
   或
1. 前往可新增 [!UICONTROL 儀表板] 中。\
   有關可以添加自定義節的區域和對象的詳細資訊，請參見 [[!DNL Adobe Workfront] 區段](#adobe-workfront-sections).
1. 按一下 **[!UICONTROL 新增控制面板]** 中。
1. 在 **[!UICONTROL 快速連結名稱]** 欄位。 這隻對您可見。
1. 開始在 **[!UICONTROL 選擇控制面板]** 欄位中，然後選取顯示在清單中的控制面板。
1. 按一下 **[!UICONTROL 新增]**.
1. （選用）依照您要顯示區段的順序來拖放區段。

   頂端區段是頁面的預設區段。

   訪問所有同類型對象時，您為單個對象建立的節將顯示，並且只對您可用。

## 在對象的左側面板中顯示控制面板

如需在物件下新增控制面板的詳細資訊，請參閱區段 [[!UICONTROL 新增控制面板] 在Workfront物件或區域的左側面板中](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) 這篇文章。

將控制面板新增至物件下的自訂區段時，物件會作為控制面板的篩選器。 例如，如果在控制面板上添加任務報告並將控制面板添加到項目，則包含項目上控制面板的自定義部分將僅顯示您正在查看的項目上的任務。

如果該對象的層次結構高於它們，則會篩選其顯示所在對象的以下對象：

* 專案
* 任務
* 問題
* 核准流程
* 備註
* 文件

有關對象的層次結構和互依關係的詳細資訊，請參閱一節 [對象的相互依存和層次](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 在版面範本中自訂左側面板

將控制面板新增至 [!DNL Workfront] 例項，則只有您可看到。

您可以自訂 [!DNL Workfront] 並與版面範本中的多名使用者共用新版面。 只有系統或群組管理員才能與版面範本中的其他使用者共用這些內容。 如需使用版面範本自訂左側面板的詳細資訊，請參閱 [使用版面範本自訂左側面板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
