---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 連結介於 [!DNL Adobe Workfront] 和 [!DNL Jira]之間的專案
description: 您可以自動或手動將 [!DNL Jira] 問題連結至 [!DNL Adobe Workfront] 任務或問題。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: 97d755c71eb1bdfa8a031fa387741318f9a7f261
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 0%

---

# 連結介於[!DNL Adobe Workfront]和[!DNL Jira]之間的專案

<!-- Audited: 5/2025 -->

您可以自動或手動將[!DNL Jira]問題連結至[!DNL Adobe Workfront]個任務或問題。

[!DNL Workfront]中只有一個專案可以連結到[!DNL Jira]中的一個專案。 您永遠無法將一個[!DNL Workfront]專案連結至多個[!DNL Jira]問題，也無法將一個[!DNL Jira]問題連結至多個[!DNL Workfront]專案。

## 存取需求

您必須具備下列條件：

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] 計畫]</a></td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront]授權總覽</a></td> 
   <td> 
   <p>新增：標準<p>
   <p>或</p>
   <p>目前：計畫 </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira存取</td> 
   <td> <p>系統管理員存取權</p> <p><b>重要</b>

建議您在[!DNL Jira]和[!DNL Workfront]中建立個別的系統管理員帳戶以專用於此整合，而不使用可能附加至使用者的現有帳戶。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。 如需[!DNL Workfront]管理員的相關資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否已在您的存取層級中設定其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先執行下列動作，才可連結[!DNL Workfront]與[!DNL Jira]之間的專案：

