---
product-area: projects
navigation-topic: use-the-home-area
title: 在首頁區域顯示[!UICONTROL 工作清單]中的專案
description: 每個Widget都包含自己的工作清單。 工作清單會顯示指派給您的所有工作專案。 您可以使用篩選器和群組來控制哪些專案顯示在[!UICONTROL 工作清單]中。
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 41f58261d4f2e6075187886b371a23eb5e97d823
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 4%

---

# 在[!UICONTROL 首頁]區域的[!UICONTROL 工作清單]中顯示專案

<!-- Audited: 1/2024 -->

每個Widget都包含自己的工作清單。 工作清單會顯示指派給您的所有工作專案。 您可以使用篩選器和群組來控制哪些專案顯示在[!UICONTROL 工作清單]中。

>[!IMPORTANT]
>
>* 若要在首頁Widget中顯示任務和問題，其父專案必須處於目前狀態或等於目前狀態。
>* 專案也必須處於目前狀態或等於目前顯示在首頁中的狀態。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權</strong></td> 
   <td><ul><li>[！UICONTROL參與者]僅供核准</li> <li>適用於所有其他物件的[！UICONTROL Standard]或更新版本</li> <p>或</p> 
  </ul><ul><li>[！UICONTROL Review]僅供核准</li> <li>適用於所有其他物件的[！UICONTROL Work]或更新版本</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>[！UICONTROL檢視]或更高的專案、任務、問題和檔案存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>貢獻您需要處理的任務和問題的許可權或更高</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 要在工作清單中顯示的工作專案需求

有內建需求，工作專案會針對這些需求顯示在特定Widget工作清單中。 工作專案必須符合這些要求，才能出現在下列Widget的工作清單中。

### 我的任務Widget

任務必須符合以下要求，才能出現在「我的任務」小工具中：

* 任務狀態不等於「完成」。
* 必須將登入使用者指派給任務。
* 任務狀態不等於「完成」。
* 任務所屬的專案必須處於與目前相同的狀態。


### 我的問題Widget

問題必須符合以下要求，才能出現在「我的問題」小工具中：

* 必須將登入使用者指派給問題。
* 問題狀態不等於「完成」。
* 沒有未解決的物件附加到問題。
* 問題狀態不等於「完成」。
* 問題所屬的專案必須處於與目前相同的狀態。

### 我的團隊Widget

團隊請求必須符合以下要求，才能出現在「我的團隊」小工具中：

* 登入使用者屬於指派工作專案的團隊。
* 工作專案狀態不等於「完成」。
* 工作專案沒有附加未解決的核准流程。
* 工作專案不是週期性任務。
* 工作專案所屬的專案必須處於與目前相同的狀態。

## 篩選您的工作

您可以篩選Widget的[!UICONTROL 工作清單]中的專案，以僅檢視特定型別的專案。 例如，您可以篩選「我的工作[!UICONTROL 工作清單]」以僅顯示問題或請求。

>[!NOTE]
>
>篩選器選項會儲存在瀏覽器中。 如果您一致在同一部電腦上使用相同的瀏覽器（且不清除網站資料），則請勿變更選取的篩選器。 如果您切換瀏覽器或電腦，則篩選器會還原為預設選項，該選項會取消選取所有篩選器。

若要篩選您的工作：

1. 按一下右上角的&#x200B;**[!UICONTROL 主功能表]** ![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）按一下&#x200B;**自訂**&#x200B;以新增下列任何Widget：

   | 小工具 | 說明 |
   |--------------|---------------------------------------------------------------------------------------------------|
   | 展示板 | 顯示您已建立或受邀使用的任何面板 |
   | 我的工作 | 顯示指派給您的任務和問題 |
   | 我的專案 | 顯示您擁有的專案或您所在的專案 |
   | 我的任務 | 顯示指派給您的任務 |
   | 我的問題 | 顯示指派給您的問題 |
   | 我的請求 | 顯示您已提交的所有請求 |
   | 我的核准 | 顯示所有擱置、已指派、已委派及已提交的核准 |

1. 按一下Widget工作清單右上角的&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-nwepng.png)。
1. 選擇&#x200B;**建議的**篩選器或您已建立的篩選器。
如需建議篩選的詳細資訊，請參閱[首頁Widget篩選總覽](/help/quicksilver/workfront-basics/using-home/using-the-home-area/widget-filter-overview-home.md)。
1. （選擇性）開啟&#x200B;**棧疊篩選器**&#x200B;以選取多個篩選器選項。

   ![我的任務篩選器已開啟](assets/my-task-filter-open.png)


## 將您的工作分組

您可以將Widget [!UICONTROL 工作清單]分組，讓您的工作專案維持井然有序。

若要將您的工作清單分組：

1. 按一下右上角的&#x200B;**[!UICONTROL 主功能表]** ![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）按一下&#x200B;**自訂**&#x200B;以新增下列任何Widget：

   | 小工具 | 說明 |
   |--------------|---------------------------------------------------------------------------------------------------|
   | 展示板 | 顯示您已建立或受邀使用的任何面板 |
   | 我的工作 | 顯示指派給您的任務和問題 |
   | 我的專案 | 顯示您擁有的專案或您所在的專案 |
   | 我的任務 | 顯示指派給您的任務 |
   | 我的問題 | 顯示指派給您的問題 |
   | 我的請求 | 顯示您已提交的所有請求 |
   | 我的核准 | 顯示所有擱置、已指派、已委派及已提交的核准 |

1. 按一下Widget工作清單右上角的&#x200B;**群組**&#x200B;圖示![群組圖示](assets/group-icon.png)。
1. 選擇一個&#x200B;**建議的**群組或您已建立的群組。
   ![群組已展開](assets/grouping-expanded.png)


## 自訂工作清單欄

您可以選擇要讓哪些欄出現在Widget工作清單中：

1. 按一下右上角的&#x200B;**[!UICONTROL 主功能表]** ![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）按一下&#x200B;**自訂**&#x200B;以新增下列任何Widget：

   | 小工具 | 說明 |
   |--------------|---------------------------------------------------------------------------------------------------|
   | 展示板 | 顯示您已建立或受邀使用的任何面板 |
   | 我的工作 | 顯示指派給您的任務和問題 |
   | 我的專案 | 顯示您擁有的專案或您所在的專案 |
   | 我的任務 | 顯示指派給您的任務 |
   | 我的問題 | 顯示指派給您的問題 |
   | 我的請求 | 顯示您已提交的所有請求 |
   | 我的核准 | 顯示所有擱置、已指派、已委派及已提交的核准 |

1. 按一下Widget工作清單右上角的&#x200B;**欄**&#x200B;圖示![欄圖示](assets/column-icon.png)。
1. 根據您的偏好設定開啟或關閉欄。
1. （選擇性）按一下&#x200B;**拖曳**&#x200B;圖示![拖曳圖示](assets/drag-icon.png)以重新排序欄。
   ![欄已展開](assets/columns-expanded.png)


## 檢視延遲專案

[!DNL Adobe Workfront]會使用以下日期來判斷工作請求是否延遲：

* **任務**： [!UICONTROL 計畫完成日期]
* **問題**： [!UICONTROL 規劃完成日期]
* **檔案**： [!UICONTROL 提交日期]
* **時程表**：[!UICONTROL 提交日期]
* **核准**： [!UICONTROL 提交日期]
* **校訂核准**： [!UICONTROL 校訂期限]


