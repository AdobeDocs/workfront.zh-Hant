---
filename: change-date-format-chrome
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 變更 [!DNL Adobe Workfront]中日期的格式
description: 若要變更 [!DNL Adobe Workfront] 中日期的日期格式，您必須變更瀏覽器中的語言設定。
feature: Get Started with Workfront
exl-id: 9fac92fb-e3d1-4537-b324-4b35447cef28
source-git-commit: 7ad3fbcfa5be5074016f399560cca509d81f4714
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 變更[!DNL Adobe Workfront]中日期的格式

<!--this article used to be called "Change the date format in Adobe Workfront when using Chrome". The team decieded to make it more generic and hide the steps. Also see drafted content below-->

>[!IMPORTANT]
>
> 本文資訊僅適用於尚未上線到Adobe統一體驗的組織。
> 如果您的組織已加入Adobe統一體驗，您的日期偏好設定由您在Adobe統一命令介面中設定的語言偏好設定控制。 預設語言設定（因此也是預設日期設定）是`en-US`。

您可以在[!DNL Adobe Workfront]中變更日期的日期格式，例如[!UICONTROL 計畫完成日期]、[!UICONTROL 實際完成日期]或[!UICONTROL 預計完成日期]。

例如，您可以將日期格式從&#x200B;_DD/MM/YYYY_&#x200B;變更為&#x200B;_MM/DD/YYYY_，反之亦然。
或者，您可以將日期格式從_MM/DD/YY_&#x200B;變更為&#x200B;_Mon DD， YYYY_。

您可以在Workfront中依下列方式變更日期格式，其方式取決於您要檢視的變更以及您想在何處檢視變更。

* 若要根據您的位置和語言變更[!DNL Workfront]中所有頁面的所有日期格式，您必須變更瀏覽器中的語言設定。

  例如，如果瀏覽器的預設語言設定為&#x200B;*[!UICONTROL 英文（美國）]*，則日期會以下列格式顯示：

   * MM/DD/YYYY
   * YYYY年M月D日

  若要變更[!DNL Chrome]或任何其他瀏覽器的語言設定，您必須修改該瀏覽器的設定。 修改瀏覽器設定的步驟因瀏覽器而異。 請參閱瀏覽器的[!UICONTROL 說明]、[!UICONTROL 偏好設定]或[!UICONTROL 設定]區域，瞭解如何修改其設定。

* 若要只變更報表和檢視中的日期格式，在建立報表或檢視時，您必須更新欄的[!UICONTROL 進階選項]區域中的[!UICONTROL 欄位格式]設定。 這不會根據位置或語言修改日期格式。 它會修改相同位置或語言內容中的日期格式。

  ![](assets/field-format-in-advanced-options-of-a-view-highlighted.png)

  如需詳細資訊，請參閱[建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

* 若要變更整個組織所有外寄電子郵件通知中的日期格式，您必須更新[!UICONTROL 設定]中[!UICONTROL 客戶資訊]區域的[!UICONTROL 預設電子郵件地區設定]設定。

  ![](assets/default-email-locale-field.png)

  如需詳細資訊，請參閱[設定您系統的基本資訊](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

* 若要變更單一使用者所有外寄電子郵件通知中所有日期的格式，編輯使用者設定檔時，您必須更新「[!UICONTROL 編輯人員]」方塊中的「[!UICONTROL 電子郵件地區設定]」設定。

  ![](assets/email-locale-for-user-profile-highlighted.png)

  如需詳細資訊，請參閱[編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

<!--drafted because we should not document steps for a third-party application

To change your language settings in Chrome:

1. Click the 3-dots in the top right corner of your Chrome interface, then click **Settings**.
1. On the left area of the Settings page, expand **Advanced**, then click **Languages**.  
   Or  
   Search for *language*&nbsp;at the top of the Settings page, then click **Languages**.

1. In the **Language** list, locate the language and region that use your preferred date format.

   **Example:** If you speak English and you want the date format to be MM/DD/YYYY, you would select **English (United States)**. If you speak English and you want the date format to be DD/MM/YYY, you would select **English (United Kingdom)**.

1. (Conditional) If the language and region you want to use are not visible in the list, click **Add languages** to add it to the list.
1. Click the 3-dot menu next to the language and region you want to use, then click **Move to the top**.
1. Return to the Workfront interface, then refresh the page.  
   The date format is now updated in projects and other areas of Workfront that use MM/DD/YYYY or DD/MM/YYYY format when displaying dates.

   -->
