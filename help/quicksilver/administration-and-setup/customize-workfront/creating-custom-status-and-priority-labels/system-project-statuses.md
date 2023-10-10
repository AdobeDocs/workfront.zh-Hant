---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 系統專案狀態
description: Workfront有9個內建的系統專案狀態。 下表中的前3項為必要項，表示您可以解除鎖定、重新命名及重新排序，但無法隱藏或刪除它們。 變更專案狀態通常是手動過程。 但是，有時專案狀態會自動變更，具體取決於系統中發生的其他因素。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '1572'
ht-degree: 0%

---

# 系統專案狀態

Workfront有9個內建的系統專案狀態。

下表中的前3項為必要項，表示您可以解除鎖定、重新命名及重新排序，但無法隱藏或刪除它們。

變更專案狀態通常是手動過程。 不過，當專案狀態根據系統中發生的其他因素自動變更時，有些案例會列在以下清單中。

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
   <th>系統專案狀態</th> 
   <th>此專案狀態發生於</th> 
   <th>此狀態中會發生什麼事</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planning （必要狀態）</td> 
   <td> <p>專案經理正在規劃專案的時間表、任務指派及核准。 專案經理在專案上手動設定此狀態。</p> <p><b>秘訣</p> <p> 建議您在Workfront中為新專案設定預設狀態至Planning。 身為Workfront管理員，您可以在「專案偏好設定」的「專案」區域中變更所有新專案的預設狀態。</p> </td> 
   <td> <p>專案團隊中的使用者可以在Workfront的「專案」區域中，依預設在其專案清單中檢視專案（沒有自訂篩選器）。 在專案中指派給他們的任務和問題未填入其工作清單。 首頁工作清單中僅顯示核准和接受的工作專案。</p> <p>專案處於此狀態時不會傳送任何通知。</p> <p>我們建議所有可能觸發專案時間表更新的變更，或對任務和問題指派的任何變更，在專案處於「計畫」狀態時進行。 這會將使用者收到的通知數量減到最少。</p> <p>系統不會自動計算專案的時間表。</p> </td> 
  </tr> 
  <tr> 
   <td>目前（必要狀態）</td> 
   <td> <p>使用者正在處理。 專案經理應將專案轉換為目前狀態，以表示專案已開始。</p> <p>這是Workfront中新專案的預設狀態。</p> <p><b>秘訣</b></p>

