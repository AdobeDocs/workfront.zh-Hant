---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 復原環境升級套件
description: 環境推進功能旨在提供與組態相關的物件從一個環境移動到另一個環境的功能。 瞭解如何從目標環境復原已安裝的促銷活動套件。
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
source-git-commit: 7e15301dae4b761d19c85a3581bfdb4540ed40fd
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# 復原環境升級套件



安裝套裝軟體後，您可以將其回覆。 這會移除封裝在目標環境中所做的變更，並將受影響的物件還原為其先前的組態。

您可以在促銷活動套件安裝後24小時內將其回覆。 24小時後，該安裝將無法再使用復原功能。

## 存取需求

您必須具備下列條件：

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront]計畫</strong>
   </td>
   <td> <p>新增：Prime或Ultimate</p><p>或</p><p>目前：無法使用</p>
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront]個授權</strong>
   </td>
   <td> <p>[！UICONTROL標準]</p><p>或</p><p>目前：無法使用</p>
   </td>
  </tr>
   <tr>
   <td>存取層級設定
   </td>
   <td>您必須是[!DNL Workfront]管理員。
   </td>
  </tr>
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先決條件

* 必須先安裝環境升級套件，然後才能將其復原。

  如需指示，請參閱[安裝環境升級套件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)。


## 決定是否可復原特定套件部署

若要瞭解特定套件部署是否可以回覆，請考慮下列事項：

* 安裝套件後必須經過少於24小時。
* 只能復原最近的套件部署。
* 失敗的部署可以回覆。
* 無法復原回滾。


## 復原已安裝的環境升級套件

1. 前往安裝套件的環境。
1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 在左側導覽中選取&#x200B;**環境促銷活動**。
1. 選取您要復原的封裝，然後按一下&#x200B;**部署**。
1. 將游標暫留在您要復原的部署（安裝）上，然後在該部署行的右側出現時按一下復原。

   或

   按一下您要復原的部署，然後按一下畫面右上角的&#x200B;**復原套件**。

   >[!IMPORTANT]
   >
   >在您復原部署之前，部署必須少於24小時。 超過24小時的安裝無法回覆。

1. （選擇性）在「復原預覽」區域中，檢視部署復原時將發生的變更。
1. 按一下熒幕右上角的&#x200B;**回覆**。
