---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: 設定AI共同作業人員
description: 身為Adobe Workfront管理員，您可以設定AI共同作業人員，並將其指派給專案和任務。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 2%
---
# 設定AI共同作業人員

AI共同作業人員是將AI代理程式加入您的專案和任務的方法。 您可以設定AI共同作業人員，然後將其指派為您想要的使用者。

例如，您可以使用品牌指南設定檢閱者型別的AI Collaborator，然後指派該共同作業人員檢閱檔案。

可用的AI Collaborator型別包括：

* AI檢閱者：使用品牌或Adobe Brand Intelligence建立共同作業人員，然後將共同作業人員指派為資產的檢閱者。

  如需詳細資訊，請參閱[開始使用Workfront AI檢閱者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)。

* 工作代理程式：使用Copilot或Writer建立共同作業人員，然後將共同作業人員指派給工作以完成工作層級的工作。

  如需詳細資訊，請參閱[使用工作代理](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>選取、Prime或Ultimate</p></td> 
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

### 對於AI檢閱者：

* 貴組織必須已簽署一份Adobe Gen AI合約。

  如需詳細資訊，請參閱Workfront的AI助理一文中的[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* 您必須先在Workfront中設定品牌，才能將其用於AI檢閱者。

  如需指示，請參閱[為AI檢閱者建立和管理品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。
* 若要針對AI檢閱者使用Adobe Brand Intelligence，您的組織必須在Workfront中使用統一的檢閱和核准體驗。

  如需詳細資訊，請參閱[開始進行統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。

### 工作代理程式

您必須先在Claude、Copilot Studio或Writer中設定代理程式，才能將它當作Work Agent使用。

## 建立新的AI稽核者

AI檢閱者可設定為使用Workfront品牌或Adobe Brand Intelligence。

* **品牌**：品牌是在Workfront中建立。 您可以上傳包含品牌方針的PDF檔案或手動輸入品牌元素，在Workfront中建立品牌。
* **Adobe Brand Intelligence**： AI共同作業人員使用Adobe Brand Intelligence檢閱資產時，您可以在Frame.io中檢視AI檢閱者所做的註解。


{{step-1-to-setup}}

1. 在左側導覽列中，按一下&#x200B;**AI共同作業人員**。
1. 按一下畫面右上角的&#x200B;**新增共同作業人員**。
1. 按一下&#x200B;**檢閱者**，然後按一下&#x200B;**繼續**。
1. 在「共同作業人員名稱」欄位中，輸入共同作業人員的名稱。 這是出現在任務可用受指派人清單中的名稱。
1. 選取共同作業人員將使用品牌或Adobe Brand Intelligence進行稽核。
1. （視條件而定）如果AI共同作業人員將使用品牌，請選取它將使用的品牌和品牌指引。
1. 按一下「**儲存**」。

## 設定工作代理程式

工作代理程式是可指派給Workfront中工作的代理程式。 您可使用名稱、存取層級和其他詳細資訊來設定「工作代理程式」，並將其指派給工作，就像指派使用者一樣。

因為工作代理程式是代理程式，其動作和功能會在您設定代理程式的位置進行設定。 目前，作為工作代理使用的代理可以在Copilot Studio、Claude或Writer中建立。

工作代理僅可指派給任務，目前無法指派給問題。

如需建立代理程式以作為工作代理程式時的最佳作法清單，請參閱[建立工作代理程式之代理程式的最佳作法](#best-practices-for-creating-an-agent-for-a-work-agent)。

### 在Workfront中設定工作代理程式

{{step-1-to-setup}}

1. 在左側導覽列中，按一下&#x200B;**AI共同作業人員**。
1. 按一下畫面右上角的&#x200B;**新增共同作業人員**。
1. 選取&#x200B;**工作代理程式**，然後按一下&#x200B;**繼續**。
1. 在AI共同作業人員名稱欄位中，輸入共同作業人員的名稱。 這是出現在任務可用受指派人清單中的名稱。
1. 在AI共同作業人員說明欄位中，輸入共同作業人員用途或所執行動作的說明。
1. 在存取層級欄位中，選取此共同作業人員的存取層級。 此存取層級會控制共同作業人員可以執行的動作，就像存取層級會控制使用者可以執行的動作一樣。
1. 在&#x200B;**選擇代理程式來源**&#x200B;區域中，選取您要連線在通用平台（例如Copilot或Writer）中建立的代理程式，或使用自訂代理程式。
1. （視條件而定）如果您使用來自通用平台的代理程式，請輸入代理程式平台的驗證詳細資訊：

   | 平台 | 必要的驗證 |
   |---|---|
   | Copilot Studio | 網頁管道密鑰 |
   | Claude 管理的代理 | Anthropic API金鑰<br>代理程式識別碼<br>環境識別碼 |
   | 作者 | API金鑰<br>應用程式識別碼 |

1. 按一下&#x200B;**測試連線**。 這可讓您知道連線設定是否正確。
1. 在&#x200B;**當共同作業人員完成其工作後，它可以**&#x200B;區域，切換您要共同作業人員採取的動作。
1. 按一下「**儲存**」。

如需工作代理程式的詳細資訊，包括如何將其指派給工作，請參閱[使用工作代理程式](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。


### 為工作代理程式建立代理程式的最佳做法

您可能會發現下列最佳實務有助於在Workfront中建立要作為工作代理的代理程式。 若要檢視最佳實務，請按一下您建立代理程式之應用程式的區段。

+++ 克勞德

1. 瀏覽至[platform.claude.com](https://platform.claude.com/)的Claude主控台。
1. 建立API金鑰。
   1. 在API金鑰下，按一下右上角的&#x200B;**建立金鑰**。
   1. 提供名稱和到期日。
   1. 複製金鑰並儲存在安全的地方。 您需要此金鑰才能在Workfront中設定工作代理程式。

1. 建立環境。
   1. 在&#x200B;**受管理的代理程式** > **環境**&#x200B;下，按一下右上角的&#x200B;**建立環境**。
   1. 提供適用的名稱和託管型別。
   1. 視需要設定共用套件和中繼資料。 環境可在多個代理程式中重複使用，並允許共用套件和中繼資料。
      環境ID會顯示在左上角的環境名稱下方。

1. 建立代理。
   1. 在[受管理的代理程式] > [代理程式]下，按一下右上角的[建立代理程式] ****。
   1. 提供適用的名稱、型號、系統提示、技能及工具。 描述性，因為「工作代理程式」會將工作內容傳遞至此代理程式，然後執行工作。
      代理程式ID會顯示在左上角的代理程式名稱下方。

1. 在Workfront中設定工作代理程式。
   1. 輸入您的API金鑰、環境ID和代理ID
   1. 按一下&#x200B;**測試連線**&#x200B;以進行驗證。

1. 將工作代理指派給Workfront工作。
   1. 工作代理程式會在所有前置任務完成後觸發。

+++
<!--
+++ Copilot Studio



+++
-->
+++ 作者

>[!NOTE]
>
> 您可以使用Writer代理程式作為Work Agent，但Writer教戰手冊不能用作Work Agent。

建立代理程式以用作Writer中的工作代理程式時，我們建議使用下列工作流程。

有關建立代理程式的詳細資訊，請參閱[Writer檔案](https://dev.writer.com/no-code/introduction)。

1. 在Writer AI Studio中建立無程式碼應用程式。
1. 新增單一文字輸入欄位。 您可以使用預設名稱「文字輸入」。
1. 將`@TextInput`新增至您的提示。 在應用程式設定的提示區段中，確認您的提示範本參考了輸入變數。 若沒有此專案，模型就不會看到任務資料。
1. 調整您的提示以立即產生輸出。 移除在回應之前要求使用者澄清或其他內容的任何指示。 例如：「當您收到輸入時，將其視為內容產生請求，並立即產生輸出。 請勿要求澄清。」
1. 複製您的API金鑰和應用程式ID。 您需要在Workfront中設定工作代理程式。

   * 如需在Writer中設定API金鑰的指示，請參閱Writer檔案中的[快速入門](https://dev.writer.com/home/quickstart)。
   * 如需在Writer中設定應用程式ID的說明，請參閱Writer檔案中的[透過API叫用無程式碼代理程式](https://dev.writer.com/home/applications)。

1. 在Workfront中設定工作代理程式。 在設定中，輸入您的API金鑰和應用程式ID，然後按一下[測試連線] **以進行驗證。**
1. 將工作代理指派給Workfront工作。 當任務的所有前置任務完成時，「工作代理程式」就會開始工作。

+++

## 管理AI共同作業人員

您可以編輯、複製和刪除現有的AI共同作業人員。

{{step-1-to-setup}}

1. 在左側導覽列中，按一下&#x200B;**AI共同作業人員**。
1. （條件式）若要編輯共同作業人員，請按一下您要編輯的共同作業人員名稱，在[編輯共同作業人員]視窗中進行任何編輯，然後按一下[儲存]。****
1. （視條件而定）若要刪除Collaborator，請在您要刪除的AI Collaborator列中按一下「刪除」圖示![「刪除」圖示](assets/delete-collaborator-icon.png)，然後按一下&#x200B;**「刪除」**。
