---
product-area: workfront-integrations;projects
keywords: google，doc，檔案，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 從Google Workspace檢視及管理 [!DNL Adobe Workfront] 物件詳細資料
description: 您無需離開Google Workspace，即可檢視和管理工作專案的詳細資料。 例如，您可以在Google Workspace的 [!DNL Adobe Workfront] 內讀取任務的說明、檢視其父系物件、變更其狀態，以及將其標示為完成。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 0f15b05f-3b4a-4f0b-9d9a-21a0f97de1ea
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 從[!DNL Adobe Workfront]檢視及管理[!DNL Google Workspace]物件詳細資料

>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，下列Google Workspace適用的Workfront功能在&#x200B;**2026年2月28日**&#x200B;後將無法使用：
>
>* 從Workfront存取Google Workspace功能
>
>* 從Gmail或Google行事曆網站面板檢視和管理Workfront工作
>
>為了滿足貴組織與Google Workspace的整合需求，我們建議您使用Workfront自動化和整合。
>
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Google Workspace之Workfront自動化與整合模組的特定功能相關資訊，請參閱[Gmail模組](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)和[Google行事曆模組](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)。

您無須離開[!DNL Google Workspace]即可檢視及管理工作專案的詳細資料。 例如，您可以讀取任務的說明、檢視其父系物件、變更其狀態，以及將其標示為完成，全部在[!DNL Adobe Workfront for Google Workspace]內。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL Work]， [!UICONTROL 計畫]</p> </td> 
  </tr> 
</tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 先決條件

在[!DNL Google Workspace]中檢視和管理工作專案詳細資料之前，您必須

* 安裝[!DNL Workfront for Google Workspace]\
   如需指示，請參閱[安裝 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)。

## 在[!DNL Google Workspace]中檢視和管理工作專案詳細資料

1. 如果未顯示Google Workspace[!UICONTROL 的]Workfront面板，請按一下頁面最右側[!DNL Workfront]附加元件側邊欄中的![圖示](assets/wf-lion-icon.png)Workfront圖示[!DNL Google Workspace]。
1. 移至[!DNL Workfront]內的[!DNL Google Workspace]任務或問題，如[存取 [!DNL Adobe Workfront] [!UICONTROL 首頁]來自 [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/access-wf-home-content-from-g-suite.md)的內容中所述。

   當您選取任務或問題時，**[!UICONTROL 詳細資料]**&#x200B;索引標籤會開啟。 **[!UICONTROL 詳細資料]**&#x200B;標籤上方的區域會顯示父物件的名稱、任務或問題的名稱，以及[!UICONTROL 到期日] （如果是任務）或[!UICONTROL 優先順序日期] （如果是問題）。


   您可以在不離開[!DNL Google Workspace]的情況下在此標籤上執行各種工作，包括：

   * 檢視物件的&#x200B;**[!UICONTROL 描述]**&#x200B;和其他詳細資料，例如指派給物件的使用者、**[!UICONTROL 優先順序]**、請求者、**[!UICONTROL 規劃完成日期]**&#x200B;以及附加到物件的任何自訂欄位和表單。

     自訂表單僅顯示已新增資訊的欄位。

   * 按一下&#x200B;**[!UICONTROL 父專案]**&#x200B;區域以檢視父物件的詳細資訊。

     >[!TIP]
     >
     >當您的任務和問題具有相同名稱，而您需要加以區分時，這會很有幫助。

   * 按一下&#x200B;**[!UICONTROL 處理工作]**，接受指派給您的工作。
   * 編輯各種選項，例如&#x200B;**[!UICONTROL Done]**&#x200B;選項、**[!UICONTROL Status]**&#x200B;和&#x200B;**[!UICONTROL 完成百分比]**。

     在&#x200B;**[!UICONTROL 完成百分比]**&#x200B;下，輸入數字和（選擇性）百分比符號%，以表示您在專案上的進度。
   * 檢視核准請求的相關資訊，包括擁有者、大小和任何附件。
   * **[!UICONTROL 核准]**&#x200B;或&#x200B;**[!UICONTROL 拒絕]**&#x200B;核准要求與檔案。

   * **[!UICONTROL 授予]**&#x200B;或&#x200B;**[!UICONTROL 忽略]**&#x200B;存取要求。

1. （選擇性）按一下&#x200B;**[!UICONTROL 在[!DNL Workfront]]**&#x200B;中檢視以移至[!DNL Workfront]中的目前工作專案。

* 如需有關在[!UICONTROL 中使用]更新[!DNL Workfront for Google Workspace]索引標籤的資訊，請參閱[從 [!DNL Adobe Workfront] 更新 [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/update-a-workfront-object-in-gsuite.md)物件。
* 如需有關在[!UICONTROL 中使用]檔案[!DNL Workfront for Google Workspace]索引標籤的資訊，請參閱[從[!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/view-and-manage-documents-in-gsuite.md)檢視及管理檔案。
