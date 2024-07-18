---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: 自動化工作流程階段概觀
description: 校訂階段是不同使用者檢閱校訂的時間區段。 當校訂從一個階段移至下一個階段時，Adobe Workfront會通知檢閱者，讓他們知道何時需要處理。
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# 自動化工作流程階段概觀

校訂階段是不同使用者檢閱校訂的時間區段。 當校訂從一個階段移至下一個階段時，Adobe Workfront會通知檢閱者，讓他們知道何時需要處理。

![stages_diagram.png](assets/stages-diagram-350x63.png)

階段會發生在兩種不同的情況中：

* [使用自動化工作流程建立校訂](#create-a-proof-with-an-automated-workflow)
* [為校樣上的不同稽核者指派截止日期](#assign-deadlines-for-different-reviewers-on-a-proof)

## 使用自動化工作流程建立校訂 {#create-a-proof-with-an-automated-workflow}

將自動化工作流程新增到校訂時，您可以設定希望發生的稽核工作階段。

當您使用自動工作流程設定校訂的階段時：

* 您可以將階段設定為連續或同時執行。
* 您可以將某些階段設定為僅在前一個階段完成後才啟用。
* 您可以將某些階段設為私人。 例如，這對於在與使用者端共用校訂之前檢視校訂，並且不希望使用者端看到所產生的評論的機構非常有用。

如需使用自動化工作流程建立校訂階段的相關指示，請參閱[使用自動化工作流程建立進階校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)。

>[!NOTE]
>
>如果使用者未包含在任何階段中，但擁有檔案的存取權並開啟校訂，則系統會建立名為&#x200B;*Workfront*&#x200B;的階段。
>
>開啟檔案校樣的使用者會被指派設定>檢閱和核准>開啟檔案校樣的非收件者角色中指定的角色。

## 為校樣上的不同稽核者指派截止日期 {#assign-deadlines-for-different-reviewers-on-a-proof}

當您為校訂上的稽核者指派不同的校訂截止日期時，系統會為每個截止日期建立一個階段，並將稽核者分組到對應階段中的每個截止日期。 

**範例：**&#x200B;例如，如果您建立有四名稽核者的校訂：

* 對於稽核者Olivia和Tony，您指定從現在起數天後的14:00的截止日期。
* 對於Aaron和Amy，您會在幾天後指定17:00的截止日期。
* 您沒有指定自己的截止日期。

系統會為每個檢閱者的「群組」建立一個階段：

![階段.png](assets/stages-350x239.png)

如果您與其他檢閱者共用校訂，但未指定截止日期，則Workfront會將使用者新增至沒有截止日期的階段3。 
