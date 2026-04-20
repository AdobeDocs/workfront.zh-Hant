---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 設定AI共同作業人員
description: 身為Adobe Workfront管理員，您可以設定AI共同作業人員，並將其指派給專案和任務。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: d20215ae2d535ba98ca27ce62aaa28fd372e935a
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 2%

---

# 設定AI共同作業人員

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽Sandbox」環境中使用。</span>

>[!IMPORTANT]
>
>目前，內容檢閱者是唯一可用的AI Collaborator型別。 未來將提供更多的AI Collaborator功能。

AI共同作業人員是將AI代理程式加入您的專案和任務的方法。 您可以設定AI共同作業人員，然後將其指派為您想要的使用者。

例如，您可以使用品牌指南設定檢閱者型別的AI Collaborator，然後指派該共同作業人員檢閱檔案。

可用的AI Collaborator型別包括：

* 檢閱者：使用品牌或Adobe Brand Intelligence建立共同作業人員，然後將共同作業人員指派為資產的檢閱者。

  如需詳細資訊，請參閱[開始使用Workfront內容檢閱者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)。


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>Standard、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[！UICONTROL標準]</p>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
  </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

* 貴組織必須已簽署一份Adobe Gen AI合約。

  如需詳細資訊，請參閱Workfront的AI助理一文中的[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* 您必須先在Workfront中設定品牌，才能將其用於檢閱者型別的AI共同作業人員。

  如需指示，請參閱[建立和管理內容檢閱者的品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。
* <span class="preview">若要針對檢閱者AI共同作業人員使用Adobe Brand Intelligence，您的組織必須在Workfront中使用統一的檢閱和核准體驗。</span>

  <span class="preview">如需詳細資訊，請參閱[開始進行統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。</span>

## 建立新的檢閱者型別AI共同作業人員

Reviewer AI共同作業人員可設定為使用Workfront品牌或Adobe Brand Intelligence。

* **品牌**：品牌是在Workfront中建立。 您可以上傳包含品牌方針的PDF檔案或手動輸入品牌元素，在Workfront中建立品牌。
* <span class="preview">**Adobe Brand Intelligence**：當AI共同作業人員使用Adobe Brand Intelligence檢閱資產時，您可以在Frame.io中檢視檢閱者所做的評論。 </span>

>[!NOTE]
>
>沙箱環境中沒有內容檢閱者可用。


{{step-1-to-setup}}

1. 在左側導覽列中，按一下&#x200B;**AI共同作業人員**。
1. 按一下畫面右上角的&#x200B;**新增共同作業人員**。
1. 按一下&#x200B;**檢閱者**，然後按一下&#x200B;**繼續**。

   >[!NOTE]
   >
   >目前，只有檢閱者型別可用。 未來將提供更多的AI共同作業人員型別。

1. 在「共同作業人員名稱」欄位中，輸入共同作業人員的名稱。 這是出現在任務可用受指派人清單中的名稱。
1. <span class="preview">選取共同作業人員要使用品牌或Adobe Brand Intelligence進行稽核。</span>
1. （視條件而定）如果AI共同作業人員將使用品牌，請選取它將使用的品牌和品牌指引。
1. 按一下「**儲存**」。

## 管理AI共同作業人員

您可以編輯、複製和刪除現有的AI共同作業人員。

{{step-1-to-setup}}

1. 在左側導覽列中，按一下&#x200B;**AI共同作業人員**。
1. （條件式）若要編輯共同作業人員，請按一下您要編輯的共同作業人員名稱，在[編輯共同作業人員]視窗中進行任何編輯，然後按一下[儲存]。****
1. （視條件而定）若要複製Collaborator，請按一下要複製之AI Collaborator列中的復製圖示![復製圖示](assets/copy-ai-collaborator.png)，按一下複製的名稱，在Edit Collaborator視窗中進行任何編輯，然後按一下&#x200B;**儲存**。
1. （視條件而定）若要刪除Collaborator，請在您要刪除的AI Collaborator列中按一下「刪除」圖示![「刪除」圖示](assets/delete-collaborator-icon.png)，然後按一下&#x200B;**「刪除」**。
