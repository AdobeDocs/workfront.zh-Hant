---
title: AI助理提示最佳實務
content-type: reference
description: 瞭解使用AI助理的最佳實務，並檢視提示範例清單。
author: Jenny
feature: Get Started with Workfront
exl-id: 34a60482-e060-49f9-bbaf-8aed85845e26
source-git-commit: 4bab0129d694d7134a5dae90474678226368ca78
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 4%

---

# AI助理提示最佳實務

Workfront的AI Assistant是一款功能強大的工具，可協助您提供關於帳戶資料和特定物件型別的有用資訊，以更有效完成工作。

在本文中，您將瞭解AI助理的目前最佳實務，包括如何撰寫清除提示、您可以要求哪些物件型別提供資訊，以及如何在需要時存取其他資源以驗證資訊。

如需AI助理的詳細資訊，請參閱[AI助理概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。

>[!NOTE]
>
>隨著AI Assistant功能的發展，您可以詢問它的請求和問題型別將會增加。 建議您重新瀏覽本文，因為新的AI助理功能已發行，以深入瞭解您可以使用的可用提示。


## AI助理可用的物件型別

AI助理可以提供下列物件型別的資料：

* 專案組合
* 計劃
* 專案
* 任務
* 問題
* 自訂表單
* 使用者
* Workfront Planning記錄

>[!NOTE]
>
>您必須擁有物件存取層級的必要許可權，才能向AI助理要求其資料。

## 最佳做法

### 輸入清除提示

若要從AI助理存取最有用的資訊，請務必建立提示，提供您正在尋找的回應。 下列清單包含可以協助您最好地制定適當提示的原則：

* **請使用清楚且明確的語言**：避免模糊且一般的提示，將可協助引導AI助理取得您嘗試收到的資料。
* **請包含時間範圍**：為物件指定AI助理特定時間範圍有助於縮小需要處理的資料範圍，並在回應中產生更多目標資訊。
* **一次只要求一件事**：當多個不相關的要求包含在單一提示中時，AI助理將無法提供正確的資訊。

如需有關建議提示的資訊，請參閱本文中的下列章節： [提示範例](#prompt-examples)。


### 驗證AI助理回應

在AI Assistant開發的這個階段，建議您在詢問Workfront程式的相關資訊時，驗證它所提供的資訊。 若要這麼做，請按一下提示回應中「來源」區段中提供的文章連結。

![來源區段](assets/sources-section.png)

如需Workfront程式提示的詳細資訊，請參閱本文中的[瞭解Workfront動作的提示](#prompts-to-learn-about-workfront-actions)。


## 提示範例

下表包含的提示範例可用來產生工作相關資訊，並深入瞭解您想要執行的特定Workfront流程或動作。

### 提示尋找有關您工作的資訊

<table>
    <tr>
        <td><b>物件類型</b></td>
        <td><b>提示</b></td>
    </tr>
        <tr>
        <td>專案</td>
        <td><em> [專案名稱]的到期日為何？</em>
        </td>
    </tr>
    <tr>
        <td>專案</td>
        <td><em> [專案名稱]的狀態為何？</em>
        </td>
    </tr>
    <tr>
        <td>專案 </td>
        <td><em>[專案名稱]的專案所有者是誰？</em></td>
    </tr>
    <tr>
        <td>任務</td>
        <td><em>本週指派給我的任務有哪些？</em></td>
    </tr>
       <tr>
        <td>問題 </td>
        <td><em>指派給我的團隊的未完成問題為何？</em></td>
           <tr>
        <td>使用者</td>
        <td><em>誰是[PROJECT NAME]的創意團隊？</em></td>
    </tr>
           <tr>
        <td>使用者 </td>
        <td><em>有多少任務指派給[USER]？</em></td>
    </tr>
   </table>


### 提示以瞭解Workfront動作

<table>
    <tr>
        <td><b>物件類型</b></td>
        <td><b>提示</b></td>
    </tr>
    <tr>
        <td>專案</td>
        <td><em>如何從範本建立新專案？</em>
        </td>
    </tr>
    <tr>
        <td>專案 </td>
        <td><em>專案和方案之間有何差異？</em></td>
    </tr>
    <tr>
        <td>任務</td>
        <td><em>如何將任務指派給多位使用者？</em></td>
    </tr>
       <tr>
        <td>任務</td>
        <td><em>「準備開始」狀態的意義是什麼？</em></td>
    </tr>
       <tr>
        <td>問題 </td>
        <td><em>如何將請求轉換為任務？</em></td>
    </tr>
           <tr>
        <td>問題 </td>
        <td><em>Workfront中問題的生命週期為何？</em></td>
    </tr>
        </tr>
           <tr>
        <td>問題 </td>
        <td><em>如何呈報請求？</em></td>
    </tr>
           <tr>
        <td>文件</td>
        <td><em>如何上傳檔案的新版本？</em></td>
    </tr>
           <tr>
        <td>文件 </td>
        <td><em>我可以設定檔案核准工作流程嗎？</em></td>
    </tr>
   </table>


## AI助理目前限制

AI Assistant是一款功能強大的工具，但在目前的開發階段，有某些型別的問題和請求無法提供資料。 下表包含AI助理無法顯示資料的提示範例。

<table>
    <tr>
        <td><b>提示型別</b></td>
        <td><b>範例</b></td>
    </tr>
    <tr>
        <td>關於自訂設定的問題</td>
        <td><em>在我們的Workfront執行個體中執行什麼自訂整合邏輯？</em>
        </td>
    </tr>
    <tr>
        <td>關於Workfront外部資料的問題 </td>
        <td><em>您可以顯示今天的Outlook行事曆嗎？</em></td>
    </tr>
             <tr>
        <td>有關未整合的Adobe產品的問題 </td>
        <td><em>如何從這裡編輯Acrobat中的PDF？</em></td>
         <tr>
        <td>需要人為判斷的問題</td>
        <td><em>此專案是否應暫停？</em></td>
    </tr>
    </tr>
       <tr>
        <td>要求大量更新</td>
        <td><em>重新指派[USER]的所有逾期工作。</em></td>
    </tr>
       <tr>
        <td>預測性分析的請求</td>
        <td><em>根據我們的歷史資料提出新的專案計畫。</em></td>
    </tr>
           <tr>
        <td>超過存取層級的資訊請求</td>
        <td><em>列出帳戶中的所有收費率。</em></td>
    </tr>
           <tr>
        <td>包含Vague資訊的請求 </td>
        <td><em>修正我的專案。</em></td>
    </tr>
   </table>
