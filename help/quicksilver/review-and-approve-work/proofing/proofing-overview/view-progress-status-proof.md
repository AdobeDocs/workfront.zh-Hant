---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 校訂進度和狀態概觀
description: 您可以檢視有關校訂如何在稽核流程中進行的資訊，並從檔案區域檢視校訂決策狀態的整體摘要。
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 1%

---

# 校訂進度和狀態概觀

您可以檢視有關校訂如何在稽核流程中進行的資訊，並從檔案區域檢視校訂決策狀態的整體摘要。

## 校訂進度概觀

校訂進度指出對校訂完成的工作，從您傳送校訂給收件者到他們對校訂做出決定為止。 進度圖示S、O、C和D會出現在校樣名稱旁，並提供有關校樣進度的資訊。

![](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>進度圖示</strong> </p> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>已傳送</strong> </p> </td> 
   <td> <p>校訂已傳送給指派的收件者。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>已開啟</strong> </p> </td> 
   <td> <p>所有指派的收件者都會開啟校樣或校樣詳細資訊頁面。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>個註解</strong> </p> </td> 
   <td> <p>所有指派的收件者至少會對校訂進行一項評論。</p> <p>如果沒有檢閱者指派給校訂，則進度列中不會出現<strong>C</strong>圖示。</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>已作出決定</strong> </p> </td> 
   <td> <p>所有獲指派的核准者都會對校訂做出決定，所有獲指派的核准者都會對校訂做出決定，除非校訂建立者僅指定一個決定即可。</p> <p>如果沒有為校訂指定的核准者（決策者），<strong>D</strong>圖示就不會出現在進度列中。 </p> </td> 
  </tr> 
 </tbody> 
</table>

進度圖示可以以下列顏色顯示，以指示有關校樣進度的特定資訊：

* **綠色**：完成。
* **白色**：未完成。
* **橘色**：未完成且離期限不到24小時。
* **紅色**：未完成且已超過期限。

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## 校訂狀態概觀

校訂狀態顯示校訂所需的決定狀態。 證明的狀態是由「最壞情況」參與者所驅動。 例如，假設證明上有三個決定：兩個決定的狀態為&#x200B;**已接受**，另一個決定的狀態為&#x200B;**已拒絕**。 **已拒絕**&#x200B;的「最壞情況」決定會優先於其他決定，而且證明的整體狀態會顯示為&#x200B;**已拒絕**。 

![](assets/proof-edit-existing-progress-350x62.png)

標準狀態選項如下：

* 未決
* 已核准
* 已核准 (附帶變更)
* 需要變更
* 不相關

如果您已在帳戶中設定自訂決策，則狀態選項會反映您的自訂決策設定。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->
