---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 系統項目狀態
description: Workfront有9個內建系統專案狀態。 下表中的前3個是必要項，這表示您可以解除鎖定、重新命名和重新排序，但無法隱藏或刪除它們。 變更專案狀態通常是手動處理。 不過，有時專案狀態會自動變更，端視系統中發生的其他因素而定。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# 系統項目狀態

Workfront有9個內建系統專案狀態。

下表中的前3個是必要項，這表示您可以解除鎖定、重新命名和重新排序，但無法隱藏或刪除它們。

變更專案狀態通常是手動處理。 不過，根據系統中發生的其他因素，當專案狀態自動變更時，以下清單中會列出一些案例。

您的Workfront執行個體會提供下列專案狀態：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>系統項目狀態</th> 
   <th>當</th> 
   <th>此狀態中會發生什麼</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計畫（必需狀態）</td> 
   <td> <p>項目經理正在規劃項目的時間表、任務分配和批准。 項目經理在項目上手動設定此狀態。</p> <p>提示：建議您將Workfront中新專案的預設狀態設為「規劃」。 作為Workfront管理員，您可以在「項目首選項」的「項目」區域中更改所有新項目的預設狀態。</p> </td> 
   <td> <p>依預設，專案團隊的使用者可以在Workfront的「專案」區域中，查看其「專案」清單中的專案。 項目上分配給它們的任務和問題不會填入其工作清單。 「首頁工作清單」中只顯示批准和接受的工作項。</p> <p>專案處於此狀態時不會傳送任何通知。</p> <p>我們建議在項目處於「計畫」狀態時進行所有可觸發對項目時間軸的更新的更改，或對任務和問題分配的任何更改。 這將用戶收到的通知量降至最低。</p> <p>系統不會自動計算項目的時間軸。</p> </td> 
  </tr> 
  <tr> 
   <td>當前（必需狀態）</td> 
   <td> <p>使用者正在操作。 專案經理應將專案轉換為「目前」，以指出已開始。</p> <p>這是Workfront中新專案的預設狀態。</p> <p>提示：作為Workfront管理員，您可以在「項目首選項」的「項目」區域中更改新項目的預設狀態。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>.</p> </td> 
   <td> <p>依預設，專案團隊的使用者可以在Workfront的「專案」區域中，查看其「專案」清單中的專案。 專案上指派給他們的工作和問題會填入其「工作清單」。 他們可以開始接受有關任務和問題的工作，並將其移至「工作內容」清單。</p> <p>此外，在「當前」項目上，所有有關時間軸更改、分配、所需操作和批准的通知都將發送給項目團隊中的用戶。</p> <p>如果項目的「更新類型」設定為「自動」、「更改時」或「自動」和「更改時」，則系統會自動計算項目的時間軸。</p> <p>提示：最好在項目處於此狀態時，將項目計畫調整量保持在最低，這樣用戶就不會收到太多通知。</p> </td> 
  </tr> 
  <tr> 
   <td>完成（必要狀態）</td> 
   <td> <p> 項目已完成：</p> 
    <ul> 
     <li> <p>如果項目的「完成模式」設定為「手動」，項目經理將手動選擇此狀態，以通知項目團隊的用戶停止處理項目。</p> </li> 
    </ul> 
    <ul> 
     <li>如果項目的「完成模式」設定為「自動」，則當項目中的所有任務和問題都標籤為「完成」時，Workfront會自動將項目標籤為「完成」。 </li> 
    </ul> <p><b>重要</b>:只有在項目上的所有任務、問題和批准都已解決後，才能將項目標籤為已完成。</p> </td> 
   <td>
    <ul>
     <li>依預設，專案團隊的使用者無法在其Workfront的「專案」區域中的「專案」清單上看見專案。 項目上分配給它們的任務和問題不會填入其「工作請求」或「正在處理」清單。</li>
     <li>與專案相關的所有通知（狀態變更通知除外）停止傳送給專案團隊的使用者。 </li>
     <li>系統不再計算項目的時間軸。</li>
     <li>無法複製項目。</li>
    </ul><p>當專案標示為「完成」時，您可以防止使用者執行其他動作。 </p><p>有關如何限制標籤為「完成」的項目上的操作的詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>.</p></td> 
  </tr> 
  <tr> 
   <td>廢棄</td> 
   <td>該項目尚未完成，但由於設定障礙或範圍改變，該項目無法繼續進行並已被放棄。 項目經理將狀態更改為「無效」(Dead)，以提醒項目團隊中的用戶此項目將永遠無法完成，並且他們不應再繼續使用該項目。</td> 
   <td> <p>依預設，專案團隊的使用者無法在其Workfront的「專案」區域中的「專案」清單上看見專案。 項目上分配給它們的任務和問題將從其「工作清單」中消失。</p> <p>不能向任務或問題授予批准決定。</p> <p>不會將時間軸變更、工作分配、所需動作、核准的相關通知傳送給專案團隊的使用者。</p> <p>系統不會自動計算項目的時間表，因為項目被認為已完成。</p> <p>當專案標示為「無效」時，您可以防止使用者執行特定動作。 如需如何限制無效專案上動作的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>保留</td> 
   <td>項目尚未完成，但由於一些延誤，項目需要暫時暫停。 項目經理選擇使用此狀態來提醒項目團隊中的用戶在當前時間停止處理項目。</td> 
   <td> <p>依預設，專案團隊的使用者無法在其Workfront的「專案」區域中的「專案」清單上看見專案。 項目上分配給它們的任務和問題將從其「工作清單」中消失。 </p> <p>不能向任務或問題授予批准決定。</p> <p>不會將時間軸變更、工作分配、所需動作、核准的相關通知傳送給專案團隊的使用者。</p> <p> <p><b>注意</b>:將項目置於「暫掛」狀態時，項目時間軸不會停止。 即使沒有人在積極處理項目，項目仍可顯示為「有風險」或「有麻煩」。 當將項目重新調回「當前」狀態時，可能需要手動調整剩餘未結任務的日期，以便項目可以顯示更新的進度。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>已請求</td> 
   <td>當項目請求的業務案例已完成並提交審批時，系統會自動將項目狀態標籤為「請求」。 如需使用商業案例請求專案的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">審查請求的項目</a>.</td> 
   <td> <p>依預設，專案團隊的使用者無法在其Workfront的「專案」區域中的「專案」清單上看見專案。 分配給它們的項目上的任務和問題不會填充其「工作清單」。</p> <p>除了狀態變更通知之外，與專案相關的所有通知都不會傳送給任何使用者。</p> <p>系統不會自動計算項目的時間軸。</p> </td> 
  </tr> 
  <tr> 
   <td>已核准</td> 
   <td>當項目請求的業務案例獲得批准時，項目狀態會自動標籤為「已批准」。 如需使用商業案例請求專案的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">審查請求的項目</a>.</td> 
   <td> <p>依預設，專案團隊的使用者可以在Workfront的「專案」區域中，查看其「專案」清單中的專案。 項目上分配給它們的任務和問題不會填入其工作清單。</p> <p>除了狀態變更通知之外，與專案相關的所有通知都不會傳送給任何使用者。</p> <p>系統不會自動計算項目的時間軸。 </p> </td> 
  </tr> 
  <tr> 
   <td>已拒絕</td> 
   <td>當項目請求上的業務案例被拒絕時，項目狀態會自動標籤為「已拒絕」。 如需使用商業案例請求專案的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">審查請求的項目</a>.</td> 
   <td> <p>依預設，專案團隊的使用者無法在其Workfront的「專案」區域中的「專案」清單上看見專案。 項目上分配給它們的任務和問題不會填入其工作清單。</p> <p>除了狀態變更通知之外，與專案相關的所有通知都不會傳送給任何使用者。</p> <p>系統不會自動計算項目的時間軸。</p> </td> 
  </tr> 
  <tr> 
   <td>構想</td> 
   <td>當您提交專案請求時，專案狀態會自動標示為「構想」。 如需使用商業案例請求專案的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">審查請求的項目</a>.</td> 
   <td> <p>依預設，專案團隊的使用者無法在其Workfront的「專案」區域中的「專案」清單上看見專案。 項目上分配給它們的任務和問題不會填入其工作清單。</p> <p>除了狀態變更通知之外，與專案相關的所有通知都不會傳送給任何使用者。</p> <p>系統不會自動計算項目的時間軸。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>以下項目狀態不能更改為「無效」、「暫掛」或「完成」狀態：
>
>* 已請求
>* 構想
>* 已核准
>* 已拒絕（或相等）
>

