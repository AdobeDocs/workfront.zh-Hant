---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 使用Adobe Workfront API新增進階校訂選項
description: 使用Adobe Workfront API新增進階校訂選項
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# 透過Adobe Workfront API建立校訂時新增進階校訂選項

在Workfront API中建立校訂時，您可以新增進階校訂選項。

使用以下工作流程之一，透過API將校訂選項新增到校訂中：

* （建議）使用Workfront API建立簡單的校訂，然後使用ProofHQ API新增進階校訂選項到校訂中

* 使用Workfront API中的JSON建立具有進階校訂選項的校訂

## 使用Workfront和ProofHQ API建立校訂（建議） {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

本節說明如何透過Workfront API，使用Workfront和ProofHQ API的組合，使用進階校訂選項來建立校訂。

ProofHQ API包含多種在Workfront API中無法用於校訂的動作。 使用這些動作，您可以比Workfront API更精確地修改或設定校訂。

如需ProofHQ API的概觀，請參閱[PoofHQ概觀](../../proofhq-api/general/overview.md)。 您也可以參閱[ProofHQ檔案](https://api.proofhq.com/home.html)。

>[!NOTE]
>
>* Workfront API是REST-FUL API。 ProofHQ API是SOAP API。
>* 在ProofHQ API中建立的校訂不會自動連結至Workfront。 因此，我們建議先在Workfront API中建立校訂，再使用ProofHQ API更新它們。
>

### 使用進階校訂選項建立校訂

1. 使用Workfront API中的`Document createProof`動作建立校訂。

   >[!NOTE]
   >
   >建立校訂時，將`{}`設定為`advancedProofingOptions`引數的值。

1. 建立校訂後，使用ProofHQ API新增任何進階選項。

### 範例

本節顯示您可以使用ProofHQ API進行的一些更新範例。

**範例：**

* [校訂可以下載、有訊息且已公開共用](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [更新階段，讓它不是私人的、不是強制性的，而且只需要一次核准](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [將兩個收件者新增至沒有主要決策者的校訂](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**校訂可以下載、有訊息且已公開共用**

您可以在[ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html)頁面上找到此端點的檔案。

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

**更新階段，讓它不是私人的、不是強制性的，而且只需要一次核准**

您可以在[ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html)頁面上找到此端點的檔案。

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

**將兩個收件者新增至沒有主要決策者的校訂**

您可以在[ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html)頁面上找到此端點的檔案。

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

## 在Workfront API中使用JSON建立校訂

本節說明如何透過Workfront API，使用JSON作為Workfront API中的引數值，使用進階校訂選項來建立校訂

### 使用進階校訂選項建立校訂

您可以使用`Document createProof`動作，透過Workfront API建立校樣。 此動作接受`advancedProofingOptions`引數，其值型別為`string`。 若要在`createProof`動作中加入進階校訂選項，您必須以JSON格式輸入`advancedProofingOptions`引數中的選項。

>[!NOTE]
>
>可能很難預測要包含在advancedProofingOptions JSON中的欄位。 在Workfront中使用進階校訂時，您可能會想要檢查組織的網路資料，並將JSON建立在組織常用的欄位和值上。
>
>由於這些欄位可能很難預測，因此建議您使用Workfront API建立校訂，然後使用ProofHQ API更新它。 如需詳細資訊，請參閱本文中的[使用Workfront和ProofHQ API建立校訂（建議）](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended)

### 範例

此範例顯示當您為`advancedProofingOptions`引數建立JSON時，可以使用的欄位和格式。 您的`advancedProofingOptions` JSON檔案可以包含比此處顯示更多或更少的欄位。

**範例：**

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
