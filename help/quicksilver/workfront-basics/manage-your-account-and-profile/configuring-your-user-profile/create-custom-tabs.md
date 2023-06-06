---
product-area: user-management
navigation-topic: configure-your-user-profile
title: 建立自訂區段
description: 您在中看到的資訊 [!DNL Workfront] 根據預設，Web應用程式通常會顯示在左側面板的區段中。 每個區段都包含關於 [!DNL Workfront] 區域或物件。
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 2%

---

# 建立自訂區段

## [!DNL Adobe Workfront] 區段

您在中看到的資訊 [!DNL Workfront] 根據預設，Web應用程式通常會顯示在左側面板區段中。 每個區段都包含關於 [!DNL Workfront] 區域或物件。\
如需預設區域的詳細資訊， [!DNL Workfront]，請參閱文章 [關於預設值 [!DNL Adobe Workfront] 版面](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

除了隨附的章節以外 [!DNL Workfront] 依預設，您可以新增一個儀表板，以顯示與工作流程相關的資訊。 您無法將儀表板新增到所有區域和物件。

下表列出所有 [!DNL Workfront] 包含左側面板中區段以及可自訂區段的區域和物件：

| **[!DNL Workfront]區域或物件** | **預設系統區段** | **自訂部分** |
|---|---|---|
| [!UICONTROL 專案] 區域 | ✓ (N) | ✓ |
| [!UICONTROL 團隊] | ✓ |   |
| [!UICONTROL 請求] 區域 | ✓ |   |
| [!UICONTROL 時間表] 區域 | ✓ |   |
| [!UICONTROL 專案組合] | ✓ | ✓ |
| [!UICONTROL 方案] | ✓ | ✓ |
| [!UICONTROL 專案] | ✓ | ✓ |
| [!UICONTROL 任務] | ✓ |  ✓ |
| [!UICONTROL 問題] |  ✓ |  ✓ |
| [!UICONTROL 使用者] |  ✓ |  ✓ |
| [!UICONTROL 文件] |  ✓ |  ✓ |

{style="table-layout:auto"}

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td>[！UICONTROL Reviewer]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td>檢視物件型別的存取權</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫或授權型別，請連絡 [!DNL Workfront] 管理員。

## 在的左側面板中新增儀表板 [!DNL Workfront] 物件或區域

在新增儀表板之前，您必須先建立儀表板，其中包含您要在其上顯示的所有資訊。 您也可以建置外部頁面。\
如需有關建立儀表板的詳細資訊，請參閱文章 [建立控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
如需有關建立外部頁面的詳細資訊，請參閱文章 [將外部網頁內嵌在儀表板中](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

建立儀表板或外部頁面後，您可以將其新增到左側面板。

1. 前往其中一項 [!DNL Workfront] 可在左側面板中新增自訂區段的區域或物件。\
   或
1. 前往可以新增的物件 [!UICONTROL 儀表板] 在左側面板中。\
   如需可新增自訂區段的區域和物件的詳細資訊，請參閱 [[!DNL Adobe Workfront] 區段](#adobe-workfront-sections).
1. 按一下 **[!UICONTROL 新增儀表板]** 在左側面板中。
1. 在「 」中輸入儀表板名稱 **[!UICONTROL 快速連結名稱]** 欄位。 只有您能看見。
1. 開始在「 」中輸入現有儀表板或外部頁面的名稱 **[!UICONTROL 選擇儀表板]** 欄位，然後選取在清單中顯示的控制面板。
1. 按一下 **[!UICONTROL 新增]**.
1. （可選）以您要顯示的順序拖放區段。

   頂端區段是頁面的預設區段。

   您為個別物件建立的區段會在您存取相同型別的所有物件時顯示，而且僅供您使用。

## 在物件的左側面板中顯示儀表板

如需在物件下新增控制面板的詳細資訊，請參閱區段 [[!UICONTROL 新增儀表板] Workfront物件或區域的左側面板中](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) 本文章內容。

當您將儀表板新增到物件下的自訂區段時，該物件會充當儀表板的濾鏡。 例如，如果您在儀表板上新增任務報告，並將儀表板新增到專案，則包含專案儀表板的自訂區段僅顯示您正在檢視的專案上的任務。

如果物件的階層高於顯示物件的階層，則會針對顯示物件的物件篩選下列物件：

* 專案
* 任務
* 問題
* 核准流程
* 備註
* 文件

如需物件的階層與相依性的詳細資訊，請參閱區段 [物件的相依性和階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 自訂版面配置範本中的左側面板

當您新增儀表板到 [!DNL Workfront] 例如，只有您能看見。

您可以自訂以下專案的區段： [!DNL Workfront] 並在版面配置範本中與多位使用者共用新版面。 只有系統或群組管理員才能與版面配置範本中的其他使用者共用它們。 如需使用版面配置範本自訂左側面板的詳細資訊，請參閱 [使用版面配置範本自訂左側面板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
