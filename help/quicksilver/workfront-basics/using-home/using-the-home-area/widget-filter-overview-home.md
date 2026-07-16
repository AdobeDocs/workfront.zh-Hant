---
product-area: home
navigation-topic: new-home
title: 首頁Widget篩選器概觀
description: 您可以從多個Widget中進行選擇，以自訂首頁上顯示的內容。 這些Widget可以在首頁上調整大小和排列。
author: Courtney
feature: Get Started with Workfront
exl-id: 58f79e81-df6b-456f-9e91-4e00a1c2a8a2
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/1VkGz7LgrE1uBZ4uSwcTNLn3VpSMB-VI3o5HhpBG2XA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: d3382524-5489-431b-bde9-271ab257bc37
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9ef64f5a39c94426b2158c6504b913c8cb749c8e
workflow-type: tm+mt
source-wordcount: 881
ht-degree: 13%

---

# 首頁Widget篩選器概觀

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>
-->

您可以對下列Widget使用篩選器來尋找及組織工作：

* [我的專案](#my-projects)
* [我的任務](#my-tasks)
* [我的問題](#my-issues)
* [我的請求](#my-requests)
* [我的工作](#my-work)
* [我的核准](#my-approvals)

>[!IMPORTANT]
>
>* 若要在首頁Widget中顯示任務和問題，其父專案必須處於目前狀態或等於目前狀態。
>* 專案也必須處於目前狀態或等於目前狀態才能顯示。

## 我的專案

您可以在「我的專案」Widget中使用下列篩選器：

<table>
  <tr>
    <td>作用中</td>
    <td>以下列狀態顯示專案：目前、已計畫和已核准 </td>
  </tr>
  <tr>
    <td>有風險</td>
    <td>顯示處於風險狀態的專案 </td>
  </tr>
  <tr>
    <td>晚於排程</td>
    <td>顯示落後狀態的專案</td>
  </tr>
  <tr>
    <td>目前</td>
    <td>顯示目前狀態的專案 </td>
  </tr>
  <tr>
    <td>本月到期</td>
    <td>顯示計畫完成日期在目前日曆月內的專案</td>
  </tr>
  <tr>
    <td>遲到</td>
    <td>顯示處於延遲狀態的專案</td>
  </tr>
  <tr>
    <td>我的專案</td>
    <td>顯示指派給我或我的專案團隊處於目前狀態的專案</td>
  </tr>
  <tr>
    <td>準時</td>
    <td>顯示準時狀態的專案</td>
  </tr>
  <tr>
    <td>在成本預算之上</td>
    <td>顯示實際成本值大於其計畫成本值的專案</td>
  </tr>
  <tr>
    <td>在工作預算之上</td>
    <td>顯示實際所需工作值大於所需工作值的專案</td>
  </tr>
  <tr>
    <td>僅佇列</td>
    <td>顯示指定為請求佇列的專案</td>
  </tr>
  <tr>
    <td>已請求</td>
    <td>顯示處於請求狀態的專案</td>
  </tr>
  <tr>
    <td>案例規劃工具專案</td>
    <td>顯示透過「情境規劃工具」設定方案ID的專案</td>
  </tr>
</table>

## 我的任務

您可以在「我的任務」小工具中使用下列篩選器：

<table>
  <tr>
    <td>進行中的任務</td>
    <td><p>顯示沒有移交日期或移交日期為今天或更早的任務，並且</p>
<ul>
  <li>少於100%的完成百分比</li>
  <li>可開始值設為True</li>
</ul>
</td>
  </tr>
  <!--
    <tr>
    <td>All Unassigned Tasks</td>
    <td></td>
  </tr>
  -->
  <tr>
    <td>核准任務</td>
    <td>顯示處於未決核准狀態的任務</td>
  </tr>
  <tr>
    <td>可以開始</td>
    <td><p>顯示指派給我的任務</p>
<ul>
  <li>未處於等於完成的狀態</li>
  <li>Can Start值為true</li>
</ul>
</td>
  </tr>
  <tr>
    <td>關鍵路徑</td>
    <td>顯示指定為「關鍵」的任務</td>
  </tr>
  <tr>
    <td>未完成的任務</td>
    <td>顯示狀態設定為完成以外任何專案的任務</td>
  </tr>
  <tr>
    <td>里程碑任務</td>
    <td>顯示與里程碑關聯的任務。 如需詳細資訊，請參閱<a href="/help/quicksilver/manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">將里程碑與任務關聯</a>。
</td>
  </tr>
  <tr>
    <td>我的專案任務</td>
    <td>顯示目前狀態中的任務，其中我是專案團隊的成員 </td>
  </tr>
    <tr>
    <td>我的任務</td>
    <td>顯示指派給我的任務</td>
  </tr>
  <tr>
    <td>未指派給疊代</td>
    <td>顯示未指派給疊代的任務</td>
  </tr>
  <tr>
    <td>最近有趣的</td>
    <td><p>顯示上次更新是在過去兩週內的任務，並且</p>
<ul>
  <li>認可日期晚於計畫完成日期</li>
  或
  <li>專案期間大於計畫期間</li>
  或
  <li>狀況進展順利或有問題</li>
  或
  <li>主要任務受指派人已開始處理任務</li>
</ul>
</td>
  </tr>
  <tr>
    <td>我的角色中的未指派任務</td>
    <td><p>顯示符合以下條件的任務</p>
<ul>
  <li>指派給我的角色</li>
  <li>未完成</li>
</ul>
</td>
  </tr>
  <tr>
    <td>近期任務</td>
    <td><p>顯示符合以下條件的任務</p>
<ul>
  <li>不完整</li>
  <li>屬於處於目前狀態的專案</li>
  <li>計劃開始日期在今天日期後的兩週內</li>
</ul>
</td>
  </tr>
</table>

## 我的問題

您可以在「我的問題」Widget中使用下列篩選器：

<table>
<tr>
    <td>所有未指派</td>
    <td>顯示所有未指派且未附加解決物件的問題 </td>
  </tr>
  <tr>
    <td>指派給我</td>
    <td>顯示我是主要受指派人的問題</td>
  </tr>
  <tr>
    <td>完成</td>
    <td>顯示具有完成日期的問題 </td>
  </tr>
  <tr>
    <td>由我輸入</td>
    <td>顯示我輸入的問題</td>
  </tr>
  <tr>
    <td>我的專案問題</td>
    <td><p>顯示下列位置的問題</p>
<ul>
  <li>我是主要受指派人</li>
  <li>狀態為未完成</li>
  <li>沒有附加解析物件</li>
</ul>
</td>
  </tr>
    <tr>
    <td>我最近提交的問題</td>
    <td><p>顯示下列問題</p>
<ul>
  <li>我已提交</li>
  <li>沒有附加解析物件</li>
  <li>狀態不是「完成」且沒有「完成日期」</li>
  <li>在今天日期的三個月內提交</li>
</ul>
</td>
  </tr>
    </tr>
    <tr>
    <td>我已提交的問題</td>
    <td>顯示我擁有的問題</td>
  </tr>
  <tr>
    <td>開啟</td>
    <td>顯示沒有完成日期的問題</td>
  </tr>
  <tr>
    <td>可解決</td>
    <td>顯示已附加解析物件的問題</td>
  </tr>
  <tr>
    <td>我的角色中的未指派</td>
    <td>顯示所有未指派主要使用者但已指派角色的問題 </td>
  </tr>
</table>

## 我的請求

我的請求Widget具備可自訂的篩選器，可讓您控制哪些請求會出現在Widget中。 您可以為不同的欄位和值設定此篩選器，也可以使用AND和OR棧疊條件。

如需在「我的請求」Widget中設定篩選器的指示，請參閱「使用我的請求」Widget一文中的[篩選請求](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md#filter-requests)。

<!--
In the Production environment:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">All</td> 
      <td>Displays all submitted requests, regardless of status or who submitted them.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Open</td> 
      <td> <p>Displays all submitted requests 
      <ul>
      <li>That are currently open, regardless of who submitted them. Only requests you have at least permissions to view display here if you did not submit them yourself.</li>
      <li>Without an Actual Completion Date or whose resolving object does not have an Actual Completion Date are listed in the Open subtab.</li> 
      </ul>
      <p><b>NOTE</b> 
      Requests that are in any status that does not equate with Closed are considered open.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">My Requests</td> 
      <td>Displays requests you submitted regardless of their status. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">My Open Requests</td> 
      <td> <p>Displays requests 
      <ul>
      <li>That you submitted and are still open. </li> 
      <li>Without an Actual Completion Date or whose resolving object does not have an Actual Completion Date are listed in the My Open Requests subtab.  </li> 
      </ul>
      <p><b>NOTE</b> 
      Requests that are not in a status that equates with Closed are considered open.</p> </td> 
     </tr> 
    </tbody> 
   </table>



In the Preview environment:
-->

## 我的工作

您可以在「我的工作」Widget中使用下列篩選器：

<table>
  <tbody>
    <tr>
      <td>正在處理</td>
      <td>顯示您目前正在處理的專案</td>
    </tr>
    <tr>
      <td>已就緒可開始</td>
      <td>顯示專案與 
      <ul>
      <li>沒有未完成的前置任務或任務限制</li>
      <li>計劃開始日期是過去或未來最多兩週</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>尚未就緒</td>
      <td>顯示具有
       <ul>
      <li>未完成的前置任務或無法處理專案的任務限制</li>
      或
      <li>超過兩週的計劃開始日期</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>已請求</td>
      <td>顯示您尚未開始處理的問題</td>
    </tr>
    <tr>
      <td>由我委派</td>
      <td>顯示您已委派給其他使用者的專案</td>
    </tr>
    <tr>
      <td>已委派給我</td>
      <td>顯示使用者委派給您的專案</td>
    </tr>
    <tr>
      <td>已完成</td>
      <td>顯示過去兩週內完成的工作。 此篩選選項不包含核准。</td>
    </tr>
  </tbody>
</table>

## 我的核准

您可以在我的核准Widget中使用以下篩選器：

<table>
  <tbody>
    <tr>
      <td>已委派的核准</td>
      <td>顯示委派給您的核准</td>
    </tr>
    <tr>
      <td>我的核准</td>
      <td>顯示需要您核准的專案
      </td>
    </tr>
    <tr>
      <td>我已提交的核准</td>
      <td>顯示您已提交核准的專案
       </td>
    </tr>
  </tbody>
</table>
