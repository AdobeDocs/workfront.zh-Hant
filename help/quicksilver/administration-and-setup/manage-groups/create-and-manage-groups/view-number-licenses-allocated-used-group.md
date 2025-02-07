---
title: 檢視群組中配置及使用的授權數目
description: 身為Adobe Workfront管理員，您可以檢視目前用於群組及其子群組的個別授權型別計數。 當您需要評估是否重新分配授權時，這個選項非常有用。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# 檢視群組中配置及使用的授權數目

身為Adobe Workfront管理員，您可以檢視目前用於群組及其子群組的個別授權型別計數。 當您需要評估是否重新分配授權時，這個選項非常有用。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

>[!IMPORTANT]
>
>只有當群組是使用者的「主群組」時，才會在特定群組中計算使用者的授權。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視群組中使用的授權數目

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

1. 按一下群組的名稱。
1. 在顯示的頁面上，在右上角附近的標頭區域中，檢視&#x200B;**使用中的授權**&#x200B;區域，以檢視目前使用的&#x200B;**計畫**&#x200B;和&#x200B;**工作**&#x200B;授權數目。

   如果您檢視的是頂層群組，而Workfront管理員已為群組定義了每個授權型別的最大數量，這些數字也會顯示。 例如，在下列群組中，最多10名使用者可以擁有「計畫」授權，15名使用者可以擁有「工作」授權：

   ![已配置的授權](assets/licenses-used-allocated.png)

   如需Workfront管理員如何定義群組最大分配授權數目的詳細資訊，請參閱[管理系統中的可用授權](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)一文中的[設定主群組的授權數目上限](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set)小節。

   >[!NOTE]
   >
   >如果您要檢視的群組是子群組，您只能檢視正在使用的授權數目，而非配置給該群組的授權數目上限。 這是因為Workfront管理員不會為子群組定義授權數量上限。
   >
   >![在子群組](assets/subgroup-used-licenses-only.png)中使用授權
   >

1. 如需群組目前使用的每種授權型別（包括檢閱和要求）的個別計數，請按一下&#x200B;**使用中授權正下方的文字區域：**

   ![按一下以檢視更多](assets/click-text-to-see-more.png)

   顯示的方塊針對所有四種Workfront授權型別提供相同的資訊：計畫、工作、稽核和請求。 在方塊底部，您可以看到此群組或其子群組的成員所使用的授權總數：

   ![更多授權資訊](assets/more-license-info.png)

   對於「檢閱和請求」授權，「最大值」欄一律顯示「無限制」。
