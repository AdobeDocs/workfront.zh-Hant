---
navigation-topic: get-started-with-workfront
title: 使用優先順序篩選及分組您的工作
description: 您可以使用篩選器來尋找您要尋找的工作，然後套用分組，讓工作保持井然有序。
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: 8eb9dcaf-bba3-466d-b06d-5383991bc4ea
source-git-commit: 20cb2237a534b51ab5c75e393369bdd92c233efb
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 4%

---

# 使用優先順序篩選及分組您的工作

您可以使用篩選器來尋找您要尋找的工作，然後套用分組以使其保持井然有序。

優先順序顯示指派給您的工作專案。 您無法在「優先順序」工作清單中看到指派給您團隊的工作專案。

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
   <p>目前：要求或以上</p>
   <p>新增：投稿人或更高版本</p> 
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

## 使用標準篩選器篩選您的工作

您可以篩選指派給您的任務和問題。

{{step1-to-priorities}}

1. 按一下工作清單左上角的&#x200B;**篩選器**。
1. 按一下&#x200B;**標準篩選器**。
1. 選取一個或多個篩選器以縮小您的工作專案。
   ![](assets/filter-new.png)

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

1. （選擇性）按一下&#x200B;**返回預設值**&#x200B;以重設您的選擇。

## 使用智慧型篩選器篩選您的工作

使用自然語言來篩選快速篩選工作。 您的Workfront執行個體必須在新的Workfront計畫上，並在Adobe Unified Experience上啟用。 如需詳細資訊，請參閱[適用於Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

{{step1-to-priorities}}

1. 按一下工作清單左上角的&#x200B;**篩選器**。
1. 按一下&#x200B;**智慧型濾鏡**。
1. 輸入您要如何篩選您的工作。

   您可以輸入類似以下的內容

   * 顯示延遲任務
   * 顯示我最優先的順序
   * 顯示今天到期的工作

</div>

## 將您的工作分組

{{step1-to-priorities}}

1. 按一下工作清單左上角的&#x200B;**群組**。
1. 選取群組以組織您的工作清單
   ![](assets/groups-new.png)

+++展開以檢視有關可用群組的詳細資訊

| 群組 | 說明 |
|-----------|-------------|
| 專案 | 這會依專案分組專案。 |
| 我的焦點 | 這會根據您指派的焦點層級來分組專案。 |
| 到期週數 | 這會將專案依其到期周分組。 到期日由計畫完成日期決定。 |
| 狀態 | 這會依下列狀態分組專案：新增、進行中、完成。 <br>注意：您目前無法在[優先順序]中使用自訂狀態。 |

+++

### 依「我的優先順序」或「狀態」分組時，拖放工作專案

按「我的優先順序」或「狀態」分組時，您可以在類別之間拖放個別工作專案。

1. 依&#x200B;**狀態**&#x200B;或&#x200B;**我的優先順序**&#x200B;將您的工作分組。
2. 將滑鼠停留在工作專案上以尋找移動圖示，並將其拖曳到所需的類別。
   ![拖曳圖示](assets/drag-and-drop.png)

## 排序您的工作

### 按群組排序

若要排序群組中的工作，請開啟&#x200B;**群組**&#x200B;並按一下&#x200B;**遞增排序**&#x200B;或&#x200B;**遞減排序**。

![](assets/sort-in-groups.png)

### 排序欄

若要排序個別欄，請移至欄並按一下向下箭頭。

![欄](assets/sort-columns.png)中的向下箭頭

### 展開或摺疊所有群組區段

若要展開或收合所有群組區段，請開啟&#x200B;**群組**&#x200B;並按一下&#x200B;**全部展開**&#x200B;或&#x200B;**全部收合**。

![](assets/expand-collapse-groups.png)