<p> 身為Workfront管理員，您可以在「專案偏好設定」的「專案」區域中變更新專案的預設狀態。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>.</p> </td> 
   <td> <p>專案團隊中的使用者可以在Workfront的「專案」區域中，依預設在其專案清單中檢視專案（沒有自訂篩選器）。 在專案中指派給他們的任務和問題會填入其工作清單。 他們可以開始接受任務和問題的工作，並將他們移至其工作清單。</p> <p>此外，在「目前」專案中，所有關於時間表變更、指派、所需動作和核准的通知，都會傳送給專案團隊的使用者。</p> <p>如果專案的「更新型別」設定為「自動」、「變更時」或「自動與變更時」，則系統會自動計算專案的時間表。</p> <p>提示：當專案處於此狀態時，最好將專案計畫調整保持在最低程度，這樣使用者不會收到太多通知。</p> </td> 
  </tr> 
  <tr> 
   <td>完成（必要狀態）</td> 
   <td> <p> 專案已完成：</p> 
     <p>如果專案的「完成模式」設定為「手動」，專案經理會手動選擇此狀態，以通知專案團隊的使用者停止處理專案。</p> 
    <p>如果專案的「完成模式」設定為「自動」，當專案中的所有任務和問題都標示為「完成」時，Workfront會自動將專案標籤為「完成」。 
    <p><b>重要</b> </p>
    <p>只有當專案上的所有任務、問題和核准都已解決時，您才能將專案標籤為完成。</p> </td> 
   <td>
    <p>專案團隊的使用者預設無法在Workfront的專案區域的專案清單中看到專案（沒有自訂篩選器）。 在專案中指派給他們的任務和問題不會填入其「工作請求」或「正在處理」清單。 </p>
    <p>除了狀態變更通知之外，所有與專案相關的通知都會停止傳送給專案團隊的使用者。</p>
    <p>系統不再計算專案的時間表。 </p>
    <p>無法複製專案。</p>
    <p>當專案標籤為完成時，您可以防止使用者執行其他動作。 </p><p>如需有關如何限制標示為完成的專案之動作的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>.</p></td> 
  </tr> 
  <tr> 
   <td>廢棄</td> 
   <td>專案尚未完成，但由於路障或範圍變更，專案無法繼續運作且已放棄。 專案經理會將狀態變更為廢棄，以提醒專案團隊中的使用者，此專案將永遠不會完成，且他們不會再處理此專案。</td> 
   <td> <p>專案團隊的使用者預設無法在Workfront的專案區域的專案清單中看到專案（沒有自訂篩選器）。 在專案中指派給他們的任務和問題從他們的工作清單中消失。</p> <p>無法將核准決定授予任務或問題。</p> <p>不會將有關時間表變更、指派、所需動作和核准的通知傳送給專案團隊中的使用者。</p> <p>系統不會自動計算專案的時間表，因為系統會將專案視為已完成。</p> <p>當專案被標籤為廢棄時，您可以防止使用者執行某些動作。 如需有關如何限制已廢棄專案之動作的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>保留</td> 
   <td>專案尚未完成，但由於一些延遲，專案需要暫時暫停。 專案經理選擇使用此狀態來提醒專案團隊中的使用者在目前時間停止處理專案。</td> 
   <td> <p>專案團隊的使用者預設無法在Workfront的專案區域的專案清單中看到專案（沒有自訂篩選器）。 在專案中指派給他們的任務和問題從他們的工作清單中消失。 </p> <p>無法將核准決定授予任務或問題。</p> <p>不會將有關時間表變更、指派、所需動作和核准的通知傳送給專案團隊中的使用者。</p> <p> <p><b>注意</b>：當您擱置專案時，專案的時間表未停止。 即使目前沒有任何人在處理此專案，此專案仍會顯示為「有風險」或「存在問題」。 再次將專案切換回「目前」時，可能需要手動調整剩餘未完成任務的日期，以便專案可以顯示更新的進度。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>請求日期</td> 
   <td>當專案請求的業務案例完成並提交核準時，系統會自動將專案狀態標示為「已請求」。 如需使用業務案例請求專案的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">檢閱請求的專案</a>.</td> 
   <td> <p>專案團隊的使用者預設無法在Workfront的專案區域的專案清單中看到專案（沒有自訂篩選器）。 指派給他們的專案上的任務和問題未填入其工作清單。</p> <p>除了狀態變更通知之外，所有與專案相關的通知都不會傳送給任何使用者。</p> <p>系統不會自動計算專案的時間表。</p> </td> 
  </tr> 
  <tr> 
   <td>已核准</td> 
   <td>當專案請求中的業務案例獲得核準時，專案狀態會自動標示為「已核准」。 如需使用業務案例請求專案的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">檢閱請求的專案</a>.</td> 
   <td> <p>專案團隊中的使用者可以在Workfront的「專案」區域中，依預設在其專案清單中檢視專案（沒有自訂篩選器）。 在專案中指派給他們的任務和問題未填入其工作清單。</p> <p>除了狀態變更通知之外，所有與專案相關的通知都不會傳送給任何使用者。</p> <p>系統不會自動計算專案的時間表。 </p> </td> 
  </tr> 
  <tr> 
   <td>已拒絕</td> 
   <td>當專案請求的業務案例被拒絕時，專案狀態會自動標示為「已拒絕」。 如需使用業務案例請求專案的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">檢閱請求的專案</a>.</td> 
   <td> <p>專案團隊的使用者預設無法在Workfront的專案區域的專案清單中看到專案（沒有自訂篩選器）。 在專案中指派給他們的任務和問題未填入其工作清單。</p> <p>除了狀態變更通知之外，所有與專案相關的通知都不會傳送給任何使用者。</p> <p>系統不會自動計算專案的時間表。</p> </td> 
  </tr> 
  <tr> 
   <td>構想</td> 
   <td>當您提交專案請求時，專案狀態會自動標示為「構想」。 如需使用業務案例請求專案的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">檢閱請求的專案</a>.</td> 
   <td> <p>專案團隊的使用者預設無法在Workfront的專案區域的專案清單中看到專案（沒有自訂篩選器）。 在專案中指派給他們的任務和問題未填入其工作清單。</p> <p>除了狀態變更通知之外，所有與專案相關的通知都不會傳送給任何使用者。</p> <p>系統不會自動計算專案的時間表。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>下列專案狀態無法變更為「廢棄」、「保留」或「完成」狀態：
>
>* 請求日期
>* 構想
>* 已核准
>* 已拒絕（或其同等專案）
>