* 安裝[!DNL Jira]的[!DNL Workfront]。

  如需指示，請參閱[安裝Jira適用的Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

* 設定Jira的[!DNL Workfront]。

  如需指示，請參閱[設定Jira的Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## 自動將[!DNL Workfront]個專案連結至[!DNL Jira]個問題

作為[!DNL Workfront]管理員，您可以定義觸發器，每次在任務或[!DNL Workfront]中的問題符合特定條件時，這些觸發器都會在[!DNL Jira]中自動建立問題。 Workfront和[!DNL Jira]專案會變成連結。

在您完成Jira的[!DNL Workfront]設定後，在[!DNL Workfront]中建立或更新專案以符合您的觸發程式時，就會在[!DNL Jira]中自動建立新專案。

建立和更新Workfront專案的Workfront使用者不需要[!DNL Jira]授權即可觸發在[!DNL Jira]中建立專案。

如需詳細資訊，請參閱[為Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)設定 [!DNL Adobe Workfront] 。

>[!NOTE]
>
>您可以將範本附加至專案以自動建立[!DNL Jira]專案。 如果範本包含的工作分派符合[!DNL Jira]個觸發程式，則新工作會產生新的[!DNL Jira]個問題。

自動將[!DNL Workfront]問題連結至[!DNL Jira]問題等同於自動將[!DNL Workfront]任務連結至[!DNL Jira]問題。

若要自動將[!DNL Workfront]任務連結至[!DNL Jira]問題：

1. 確保您的[!DNL Jira]系統管理員已設定在指派[!DNL Workfront]專案時自動建立[!DNL Jira]問題的觸發器，然後以可讓您建立任務的存取層級登入[!DNL Workfront]。

   如需存取工作的詳細資訊，請參閱[授與工作存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)。

{{step1-to-projects}}

1. 在&#x200B;**專案**&#x200B;頁面上，選取專案。

1. 在專案左側面板中，選取&#x200B;**[!UICONTROL 任務]**。

1. 按一下&#x200B;**+新工作**。
   >[!NOTE]
   >
   >若要將現有Workfront專案連結至Jira問題，請從專案的&#x200B;**更多** ![更多圖示](assets/more-icon.png)功能表中選取&#x200B;**編輯**。

1. 指定或更新任何可用於任務的欄位。
1. 在&#x200B;**[!UICONTROL 指派]**&#x200B;欄位中，搜尋並選取在[!DNL Jira]整合中指定為觸發器的使用者、角色或團隊。

1. 按一下&#x200B;**建立工作**。 任務已在Workfront中建立，且任務的&#x200B;**更新**&#x200B;標籤中出現新註解，表示已在[!DNL Jira]中建立新問題。

1. （選擇性）在任務或問題標題的&#x200B;**[!UICONTROL 詳細資料]**&#x200B;區段的&#x200B;**[!UICONTROL 整合]**&#x200B;區域中，按一下&#x200B;**[!UICONTROL 前往Jira]**&#x200B;連結以在Jira中開啟問題。

   您的系統或群組管理員必須將[!UICONTROL 整合]欄位新增到您的版面配置範本，才能在任務或問題標題中顯示該欄位。 如需詳細資訊，請參閱[使用配置範本自訂物件標頭](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

   任何[!DNL Jira]使用者都可以立即開始處理從[!DNL Workfront]自動建立的專案，其更新將轉移到[!DNL Workfront]，而不需要[!DNL Workfront]的授權。

   只有您在[!DNL Workfront]附加元件設定期間設定為[!DNL Workfront]管理員的欄位才會更新。

   如需有關在Workfront和Jira之間同步欄位的詳細資訊，請參閱[為Jira設定Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)中的「為Jira設定Adobe Workfront」一節。

   >[!NOTE]
   >
   >從Workfront自動建立[!DNL Jira]問題時，未指派給[!DNL Jira]中的任何人。

## 手動將[!DNL Jira]個問題連結至[!DNL Workfront]個專案

在[!DNL Jira]與[!DNL Workfront]中建立彼此獨立的專案後，您可以手動將[!DNL Jira]問題連結至現有的[!DNL Workfront]任務或問題。

您無法從[!DNL Workfront]手動將[!DNL Workfront]專案連結至現有的[!DNL Jira]專案。

>[!NOTE]
>
>如果[!DNL Jira]問題不在未在[!DNL Workfront]整合中識別為觸發器的專案上，則當您使用與[!DNL Jira]內部部署的整合時，無法手動將其連結至Workfront專案。\
>如需設定Workfront至Jira工作流程觸發器的詳細資訊，請參閱[自動將Workfront專案連結至Jira問題](#automatically-link-workfront-items-to-jira-issues)。

連結[!DNL Workfront]和[!DNL Jira]專案時，其中一個專案的某些欄位會自動更新另一個專案。\
如需有關更新連結專案的詳細資訊，請參閱[更新Jira和Adobe Workfront之間的連結專案](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md)。

若要手動將[!DNL Jira]個問題連結至[!DNL Workfront]個專案：

1. （視條件而定）登入[!DNL Workfront]並尋找您要連結至[!DNL Jira]問題的問題或任務。
1. （視條件而定）在&#x200B;**任務詳細資料**&#x200B;或&#x200B;**問題詳細資料**&#x200B;索引標籤的&#x200B;**基本資訊**&#x200B;區段中，複製Workfront中專案的&#x200B;**[!UICONTROL 參考號碼]**。

   或

   從專案的位址列，複製Workfront中專案的&#x200B;**URL**。

   >[!IMPORTANT]
   >
   >如果您的組織已加入Adobe統一體驗，您必須使用&#x200B;**參考編號**&#x200B;將Workfront專案連結至Jira。 （URL選項可供使用，但如果您使用它，則會傳回錯誤。） 如需Unified Experience的相關資訊，請參閱[Workfront的Adobe Unified Experience ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。
   >
   >對於不在Adobe Unified Experience上的組織，不建議使用URL選項，因為URL可能會變更。

   >[!NOTE]
   >
   >您必須擁有[!DNL Workfront]授權才能登入[!DNL Workfront]。 否則，[!DNL Workfront]使用者必須提供此資訊給您。

1. 在[!DNL Jira]中，瀏覽至您要手動連結至[!DNL Workfront]專案的問題。
1. 在[!DNL Workfront]右側面板中，貼上您要連結它的[!DNL Workfront]專案的&#x200B;**[!UICONTROL 參考號碼]**&#x200B;或&#x200B;**URL**。

1. 按一下&#x200B;**[!UICONTROL 連結]**。 這兩個專案會連結，[!DNL Workfront]右側面板會填入[!DNL Workfront]專案的資訊。

   依預設，下列[!DNL Workfront]欄位會顯示在[!DNL Workfront]右側面板的[!DNL Jira]中：

   * 專案的&#x200B;**[!UICONTROL 名稱]**。 您可以按一下面板中的名稱來存取[!DNL Workfront]專案。
   * **[!UICONTROL 專案名稱]**。
   * 專案的&#x200B;**[!UICONTROL 狀態]**。
   * 專案的&#x200B;**[!UICONTROL 優先順序]**。
   * 建立日期為[!DNL Workfront]。
   * 專案的&#x200B;**[!UICONTROL 計畫時數]**。
   * **[!UICONTROL 參考號碼]**。 您可以按一下面板中的&#x200B;**參考號碼**&#x200B;來存取[!DNL Workfront]專案。

   如需有關啟用其他欄位顯示在右側面板的詳細資訊，請參閱[設定 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)中的[設定[!DNL Jira]與[!DNL Workfront]專案之間的欄位同步]區段。 來自與整合相關聯之[!DNL Workfront]管理員的註解已發佈在[!DNL Jira]問題的&#x200B;**[!DNL Workfront]**&#x200B;標籤中，以確認已建立新的[!DNL Jira]專案。 註解包含[!DNL Jira]問題的連結。

## 取消連結[!DNL Jira]和[!DNL Workfront]之間的專案

在[!DNL Jira]中可以手動取消連結[!DNL Jira]和[!DNL Workfront]之間的連結專案。 您無法從[!DNL Workfront]中相對應的[!DNL Jira]專案取消連結[!DNL Workfront]專案。

您需要以下存取權來取消手動連結的專案的連結：

* 您是手動連結專案的使用者。
* 您是[!DNL Jira]系統管理員。

>[!NOTE]
>
>只有[!DNL Workfront]管理員可以取消連結已自動連結的專案。

若要從[!DNL Workfront]專案取消連結[!DNL Jira]問題：

1. 登入Jira。
1. 導覽至連結至[!DNL Workfront]任務或問題的問題。
1. 前往&#x200B;**Workfront**&#x200B;右側面板。
1. 按一下&#x200B;**[!UICONTROL 取消連結]**&#x200B;圖示，然後按一下&#x200B;**[!UICONTROL 取消連結]**。 先前連結的[!DNL Jira]和[!DNL Workfront]專案已取消連結。

   未來更新的任何欄位、註解或檔案都不會在其他應用程式中更新為先前的對應專案。
