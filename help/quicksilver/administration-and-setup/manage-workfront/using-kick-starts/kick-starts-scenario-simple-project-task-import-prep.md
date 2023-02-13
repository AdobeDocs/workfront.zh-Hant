---
user-type: administrator
product-area: system-administration;projects
keywords: kickstart,kickstart,kickstarts,kickstarts
navigation-topic: use-kick-starts
title: Kick-Starts情境 — 簡單項目和任務導入準備
description: 詳細說明使用「啟動」方法導入基本項目和任務的可用設定和控制項。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c095ce9d-b189-449b-bd13-2633837697ed
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 9%

---

# Kick-Starts案例：簡單的項目和任務導入準備

詳細說明使用「啟動」方法導入基本項目和任務的可用設定和控制項。

## 情境

實施團隊寧可匯入作用中專案的專案和任務資訊，也不願手動將這些資料輸入系統。

* [專案](#projects)
* [任務清單](#task-list)

### 專案 {#projects}

下表顯示需要映射為Kick Start檔案格式的四個項目及其基本詳細資訊。

此案例假設使用者已匯入Adobe Workfront。 如果使用者尚未進入Workfront，請在此案例之前，替換不同名稱或與使用者完成「開始」案例。

1. 實作Workfront。

   | 計畫開始日期 | 今天 |
   |---|---|
   | 專案經理 | 詹妮弗·坎貝爾 |
   | 專案贊助者 | 馬克·路易斯 |
   | 群組 | 行銷 |
   | 公司 | *YourCompany* |

   {style=&quot;table-layout:auto&quot;}

1. 實施人力資源系統。

   | 計畫開始日期 | 20XX年7月14日 |
   |---|---|
   | 專案經理 | 帕姆·雷諾茲 |
   | 專案贊助者 | 馬克·路易斯 |
   | 群組 | 行銷 |
   | 公司 | *YourCompany* |

   {style=&quot;table-layout:auto&quot;}

1. 實作檔案管理系統。

   | 計畫開始日期 | 20XX年8月22日 |
   |---|---|
   | 專案經理 | 詹妮弗·坎貝爾 |
   | 專案贊助者 | 雷·安德魯斯 |
   | 群組 | IT |
   | 公司 | *YourCompany* |

   {style=&quot;table-layout:auto&quot;}

1. 實作新的日曆系統。

   | 計畫開始日期 | 20XX年9月6日 |
   |---|---|
   | 專案經理 | 帕姆·雷諾茲 |
   | 專案贊助者 | 雷·安德魯斯 |
   | 群組 | IT |
   | 公司 | *YourCompany* |

   {style=&quot;table-layout:auto&quot;}

### 任務清單 {#task-list}

以下任務清單顯示了項目的過簡化的任務清單。 專案之間的唯一差異是每個專案的開始日期和進度。

父任務繼承子任務的「持續時間」、「工作」和「完成百分比」。 不需要為這些值設定，這些值將成為摘要任務。

>[!NOTE]
>
>本案例中提供的指示不像 [啟動方案：公司、組、角色和用戶啟動準備](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-company-group-role-user-prep.md). 假設是您已學習如何從公司和集團工作表中查找和複製值，因此將提及這些步驟，但並未具體說明。

1. 設定.
1. 匯入使用者。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">指派至</td> 
      <td>雷·安德魯斯</td> 
     </tr> 
     <tr> 
      <td role="rowheader">父任務</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>1 小時</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>1 小時</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>檔案：100%</p> <p>日曆：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 設定權限。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">指派至</td> 
      <td>雷·安德魯斯</td> 
     </tr> 
     <tr> 
      <td role="rowheader">父任務</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">前置任務</td> 
      <td>2</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>1 小時</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>1 小時</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>檔案：100%</p> <p>日曆：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 建立群組。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">指派至</td> 
      <td>雷·安德魯斯</td> 
     </tr> 
     <tr> 
      <td role="rowheader">父任務</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">前置任務</td> 
      <td>4</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>2 天</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>4 小時</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>檔案：100%</p> <p>日曆：25%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 準備培訓。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">指派至</td> 
      <td>克里斯·曼寧</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>2 天</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>4 小時</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>檔案：50%</p> <p>日曆：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 構建持續的支援策略。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">指派至</td> 
      <td>克里斯·曼寧</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>2 天</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>4 小時</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>檔案：50%</p> <p>日曆：0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 滾。

   | 前置任務 | 1, 6, 7 |
   |---|---|

   {style=&quot;table-layout:auto&quot;}

1. 培訓用戶。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">指派至</td> 
      <td>克里斯·曼寧</td> 
     </tr> 
     <tr> 
      <td role="rowheader">父任務</td> 
      <td>8</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>1 天</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作</td> 
      <td>2 小時</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>Workfront:0%</p> <p>HR:0%</p> <p>檔案：0%</p> <p>日曆：0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 下載範本

前往「開始」頁面。 選擇公司、組、項目、任務和用戶對象。 選取「包含現有資料」核取方塊（這麼做可快速參考公司、群組和使用者ID）。 按一下「下載」按鈕。

## 輸入項目詳細資訊

開啟您剛下載的Workfront.xlsx檔案。 轉到PROJ項目工作表。

![](assets/im2-350x14.png)\
除非您已在Workfront中建立專案，否則專案應為空。\
![](assets/im3-350x37.png)

>[!NOTE]
>
>請考慮使用試算表的「凍結窗格」工具和/或隱藏或移除不需要的欄，讓工作表更易於使用。 但請留意，請勿移除任何後續使用的必要欄或欄。

![](assets/im10-350x42.png)

設定下列專案欄位的值：

* **Set isNew列**
將TRUE輸入到行3到行6中的isNew列。
* **設定唯一ID**
為ID列在每一行中輸入唯一ID — 通常，從1開始的整數在建立新記錄時工作正常。
* **設定專案名稱**
將每個項目的名稱輸入setName列中。
* **設定專案排程**

   在setScheduleID欄位中輸入要項目使用的計畫ID

* **設定項目計畫起始日期**

   在setPlannedStartDate列中輸入日期和時間，以及您希望項目開始的時間和日期。 如果保留為空白，Workfront會根據瀏覽器的時區，匯入包含當天日期和當天午夜時間戳記的專案。

* **設定任務編號**
將值輸入setTaskNumber列，以控制任務在項目計畫中的顯示順序。
* **提供專案日期。**
在setPlannedStartDate列中輸入每個項目的計畫起始日期。
* **設定其他需要的詳細資訊。**
視需要填入其他詳細資訊，例如說明或目前狀態。 在「組組」工作表上查找每個項目的組ID，並將它們輸入到相應項目的setGroupID列中。 在「CMPY公司」工作表上查找項目的公司ID，並將其輸入到setCompanyID列中。 在「用戶」(USER)工作表上查找每個項目所有者的用戶ID，並將其輸入到setOwnerID列中。 查找「用戶」(USER)工作表上每個項目贊助商的用戶ID，並將其輸入到setPonsorID列中。

![](assets/im9-350x24.png)

>[!NOTE]
>
>在Workfront的「工作流設定」區域中，查看每個物件的狀態和優先順序偏好設定，即可找到「狀態」和「優先順序」欄位的可接受值。

## 輸入任務詳細資訊

使用啟動匯入專案時，您可以新增有關專案工作的資訊。

開啟您剛下載的Workfront.xlsx檔案。 **轉到「任務」工作表。**

除非您已在Workfront中建立任務，否則此工作表應為空。

![](assets/im8-350x14.png)

![](assets/im7-350x43.png)

![](assets/im6-350x16.png)

要映射任務，最簡單的方法是一次一個項目（尤其是當每個項目的任務相同時）。 然後，您可以複製第一個項目的任務計畫，並對後續項目的任務計畫進行小幅調整。 其餘步驟將假設您僅為實作Workfront專案建立工作。 根據情況，您將每個項目導入9個任務，因此，為isNew列將TRUE輸入到第3到第11行。

為以下任務欄位設定值：

* **設定ID**
在ID欄的每一列輸入唯一ID。
* **設定名稱**
將任務名輸入setName列。
* **確認專案ID**
輸入您為實作Workfront專案設定的ID;查看「PROJ項目」工作表，確保它是正確的ID。
* **設定使用者**
轉到「用戶」工作表，查找分配給每個任務的用戶的ID，並將這些值輸入setAssignedToID列的相應單元格中。
* **確定任務關係**
對於任務2到5，在setParentID列中輸入1。 對於任務9，在setParentID列中輸入8。 在setPacisomentString列中，輸入每個前置任務的任務編號。 如果任務有多個前置任務，如此情況下的任務8，則需要使用逗號來分隔每個前置任務ID。 可以使用建立前置關係文章中描述的速記，在非完成開始關係上定義前置任務時滯。
* **設定持續時間**
在setDuration欄位中輸入任務的小時、天、周或月數，以設定每個任務的持續時間。 然後在setDurationUnit欄位中輸入持續時間單位。

   |  | 可接受值 |
   |---|---|
   | 分鐘 | 一 |
   | 時數 | H |
   | 天 | D |
   | 週 | 三 |
   | 月 | 二 |

   分鐘也可以呈現為一小時（例如，分鐘= 5小時）的一小部分

* 在setWorkRequired欄位中設定每個任務的工作量。 然後在setWorkUnit欄位中輸入工作單元。 如果「需要工作」值與持續時間不同，則還需要在setDurationType欄位中輸入A。

   | 期間類型 | 可接受值 |
   |---|---|
   | 已計算的任務指派 | A |
   | 已計算的工作 | 三 |
   | 投入比導向 | D |
   | 簡單 | 日 |

* 在setPercentComplete欄位中輸入每個任務的完成百分比的整數表示。 此值不應包含百分比符號(%)。
* 視需要為您建立的每個任務包括說明和其他詳細資訊。

   ![](assets/im5-350x35.png)

* setPlaninedStartDate和setTaskConstraint列不用於構建此項目的時間軸，因為我們依賴前置關係。 您可以輸入每個任務的日期。 如果執行此操作，請確保在setTaskConstraint列中也提供有效的任務約束。 有關此欄位有效值的詳細資訊，請查看任務約束和相關文章。

   在這種情況下，為要導入的其他項目生成任務最簡單的方法是從第12行開始複製剛定義的任務並貼到下面。 然後您會：

   1. 重新編號ID欄中的值。
   1. 將setProjectID欄更新為您為下一個專案設定的值。
   1. 更新setParentID和setParentString值，以反映分配給此項目任務的新ID。
   1. 更新任務分配和完成百分比。
   1. 對下一個項目的任務重複這些步驟。

* **匯入Excel檔案**

   按照 [使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
