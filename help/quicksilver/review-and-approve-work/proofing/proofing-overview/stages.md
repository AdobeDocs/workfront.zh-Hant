---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: 自動化工作流階段概觀
description: 證明階段是不同使用者檢閱證明的時間區段。 校樣從一個階段移至下一個階段時，Adobe Workfront會通知審核者該在何時處理校樣。
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# 自動化工作流階段概觀

證明階段是不同使用者檢閱證明的時間區段。 校樣從一個階段移至下一個階段時，Adobe Workfront會通知審核者該在何時處理校樣。

![phates_diagram.png](assets/stages-diagram-350x63.png)

階段分為兩種情況：

* [使用自動化工作流程建立校樣](#create-a-proof-with-an-automated-workflow)
* [為校樣的不同審核者指定截止時間](#assign-deadlines-for-different-reviewers-on-a-proof)

## 使用自動化工作流程建立校樣 {#create-a-proof-with-an-automated-workflow}

將自動工作流添加到校樣時，您可以設定要進行的審閱工作階段。

使用自動工作流設定校樣的階段時：

* 可以配置階段以連續運行或同時運行。
* 您可以將某些階段設定為只在完成前一階段後才會生效。
* 您可以將某些階段設為私人。 例如，對於在向客戶共用證明之前審核證明，並且不希望客戶看到結果的注釋的機構，這很有用。

有關使用自動化工作流建立校樣階段的說明，請參閱 [使用自動化工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>如果用戶未包含在任何階段中，但具有對文檔的訪問權並開啟校樣，則系統將建立一個稱為 *Workfront*.
>
>為開啟校樣的非收件者指派在「設定」 > 「檢閱和核准」 > 「角色」中指定的角色，供開啟檔案校樣的人使用。

## 為校樣的不同審核者指定截止時間 {#assign-deadlines-for-different-reviewers-on-a-proof}

當您為校樣的審核者指定不同的校樣截止日期時，系統會為每個截止日期建立一個階段，並將相應階段中每個截止日期的審核者分組。 

**範例：** 例如，如果您建立校樣，校樣由四位審核者組成：

* 對於評論家Olivia和Tony，您指定從現在起的14:00的截止時間。
* 對於Aaron和Amy，你指定幾天後17:00的截止時間。
* 你沒有為自己指定最後期限。

該系統為以下三個「組」審閱者分別建立一個階段：

![png](assets/stages-350x239.png)

如果您與其他審核者共用校樣，但未指定截止日期，Workfront會將使用者新增至沒有截止日期的階段3。 
