---
content-type: reference
navigation-topic: notifications
title: 「通知：我正在執行的項目的資訊」
description: 下列通知會提醒您，您正在執行之專案中發生的活動。
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 6%

---

# 通知：關於我正在執行的項目的資訊

下列通知會提醒您，您正在執行之專案中發生的活動。

如需設定您收到哪些通知的詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另請參閱 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>包含的欄位 </p> <p> *僅限每日摘要欄位</p> </th> 
   <th>預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>向我所在的專案新增一個文件</strong> </p> <p>將檔案新增至專案時，專案團隊的成員會收到電子郵件通知，但新增檔案的使用者除外。</p> <p>僅當項目狀態為[!UICONTROL Current]且文檔不為「專用」時，才會發送通知。</p> <p>即時通知電子郵件的主旨是 <em>[!UICONTROL文檔已添加到] &lt;project name=""&gt;</em></p> <p>每日摘要通知的主旨是 <em>[!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>文檔參考編號<br>添加文檔的用戶的名稱<br>文檔名稱<br>新增日期<br>文檔詳細資訊（格式、大小、版本號）<br>文檔縮圖<br><strong>[!UICONTROL預覽]</strong> 和 <strong>[!UICONTROL下載]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*新增的檔案總數<br>*文檔名稱<br>*上傳檔案的使用者名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我所在的專案上完成了里程碑任務</strong> </p> <p>項目組的成員在項目上的里程碑任務完成時收到通知。 完成個人任務時不會發送通知。</p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>主旨行是 <em>[!UICONTROL完成]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>每日摘要通知的主旨是 <em> [!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>完成任務的用戶名<br>任務狀態<br>任務完成的日期和時間<br>上一任務狀態<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕 <br>*專案名稱<br>*項目參考編號<br>*已完成任務總數<br>*任務名稱<br>*完成任務的用戶名<br>*每日摘要日期<br></td> 
   <td><strong>[!UICONTROL每日]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我所在的一個專案變為使用中專案</strong> </p> <p>專案狀態設為[!UICONTROL目前]時，專案團隊的成員會收到電子郵件通知。</p> <p>注意：當項目狀態設定為[!UICONTROL當前]時，用戶必須列在項目的「人員配備」頁簽上才能接收通知。 有關向項目團隊添加用戶的資訊，請參閱 <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">管理專案團隊</a>.</p> <p>即時通知電子郵件的主旨是 <em>&lt;project name=""&gt; [!UICONTROL為最新 — 轉到您的項目並查看您的任務！]</em></p> <p> 每日摘要通知的主旨是 <em> [!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>項目參考編號<br>專案狀態<br>項目[!UICONTROL計畫完成日期]<br>專案擁有者<br>指派給您、您的其中一個工作角色或您其中一個團隊的工作清單<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*項目狀態<br>*每日摘要日期</p> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>我的團隊所在的一個專案變為進行中專案</strong> <p>專案生效時，團隊成員會收到電子郵件通知。 必須將團隊分配給至少一個任務以接收通知。</p><p>如果將個別使用者和團隊均指派給專案上的任務。 團隊將不會收到通知。</p><p>即時通知電子郵件的主旨是 <i>&lt;project name=""&gt; [!UICONTROL處於活動狀態 — 轉到您的項目並查看您的任務！]</i></p><p>每日摘要通知的主旨是 <em> [!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>專案名稱<br>Portfolio名稱<br>項目參考編號<br>專案狀態<br>項目[!UICONTROL計畫完成日期]<br>專案擁有者<br>指派給您團隊的任務清單<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*項目狀態<br>*每日摘要日期</td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我所在的專案已完成</strong> </p> <p>專案狀態為[!UICONTROL完成]時，專案團隊的成員會收到電子郵件通知。</p> <p>提示：如果項目定期完成，則啟用此選項可以為在許多項目上任務有限的用戶建立大量電子郵件。</p> <p>即時通知電子郵件的主旨是 <em>[!UICONTROL項目狀態更改]: &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主旨是 <em> [!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>項目參考編號<br>完成項目的用戶名<br>專案狀態<br>項目完成的日期和時間<br>上一個項目狀態<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*項目狀態<br>*每日摘要日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我所在的專案上完成了一項任務</strong> </p> <p>項目組的成員在項目上完成任務時會收到電子郵件通知。 <br>如需專案團隊的詳細資訊，請參閱 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概觀</a>.</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是 <em>[!UICONTROL完成]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>注意：如果任務更改為相當於[!UICONTROL Complete]的狀態，則電子郵件的主題仍顯示「[!UICONTROL Complete]」。</p> </p> <p><em> 每日摘要通知的主旨是：[!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>任務名稱<br>專案名稱<br>任務參考編號<br>完成任務的用戶名<br>任務狀態<br>更改任務狀態的日期和時間<br>上一任務狀態<br><strong>請參閱更多詳細資訊</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*已完成任務總數<br>*任務名稱<br>*完成任務的用戶名<br>*每日摘要日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我所在的專案新增了一個問題</strong> </p> <p>將問題新增至專案時，專案團隊的成員會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是 <em>[!UICONTROL問題已添加到] &lt;project name=""&gt;</em></p> <p> </p> <p> 每日摘要通知的主旨是 <em> [!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>問題參考編號<br>新增問題的使用者名稱<br>問題類型<br>問題名稱<br>輸入日期<br>問題優先順序<br>指派給名稱 <br>問題狀態<br>主要連絡人<br>*專案名稱<br>*項目參考編號<br>*專案新增的問題總數<br>*問題名稱<br>*分配給問題的用戶的名稱<br>*每日摘要日期 </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我所在的專案上完成了一個問題</strong> </p> <p>專案團隊成員的專案問題完成時，會收到電子郵件通知。<br>如需專案團隊的詳細資訊，請參閱 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概觀</a>.</p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是 <em>[!UICONTROL完成]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主旨是 <em> [!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>完成問題的用戶名<br>問題狀態<br>問題完成的日期和時間<br>上一個問題狀態<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*已完成問題總數<br>*問題名稱<br>*分配給問題的用戶的名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我所在的專案新增了一個未指派問題</strong> </p> <p>將未指派的問題新增至專案時，專案團隊的成員會收到電子郵件通知。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是 <em>[!UICONTROL應在上為此新問題分配誰] &lt;project name=""&gt;?</em></p> <p> 每日摘要通知的主旨是 <em> [!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>問題參考編號<br>新增問題的使用者名稱<br>問題名稱<br>問題類型<br>輸入日期<br>問題優先順序<br>指派給名稱（空） <br>問題狀態<br>主要連絡人<br>*專案名稱<br>*項目參考編號<br>*新增的問題總數<br>*問題名稱<br>*新增問題的使用者名稱<br>*每日摘要日期<br></td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被新增到一個專案</strong> </p> <p>新增至專案的使用者在新增時會收到電子郵件通知，除非使用者自行新增至專案。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是 <em>[!UICONTROL已將您添加到項目] &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主旨是 <em> [!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>項目參考編號<br>將您新增至專案的使用者名稱<br>項目[!UICONTROL計劃開始日期]<br>項目[!UICONTROL計畫完成日期]<br>項目完成百分比<br>項目上的其他名稱 <br>專案擁有者<br><strong>請參閱更多詳細資訊</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*每日摘要日期</p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我所在的專案上變更了狀態</strong> </p> <p>專案團隊的成員會在專案狀態變更時收到電子郵件通知。 <br>如需專案團隊的詳細資訊，請參閱 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概觀</a>.</p> <p>即時通知電子郵件的主旨是 <em>[!UICONTROL項目狀態更改]: &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主旨是 <em> [!UICONTROL您所在項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>項目參考編號<br>更改項目狀態的用戶的名稱<br>新項目狀態<br>項目狀態更改的日期和時間<br>上一個項目狀態<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*項目狀態<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
 </tbody> 
</table>
