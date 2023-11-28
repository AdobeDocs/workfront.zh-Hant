---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: 新的評論體驗
description: Adobe Workfront中的評論體驗更新目前正在開發中。 此更新包含新介面、新功能，以及所選物件「更新」區段的改進效能。
author: Alina
feature: Product Announcements
role: User
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: c3abb5dce14c0b19ab2e5b82f159cd29f80f79e4
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 3%

---

# 新的評論體驗


<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。  </span>

<span class="preview">如需目前發行排程的詳細資訊，請參閱 [2024年第一季版本總覽](../../product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

<!--

After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  -->

>[!IMPORTANT]
>
>本文資訊是指已發行給新評論體驗的功能。
>
>新評論體驗的Beta版計畫從2023年4月開始，到2023年10月結束。 新評論體驗的Beta版計畫已於2023年10月版本中結束。
>
>本文所述功能已於2023年10月向所有客戶發佈，除非另有說明。

<!--An update to the commenting experience in Adobe Workfront is currently in development. This update includes a new interface, new features, and improved performance in the Updates section of select objects. 

The new commenting experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.-->

<!--For additional resources for the new commenting experience, also see the following articles:

* [New commenting experience release activity](../new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md)
* [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md)
-->

## 功能

新的評論體驗包括改進和變更Adobe Workfront物件的更新區段。

新註解體驗中包括的改善包括：

* 改善的效能和使用者體驗
* 將使用者評論和系統活動更新分開
* 將新註解新增至物件時的即時指示器
* 在提交評論後進行編輯

下列功能已從新體驗中移除：

* 系統更新的註解
* 可在註解時編輯狀態、條件、認可日期
* 編輯自訂表單
* 當Workfront或群組管理員以其他使用者身份登入並代表他們新增評論時，「代表&lt;使用者名稱>」資訊最初被移除。 它已於2023年10月19日恢復。
* 當您在檔案中新增註解時標籤人員的「要求核准」選項。

<!--removed this note on November 28, 2023, when this limitation was removed: 

>[!NOTE]
>
>The objects listed below have only the comments and system updates starting with January 1, 2019 available in the new commenting experience.  
>
>You can view comments and system updates on these objects prior to January 1, 2019 when viewing the Updates section in the current experience:
>
>* Issues
>* Projects
>* Tasks
>* Documents

For more information, see the [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md). 
-->

下表說明新評論體驗中可用的功能，及其在支援區域中的可用性：

<table>
  <tr>
   <td><strong>功能 </strong>
   </td>
   <td><strong>存在於舊評論體驗中 </strong>
   </td>
   <td><strong>存在於新的評論體驗中 </strong>
   </td>
   <td><strong>將在新的評論體驗中引入 </strong>
   </td>
   <td><strong>何時會引進到新的註解體驗 </strong>
   </td>
   <td><strong>研究中 </strong>
   </td>
  </tr>
  <tr>
   <td>建立/讀取/回覆/刪除註解 
   </td>
   <td>✓ (A) 
  </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>RTF文字（不包括引號和emoji）
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>RTF文字（表情符號）
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>RTF文字（區塊引號）
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 2023年第2季
   </td>
   <td> 
   </td>
  </tr>
  <tr>
<tr>
   <td> 報價註解
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 2023年第2季
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>對評論做出反應（類似） 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>將影像附加至註解 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>在評論中標籤人員 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>移除執行緒參與者
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>


<tr>
   <td>自動標籤所有執行緒參與者
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>公司私有的評論 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>還原評論的張貼 
   </td>
   <td>✓ 
   </td>
   <td>已取代為編輯註解 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>關閉系統更新 
   </td>
   <td>✓ 
   </td>
   <td>已取代為活動索引標籤 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>編輯評論 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>離開頁面時儲存註解草稿 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>即時檢視新註解（包括刪除註解時檢視）
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>記錄時間 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>複製對話連結 
   </td>
   <td>✓ 
   </td>
   <td> 已取代為複製連結
   </td>
   <td> 
   </td>
   <td>2023年第2季 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>複製評論連結 
   </td>
   <td>✓ 
   </td>
   <td> 已取代為複製連結
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>報價註解文字 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td>2023年第2季 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>複製本文 
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>在評論中搜尋 
   </td>
   <td> 
   </td>
   <td> <span class="preview">✓</span>
   </td>
   <td> 
   </td>
   <td>2024年第1季度 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>在註解中複製並貼上影像
   </td>
   <td> 
   </td>
   <td> <span class="preview">✓</span>
   </td>
   <td> 
   </td>
   <td>2024年第1季度 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>在註解中拖放影像
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>2024年第1季度 
   </td>
   <td>✓ 
   </td>
  </tr>

<tr>
   <td>編輯自訂表單 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>可在註解時編輯狀態、條件、認可日期 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
  </tr>
<tr>
   <td>回覆系統更新 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
<tr>
   <td>新增以其他使用者身分登入的評論時顯示「代表」
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
</table>

## 發行時間表

有關最近發行給新評論體驗的功能以及發行時間表的資訊，請參閱 [新的評論Beta版體驗發行活動](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).

如需管理Workfront物件更新的詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## 找出新的註解體驗

&lt;! — 重要：我們移除舊版體驗時，請將此項的版本移至「更新」工作文章或「更新」區段總覽 — 表示除了版序之外，其他所有項的體驗都不同 — >

新的評論體驗目前適用於所有客戶和環境。

根據您存取註釋體驗的物件，您可能會在「更新」區段中看到下列功能：

* 下列物件的新舊註解體驗：

   * 專案
   * 工作（包括劇本）
   * 問題
   * 文件

  >[!TIP]
  >
  >使用新註解選項來顯示新的註解體驗（當您啟用時）或舊版註解體驗（當您停用時），如本節所述。 預設為新的註解體驗。

   * 僅限下列物件的新註解體驗。 沒有選項可啟用這些物件的舊版註解體驗：

      * 目標

     >[!NOTE]
     >
     >您必須額外取得Adobe Workfront目標授權才能存取此Workfront區域。 如需詳細資訊，請參閱 [使用Workfront目標的需求](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
      * 展示板上的卡片
      * 團隊
      * 範本
      * 範本任務
      * 時程表
      * 方案
      * 專案組合
      * 使用者

* 僅限下列物件的舊版註解體驗：

   * 疊代

     沒有選項可啟用反複專案的新註解體驗。 只有舊版註解體驗可用於反複專案。


<!--before August 17: 

The new commenting experience is currently supported for the following objects:


* When enabling the Beta experience in the Updates section for 

    * Issues, projects, tasks, and documents

    For more information about managing updates for Workfront objects, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

* By default, as the only commenting experience for

    * Goals, cards on a board

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

-->

<!--Depending on the environment you access the commenting experience you can do one of the following: 

* Enable the commenting experience Beta in the Production environment
* <span class="preview">Enable the legacy commenting experience in the Preview  environment </span>
-->

若要啟用專案、任務、問題和檔案的評論體驗選項：

1. 移至您要為其啟動新註解體驗的物件，然後按一下 **更新** 在左側面板中。
1. （視條件而定）如果已停用，請啟用 **新增註解** 「更新」區域右上角的選項以啟用它。 預設應該啟用此功能。

   ![](assets/new-commenting-toggle-off-highlighted.png)

1. 開始在 **註解** 標籤。 「註解」標籤是新體驗開啟時的預設標籤

   或

   按一下  **系統活動** 索引標籤以檢視Workfront產生的活動更新。

1. （可選）若要停用新的註解體驗並返回舊版註解，請取消選取 **新增註解** 選項。

