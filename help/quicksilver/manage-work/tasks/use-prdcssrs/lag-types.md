---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 延遲型別概觀
description: 延遲是指在強制前置任務完成後必須經過的時間量，直到相依任務可以開始為止（正延遲），或是相依任務在前置任務開始之前可以開始的時間量（負延遲）。
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: a2d3032b32d321c0089839dafad6c9b3c5ba153a
workflow-type: tm+mt
source-wordcount: '1519'
ht-degree: 0%

---

# 延遲型別概觀

延遲是指前置任務計畫完成之後必須經過的時間量，直到相依任務可以開始（正延遲），或是相依任務在前置任務開始之前可以開始的時間量（負延遲）。

後續任務的「計畫」、「預計」和「預計」日期的計算會考慮前置任務的延遲和「計畫」、「預計」和「預計開始（完成）」日期。

## 存取需求

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務與專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務和專案的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 指示任務的延遲和延遲型別

當您定義前置任務關係時，可以在任務上指示延遲型別。

* [在任務的前置任務區段中指示延遲型別](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [指示工作清單中的延遲型別](#indicate-lag-types-in-a-task-list)

### 在任務的前置任務區段中指示延遲型別 {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. 移至您要定義前置任務與延遲型別的工作。
1. 按一下 **前置任務** 在左側面板中。 您可能需要按一下 **顯示更多**，然後 **前置任務**.
1. 按一下 **新增前置任務**.
1. （選用）如果要新增跨專案前置任務，請將 **父級專案** 名稱與另一個專案。
1. 開始輸入前置任務名稱，然後將其選取於清單中。
1. 選取 **相依性型別**.

   如需前置任務相依性型別的詳細資訊，請參閱 [作業相依性型別的概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. 指定 **延遲** 使用數值的金額。 您可以指定負數來指示負延遲。
1. 從下列選項中選取，以識別您要為前置任務指示的延遲型別：

   * **天**
   * **行事曆日**
   * **百分比**
   * **星期**
   * **星期（非零）**

     如需這些延遲型別及其計算方式的詳細資訊，請參閱區段 [延遲型別概觀](#lag-types-overview) 本文章內容。

1. 按一下&#x200B;**儲存**。

### 指示工作清單中的延遲型別  {#indicate-lag-types-in-a-task-list}

1. 前往工作清單，然後選取 **標準** 從檢視 **檢視** 下拉式功能表。

1. 按一下 **前置任務** 與您要為其指定前置任務和延遲量的任務對應的欄。
1. 輸入以下內容（不含空格）：

   * 要指定為所選任務的前置任務之任務編號
   * 您要在工作之間指示的相依性型別的縮寫

     如需有關「相依性型別」縮寫的詳細資訊，請參閱 [作業相依性型別的概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * 或a **+** 正延遲或 **-** 若為負延遲

   * 延遲的金額
   * 您要使用的Lag Type縮寫。

     如需Lag型別縮寫的詳細資訊，請參閱區段 [延遲型別概觀](#lag-types-overview) 本文章內容。

   例如，若要指出某個任務具有前置任務且延遲為2天，您可以輸入  `1fs+2d` 在「前置任務」欄中。

1. 按一下鍵盤上的Enter以儲存對您工作的變更。

## 延遲型別概觀 {#lag-types-overview}

需要延遲時間的作業範例可能是將樹木切割成木材。 如果剛剪下的木頭必須乾燥一段時間才能剪下，那麼剪下樹木和鋸成木頭之間就會有時間延遲。

下表說明「延遲型別」，以及如何指出每個延遲型別的時間長度：

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>值</strong> </p> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>天數（d或de）</p> </td> 
   <td> <p>透過相依性連結的兩個任務之間的延遲是以工作日測量。 這是預設的延遲型別。 </p> <p>例如，如果有延遲了2個工作天的完成 — 開始相依性，而前置任務在星期五完成，則相依任務會在星期三開始。 週末天數不會計入延遲中。 </p> <p>注意：延遲天數的上限為366天。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>行事曆日（c或ce）</p> </td> 
   <td> <p>兩個工作之間的延遲是以日曆日計算，包括假日和週末。 </p> <p>注意：雖然此延遲型別會將非工作日計為延遲的一部分，但相依任務絕對不能在非工作日開始。 如果此延遲型別使相依任務在非工作日開始，則相依任務的計劃開始日期會排定在下一個工作日。 </p> <p>例如，如果具有2個日曆天延遲的完成 — 開始相依性，且前置任務在星期四完成，則相依任務會在星期一開始，而不是星期日。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>百分比（p或pe）</p> </td> 
   <td> <p>延遲以預估完成前置任務所需時間的百分比表示。 </p> <p>例如，如果在10天的前置任務上有20%的延遲的完成 — 開始相依性，則系統會計算多少天代表前置任務任務的20%工期，並作為延遲使用。 在這種情況下，它將在任務完成後2天。 </p>

<p><b>附註</b></p> 百分比的最大延遲限製為2000%。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>星期（w或we） </p> </td> 
   <td> <p>兩個任務之間的延遲的度量方式為指出包含前置任務計畫完成日期的一週中某天。</p> <p>對於這種「延遲型別」，一週中的每一天都與一個數字相關聯：</p> 
    <ul> 
     <li>星期日=1</li> 
     <li>星期一=2</li> 
     <li>星期二=3</li> 
     <li>星期三=4</li> 
     <li>星期四=5</li> 
     <li>星期五=6</li> 
     <li>星期六=7</li> 
    </ul> <p>如果您想要指出後續任務的「計劃開始日期」應為本週的星期二，且星期二在前身任務的計畫完成日期之前，請使用下列公式來編碼後續任務： </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>附註</b></p>

如果後續任務的「開始日期」計算為某一星期二，而本週的該日已過，則後續任務的「計劃開始日期」為下一週的同一天（星期二） （如果有的話）。 </p> <p>如果您想要指出延遲應落在本週的星期六，而星期六在前置任務的計畫完成日期之後，您可以使用下列公式來編碼您的後置任務：</p> <p><code>4fs+7w</code> </p> <p>如果星期六是非工作日，則會選取星期六之後的下一個可用日（表示正延遲）作為後續任務的計劃開始日期。 </p>

<p>這不適用於排程例外狀況。 如果日期也是排程例外，且後續任務的「開始日期」被計算為當天，則系統會嘗試尋找最近的可用日期，也就是前置任務運算式中所指定的星期幾。</p>

<p>例如，如果「開始日期」計算為某個星期二，而該日為排程例外，且前置任務的延遲為正數，則它會選擇下列星期二（如果這也是工作日）作為後續任務的開始日期。 如果延遲為負數，則系統會選擇前一個星期二作為開始日期。</p>

<p>若要指示過去或未來的周數，您可以在延遲型別的天數字前新增一個數字。 </p> <p>例如，若要指定10週前的星期一，您可以使用此程式碼來指定您的繼任者的前置任務：</p> <p><code>4fs-102w</code> </p> <p>10表示10週前，2是指派給星期一的數字。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>星期幾（k或ke）</p> </td> 
   <td> <p>兩個任務之間的延遲度量方式與一週延遲型別的「天」相同，但如果前置任務的時間在指定一週的同一天結束，則不在此限。 接著會計算相鄰一週的延遲時間(+/-)。 </p> <p>在此情況下，延遲時間絕不能為0。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 負數延遲概觀

您可以使用負延遲來指示任務需要或能夠在前置任務結束之前開始。

使用負數延遲時，請考量下列規則：

* 負延遲無法強制任務的開始/完成日期早於或晚於專案的計劃開始/完成日期。 這些日期是在專案的「排程起始日期」欄位中指定的。

  在此情況下，請考慮下列事項：

   * 從完成日期排程專案。
   * 專案上的最後一個任務應使用「必須在任務限制上完成」。 建議給予任務足夠長的工期，以便考慮專案上的所有任務。 剩餘的任務可與「儘快」限制搭配使用。

* 將前置任務的「完成 — 開始」關係用於任務可能會產生錯誤訊息。

  在此情況下，請考慮下列事項：

   * 設定任務之間的「完成 — 完成」前置任務關係。
   * 後續任務的持續時間應等於或超過任務之間的預期延遲天數。
