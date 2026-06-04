---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 篩選器按鈕未顯示在頁首中
description: 請參閱本文以疑難排解頁面標頭中未顯示的篩選器按鈕。
feature: Get Started with Workfront
author: Courtney
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
TQID: https://experienceleague.adobe.com/36hMJKo4unpIxvUOmBk79XlhFvFL5TgqUaoQXxrPd7c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 10%

---

# 篩選器按鈕未顯示在頁首中

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table>
  <tr>
   <td>Adobe Workfront 封裝
   </td>
   <td>任何</td>
  </tr>
  <tr>
   <td>Adobe Workfront 授權
   </td>
   <td><p>標準</p>
   <p>規劃</p>
   </td>
  </tr>
   <tr>
   <td>存取層級設定
   </td>
   <td>您必須是[!DNL Workfront]管理員。
   </td>
  </tr>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 問題

下列篩選按鈕不會顯示在其各自的區域中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] 區域</strong></td> 
   <td><strong>篩選按鈕</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 專案] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL 我所在的專案]</p> </li> 
     <li> <p>[!UICONTROL 我擁有的專案]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL 時程表]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL 我的時程表核准]</span> </p> </li> 
     <li> <p><span>[!UICONTROL 我的時程表]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

[!UICONTROL 專案和時程表]區域中的篩選器按鈕未顯示，因為套用至使用者的版面配置範本中未包含對應的篩選器。 [!DNL Workfront]管理員必須指派包含篩選器的配置範本。

>[!NOTE]
>
>有時篩選器會從[!UICONTROL 設定]中的[!UICONTROL 清單控制項]區域移除。 [!DNL Workfront]管理員必須包含在此區域的清單中，才能在版面配置範本中使用。

1. 確認版面配置範本顯示下列篩選器：

   * [!UICONTROL 我所在的專案]和我擁有的[!UICONTROL 專案] （在[!UICONTROL 專案]區域中）
   * [!UICONTROL 我的時程表核准]和[!UICONTROL 我的時程表] （在[!UICONTROL 時程表]區域中）

   操作步驟：

   1. 存取配置範本。
   1. 選取&#x200B;**[!UICONTROL 自訂使用者看到的內容]**&#x200B;下的&#x200B;**[!UICONTROL 清單]**。
   1. 選取&#x200B;**[!UICONTROL 下的**&#x200B;[!UICONTROL &#x200B;專案&#x200B;]&#x200B;**或**&#x200B;[!UICONTROL &#x200B;時程表&#x200B;]&#x200B;**選取要自訂的清單]**。
   1. 在&#x200B;**[!UICONTROL 篩選器]**&#x200B;區段中，確認已選取&#x200B;**[!UICONTROL 我所在的專案]**、**[!UICONTROL 我擁有的專案]** （針對專案）及&#x200B;**[!UICONTROL 我的時程表核准]**&#x200B;和&#x200B;**[!UICONTROL 我的時程表]** （針對時程表）。
   1. 按一下「**[!UICONTROL 儲存]**」。

   如需詳細資訊，請參閱[使用配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

1. 將版面配置範本指派給正確的使用者、工作角色、團隊或群組。 如需詳細資訊，請參閱[將使用者指派給配置範本](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。
