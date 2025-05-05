---
navigation-topic: get-started-with-workfront
title: 在優先順序行事曆中管理您的工作
description: 使用清晰的視覺行事曆追蹤您的工作。
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: d24ad7d1-3a88-479e-beaf-69f8264c9a6b
source-git-commit: 20cb2237a534b51ab5c75e393369bdd92c233efb
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 4%

---

# 在優先順序行事曆中管理您的工作

透過清晰的視覺行事曆，輕鬆追蹤您的工作。 使用「優先順序」行事曆，您可以

* 使用篩選器尋找您的工作
* 套用狀態和焦點層級等自訂欄位以識別高優先順序的工作
* 套用快速組織的顏色

>[!IMPORTANT]
>
>專案必須處於目前狀態或等於目前的狀態，才能顯示專案及其子任務和問題。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> 
   <p>目前：檢閱者或以上</p>
   <p>新增：淺色或更高</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>檢視或編輯更新所在物件的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>檢視物件的存取權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視您在行事曆中的工作

優先順序顯示指派給您的工作專案。 您無法在優先順序行事曆中看到指派給團隊的工作專案。

{{step1-to-priorities}}

1. 按一下工作清單頂端的「行事曆」圖示。
   ![行事曆圖示](assets/calendar-tab.png)
1. 選取一或多個篩選器以縮小您的工作專案。

   +++展開以檢視有關可用篩選器的詳細資訊
   <table>
    <tbody>
    <tr>
    <th>篩選器</th>
    <th>說明</th>
    </tr>
        <tr>
        <td>正在處理</td>
        <td>顯示您目前正在處理的專案</td>
        </tr>
        <tr>
        <td>已就緒可開始</td>
        <td>顯示專案與 
        <ul>
        <li>沒有未完成的前置任務或任務限制</li>
        <p>和</p>
        <li>計劃開始日期是過去或未來最多兩週</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>尚未就緒</td>
        <td>顯示具有
        <ul>
        <li>未完成的前置任務或無法處理專案的任務限制</li>
        <p>或</p>
        <li>超過兩週的計劃開始日期</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>已請求</td>
        <td>顯示您尚未開始處理的問題</td>
        </tr>
        <td>完成</td>
        <td>顯示過去兩週內完成的工作。 此篩選選項不包含核准。</td>
        </tr>
        <tr>
        <td>專案</td>
        <td>顯示包含您已受指派的任務或問題的專案</td>
        </tr>
        <tr>
        <td>到期日期</td>
        <td>按計畫完成日期顯示工作</td>
        </tr>
        <tr>
        <td>狀態</td>
        <td>顯示新增、進行中和完成狀態的任務或問題</td>
        </tr>
        <tr>
        <td>我的焦點</td>
        <td>顯示中已指派焦點層級的任務或問題。 焦點層級是由個別使用者指派和管理。</td>
        </tr>
    </tbody>
    </table>

   +++

1. 按一下行事曆中的工作專案列以開啟側邊摘要。 側邊摘要可讓您

* 檢視和編輯專案和工作專案詳細資訊
* 建立及檢視註解
* 檢視和上傳檔案
* 建立校訂
* 導覽至Workfront中的專案頁面
* 導覽至「優先順序」中的工作專案詳細資訊頁面
* 記錄時間
* 新增快速連結

1. （選擇性）按一下[新建] **&#x200B;**&#x200B;以新增工作專案至行事曆。 如需詳細資訊，請參閱[在優先順序](/help/quicksilver/workfront-basics/priorities/create-task-issue-priorities.md)中建立新任務或問題。

## 設定日曆

{{step1-to-priorities}}

1. 按一下工作清單頂端的「行事曆」圖示。
   ![行事曆圖示](assets/calendar-tab.png)
1. 按一下行事曆右角的&#x200B;**設定**&#x200B;圖示。

1. 在&#x200B;**列樣式**&#x200B;標籤上，選擇最多5個欄位顯示在行事曆的工作專案列上。
   ![範例列](assets/sample-task-for-field-config.png)

1. 在&#x200B;**色彩**&#x200B;標籤上，選擇您要如何顯示工作專案。 例如，如果您選擇「專案」，您的工作專案會根據工作清單上指定給專案的顏色顯示。
   ![顏色專案範例](assets/sample-calendar-projects.png)
