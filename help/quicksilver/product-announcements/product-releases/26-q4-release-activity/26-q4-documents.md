---
title: 2026年第四季檔案增強功能
description: 2026年第四季檔案增強功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# 2026年第四季檔案增強功能

本頁說明2026年第四季版本的檔案增強功能與預覽環境。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第四季版本週期目前可用的所有變更清單，請參閱[2026年第四季版本概觀](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

<!--

## Frame comment visibility in Workfront

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When an approval workflow is created for a document, users can leave comments and make annotations in the Frame.io viewer. These comments are not displayed in the Workfront Comments panel, but you can view them in the Frame.io viewer.

Now, the Comments panel in Workfront displays a message letting you know when new comments are available in Frame.io.

For more information, see [Add an update to a document](/help/quicksilver/documents/managing-documents/add-update-documents.md).

-->

## 從核准電子郵件連結直接校訂存取權

>[!NOTE]
>
>預覽：不適用
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

當檔案附加校訂時，核准電子郵件中的「前往檢閱」連結現在會直接開啟校訂檢視器，因此檢閱者和核准者可以立即開始檢閱。 如果檔案沒有校訂，連結會繼續開啟檔案的核准區段，就像之前一樣。

<!--

## Add teams to approvals for objects using Adobe cloud storage

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now add a Workfront Team as an approver or reviewer on a document approval or approval template, instead of adding each person individually:

* Objects on Adobe cloud storage: Workfront adds each active team member individually, so the approver list always reflects who's currently on the team.
* Objects using legacy Workfront storage: The team is added as a single participant by default, but you can now choose to add each team member as an individual participant.
* In approval templates, Workfront stores a reference to the team and expands it into active members when you apply the template to a document, not when you save the template.

For more information, see:

* [Create an approval workflow in the new Documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Create an approval workflow in the legacy documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

-->

## 在專案範本上設定Frame.io工作區

>[!NOTE]
>
>預覽： 2026年9月3日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

如果您的組織使用Adobe雲端儲存空間，而且您擁有Frame.io Enterprise授權，您現在可以在專案範本的專案詳細資訊中選擇Frame.io工作區。 從範本建立的專案會自動使用範本上設定的工作區，因此專案會路由到所需的Frame.io工作區，而不需要在專案建立時執行額外的動作。

新欄位會列出您有權指派專案的Frame.io工作區。 此欄位在範本上隨時保持可編輯狀態；變更僅適用於更新後建立的專案，因此現有專案會保留其原始工作區。

從範本建立專案後，其Frame.io工作區欄位就會變成唯讀，而且會連結至Frame.io中的工作區。

如果您沒有Frame.io企業授權，專案會繼續移至Workfront的預設工作區。

如需詳細資訊，請參閱[編輯專案範本](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)和[管理專案概觀區域中的資訊](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md)。

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

-->

## 電子郵件主旨列中的自訂訊息

>[!NOTE]
>
>預覽：不適用
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

當您在檔案核准上設定自訂訊息時，該訊息現在也會顯示在核准請求電子郵件的主旨行中，在設定到期日期之前先行。 這可讓檢閱者直接從其收件匣檢視需要注意的事項和方式，而不需開啟電子郵件。

如需詳細資訊，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

<!--

## Redesigned Versions panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Versions panel in the new Documents area has a new design:

* Versions are labeled V1, V2, and so on to drive consistency with Frame.io.
* Each version shows its approval status, such as "Approved" or "Withdrawn", directly in the list.
* The panel now lists only Version history — there's no longer a separate "latest file" entry at the top.

Previously, versions were timestamped instead of numbered.

For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Redesigned Approvals panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Approvals panel in the new Documents area now shows approval history across versions:

* The panel lists the approval workflow for every version that has one, not just the current version.
* Withdrawn workflows stay in the list, so you can still review their prior decisions.
* Expand any version to see its stages, approver decisions, decision rule, and due dates without leaving the panel.

Previously, the Approvals panel only showed the current version's workflow.

For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

-->

## 將影像附加至Adobe雲端儲存物件上的註解

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年7月30日
>適用於所有人的生產： 2026年7月30日
>[!BADGE 不在排程]{type=Neutral}內

使用Adobe雲端儲存空間作為統一檢閱和核准一部分的組織現在可以將影像檔案直接附加至評論，將意見反應、內容和支援的視覺效果一起保留在單一可追蹤的評論對話串中。 這彌補了之前的空白，即只有舊版Workfront儲存空間中的組織才能在評論中附加影像。

Adobe雲端儲存空間組織現在支援所有媒體型別影像格式。 （舊版物件註解僅繼續支援.jpg、.gif和.png檔案。） 舊版或Adobe雲端儲存物件的註解不支援非影像檔案。

如需詳細資訊，請參閱[更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 從Experience Manager Assets將資產連結至Adobe雲端儲存空間

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

如果您的組織使用Adobe雲端儲存空間，您可以將來自Experience Manager Assets的個別資產連結至任何支援檔案的Workfront物件。 連結的內容會自動保持同步：在Experience Manager Assets中進行的變更會顯示在Workfront中，而您可以提取新的資產版本而不離開Workfront。

連結功能由「內容顧問」提供技術支援，因此您也可以在選取內容時取得AI 搜尋、智慧建議、行銷活動簡訊分析等等。

如需詳細資訊，請參閱[將Experience Manager Assets的內容與Adobe雲端儲存空間連結](/help/quicksilver/review-and-approve-work/native-integrations/link-aem-assets-cloud-storage.md)。
