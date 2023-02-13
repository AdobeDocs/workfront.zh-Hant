---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 使用Adobe Workfront API新增進階校對選項
description: 使用Adobe Workfront API新增進階校對選項
author: John
feature: Workfront API, Workfront Proof
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---


# 透過Adobe Workfront API建立校樣時，新增進階校樣選項

在Workfront API中建立校樣時，您可以新增進階校樣選項。

使用下列其中一個工作流程，使用API將校對選項新增至校樣：

* （建議）使用Workfront API建立簡單校樣，然後使用ProofHQ API將進階校樣選項新增至校樣

* 在Workfront API中使用JSON建立包含進階校對選項的校樣

## 使用Workfront和ProofHQ API建立校樣（建議使用） {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

本節說明如何結合使用Workfront和ProofHQ API，透過Workfront API使用進階校對選項來建立校樣。

ProofHQ API包含許多無法用於Workfront API中校樣的動作。 透過使用這些動作，您可以比Workfront API更精確地修改或設定校樣。

如需ProofHQ API的概觀，請參閱 [PoofHQ概述](../../proofhq-api/general/overview.md). 您也可以參閱 [ProofHQ檔案](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* Workfront API是REST風格的API。 ProofHQ API是SOAP API。
>* 在ProofHQ API中建立的校樣不會自動連結至Workfront。 因此，建議您先在Workfront API中建立校樣，再使用ProofHQ API進行更新。
>


### 使用進階校對選項建立校樣

1. 使用 `Document createProof` 動作。

   >[!NOTE]
   建立校樣時，請勿包含advancedPookingOptions參數的值。

1. 建立校樣後，請使用ProofHQ API來新增任何進階選項。

### 範例

本節顯示一些您可以使用ProofHQ API進行的範例更新。

**範例:**

* [可下載校樣、傳送訊息，並公開共用](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [更新階段，使其不是專用階段，而非強制階段，並且只需要一個核准](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [將兩個收件者新增至沒有主要決策者的校樣](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**可下載校樣、傳送訊息，並公開共用**

此端點的檔案位於 [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html) 頁面。

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**更新階段，使其不是專用階段，而非強制階段，並且只需要一個核准**

此端點的檔案位於 [ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) 頁面。

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**將兩個收件者新增至沒有主要決策者的校樣**

此端點的檔案位於 [ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) 頁面。

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## 在Workfront API中使用JSON建立校樣

本節說明如何透過Workfront API，使用JSON做為Workfront API中的參數值，使用進階校對選項建立校樣

### 使用進階校對選項建立校樣

您可以透過Workfront API使用 `Document createProof` 動作。 此動作接受 `advancedProofingOptions` 參數，其值類型為 `string`. 若要在 `createProof` 動作，您必須在 `advancedProofingOptions` 參數。

>[!NOTE]
您很難預測進階PookingOptions JSON中要包含的欄位。 在Workfront中使用進階校對時，您可能會想要檢查組織的網路資料，並將JSON放在貴組織常用的欄位和值上。
由於這些欄位可能難以預測，建議您使用Workfront API建立校樣，然後使用ProofHQ API更新。 如需詳細資訊，請參閱 [使用Workfront和ProofHQ API建立校樣（建議使用）](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) 本文

### 範例

此範例顯示在為 `advancedProofingOptions` 參數。 您的 `advancedProofingOptions` JSON檔案中的欄位數可能比此處所示的要多。

**範例:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
