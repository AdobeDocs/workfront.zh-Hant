---
content-type: reference
navigation-topic: notifications
title: 通知：關於我所在專案的資訊
description: 下列通知會提醒您正在處理的專案中發生活動。
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 0%

---

# 通知：關於我所在專案的資訊

下列通知會提醒您正在處理的專案中發生活動。

如需有關設定您收到哪些通知的資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

另請參閱[事件通知](../../workfront-basics/using-notifications/event-notifications.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>包含的欄位 </p> <p> *僅每日摘要欄位</p> </th> 
   <th>預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>向我所在的專案新增一個檔案</strong> </p> <p>將檔案新增至專案時，專案團隊成員會收到電子郵件通知，但新增檔案的使用者除外。</p> <p>只有在專案狀態為[！UICONTROL目前]且檔案不是「私人」時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是<em>[！UICONTROL檔案已新增到] &lt;專案名稱&gt;</em></p> <p>每日摘要通知的主題為您所在專案的<em>[！UICONTROL摘要] &lt;每日摘要日期&gt;</em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>檔案參考編號<br>新增檔案的使用者名稱<br>檔名稱<br>已於日期新增<br>檔案詳細資訊（格式、大小、版本編號）<br>檔案縮圖<br><strong>[！UICONTROL預覽]</strong>和<strong>[！UICONTROL下載]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*新增的檔案總數<br>*檔名稱<br>*上傳文檔的使用者的名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我所在的專案上完成了里程碑任務</strong> </p> <p>專案團隊的成員會在專案上的里程碑任務完成時收到通知。 完成個人任務時不會傳送通知。</p> <p>只有在專案狀態為[！UICONTROL目前]或[！UICONTROL規劃]時，才會傳送通知。</p> <p>主旨列是<em>[！UICONTROL完成]： &lt;專案名稱&gt;</em>上的&lt;任務名稱&gt;</p> <p>每日摘要通知的主題是<em> [！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt;</em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>完成任務的使用者名稱<br>任務狀態<br>完成任務的日期和時間<br>先前的任務狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*完成的任務總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要的日期<br></td> 
   <td><strong>[！UICONTROL每日]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我參與的一個專案變為使用中</strong> </p> <p>專案狀態設為[！UICONTROL目前]時，專案團隊成員會收到電子郵件通知。</p> <p>注意：當專案狀態設為[！UICONTROL目前]時，使用者必須列在專案的「人員配備」標籤上才能收到通知。 如需將使用者新增至專案團隊的詳細資訊，請參閱<a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">管理專案團隊</a>。</p> <p>即時通知電子郵件的主旨為<em>&lt;專案名稱&gt; [！UICONTROL為最新 — 移至您的專案並檢視您的工作！]</em></p> <p> 每日摘要通知的主題是<em> [！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>專案參考編號<br>專案狀態<br>專案[！UICONTROL計畫完成日期]<br>專案所有者<br>指派給您、您的其中一個工作角色或其中一個團隊的任務清單<br><strong>[！UICONTROL檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*專案狀態<br>*每日摘要日期</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>我的團隊所在的一個專案變為使用中</strong> <p>專案生效時，團隊成員會收到電子郵件通知。 必須將團隊指派給至少一個任務以接收通知。</p><p>如果個別使用者和團隊都被指派給專案上的任務。 團隊將不會收到通知。</p><p>即時通知電子郵件的主旨為<i>&lt;專案名稱&gt; [！UICONTROL作用中 — 移至您的專案並檢視您的工作！]</i></p><p>每日摘要通知的主題是<em> [！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt; </em></p></td> 
   <td>專案名稱<br>Portfolio名稱<br>專案參考編號<br>專案狀態<br>專案[！UICONTROL計畫完成日期]<br>專案所有者<br>指派給團隊的任務清單<br><strong>[！UICONTROL檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*專案狀態<br>*每日摘要日期</td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我所在的專案已完成</strong> </p> <p>專案狀態為[！UICONTROL完成]時，專案團隊成員會收到電子郵件通知。</p> <p>提示：如果專案定期完成，則啟用此選項可以為許多專案中任務數量有限的使用者建立許多電子郵件。</p> <p>即時通知電子郵件的主旨是<em>[！UICONTROL專案狀態變更]： &lt;專案名稱&gt;</em></p> <p> 每日摘要通知的主題是<em> [！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>專案參考編號<br>完成專案的使用者名稱<br>專案狀態<br>專案完成的日期和時間<br>先前的專案狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*專案狀態<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我所在的專案上完成了一項任務</strong> </p> <p>專案團隊的成員會在專案上完成任務時收到電子郵件通知。 <br>如需專案團隊的詳細資訊，請參閱<a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概述</a>。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是<em>[！UICONTROL完成]： &lt;專案名稱&gt;</em>上的&lt;任務名稱&gt;</p> <p> <p>注意：如果任務變更為等於[！UICONTROL完成]的狀態，則電子郵件主旨仍會顯示「[！UICONTROL完成]」。</p> </p> <p><em>每日摘要通知的主題為：[！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt; </em> </p> </td> 
   <td> <p>任務名稱<br>專案名稱<br>任務參考編號<br>完成任務的使用者名稱<br>任務狀態<br>任務狀態變更的日期和時間<br>先前的任務狀態<br><strong>檢視更多詳細資料</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*完成的任務總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要的日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我所在的專案新增了一個問題</strong> </p> <p>將問題新增至專案時，專案團隊成員會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是<em>[！UICONTROL問題已新增到] &lt;專案名稱&gt;</em></p> <p> </p> <p> 每日摘要通知的主題是<em> [！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>問題參考編號<br>新增問題的使用者名稱<br>問題型別<br>問題名稱<br>已輸入日期<br>問題優先順序<br>指派給名稱<br>問題狀態<br>主要連絡人<br>*專案名稱<br>*專案參考編號<br>*新增到專案的問題總數<br>*問題名稱<br>*指派給問題的使用者名稱<br>*每日摘要日期 </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我所在的專案上完成了一個問題</strong> </p> <p>專案團隊的成員會在專案上完成問題時收到電子郵件通知。<br>如需專案團隊的詳細資訊，請參閱<a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概述</a>。</p> <p>只有在專案狀態為[！UICONTROL目前]或[！UICONTROL規劃]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為<em>[！UICONTROL完成]： &lt;專案名稱&gt;</em>上的&lt;問題名稱&gt;</p> <p> 每日摘要通知的主題是<em> [！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>完成問題的使用者名稱<br>問題狀態<br>完成問題的日期和時間<br>上一個問題狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*完成的問題總數<br>*問題名稱<br>*指派給問題的使用者名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我所在的專案新增了一個未指派問題</strong> </p> <p>當未指派的問題新增到專案時，專案團隊的成員會收到電子郵件通知。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>立即通知電子郵件的主旨是<em>[！UICONTROL應該指派給此新問題的人員在] &lt;專案名稱&gt;？</em></p> <p> 每日摘要通知的主題是<em> [！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>問題參考編號<br>新增問題的使用者名稱<br>問題名稱<br>問題型別<br>已輸入日期<br>問題優先順序<br>指派給名稱（空白） <br>問題狀態<br>主要連絡人<br>*專案名稱<br>*專案參考編號<br>*新增的問題總數<br>*問題名稱<br>*新增問題的使用者名稱<br>*每日摘要的日期<br></td> 
   <td> <p><strong>即時</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我已新增至專案</strong> </p> <p>加入專案的使用者會在加入專案時收到電子郵件通知，除非使用者將自己加入專案。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為<em>[！UICONTROL您已新增至專案] &lt;專案名稱&gt;</em></p> <p> 每日摘要通知的主題是<em> [！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>專案參考編號<br>將您新增至專案的使用者名稱<br>專案[！UICONTROL計劃開始日期]<br>專案[！UICONTROL計畫完成日期]<br>專案完成百分比<br>專案擁有者<br><strong>上其他人的名稱<br>專案擁有者檢視更多詳細資料</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*每日摘要日期</p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我所在的專案上變更了狀態</strong> </p> <p>專案狀態變更時，專案團隊成員會收到電子郵件通知。 <br>如需專案團隊的詳細資訊，請參閱<a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概述</a>。</p> <p>即時通知電子郵件的主旨是<em>[！UICONTROL專案狀態變更]： &lt;專案名稱&gt;</em></p> <p> 每日摘要通知的主題是<em> [！UICONTROL您所在的專案摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>專案參考編號<br>變更專案狀態的使用者名稱<br>新專案狀態<br>專案狀態變更時的日期和時間<br>先前的專案狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*專案狀態<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
 </tbody> 
</table>
