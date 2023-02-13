---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 在控制面板中內嵌外部網頁
description: 您可以在控制面板中嵌入外部網頁，以便從Adobe Workfront內的其他系統或其他Workfront頁面存取相關資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# 在控制面板中內嵌外部網頁

您可以在控制面板中嵌入外部網頁，以便從Adobe Workfront內的其他系統或其他Workfront頁面存取相關資訊。

例如，如果您的組織有網頁型檔案存放庫、Wiki或其他內容管理系統，其中包含經常透過URL存取的專案資訊，您可以在控制面板上建立外部頁面，將該資訊顯示至Workfront。

>[!IMPORTANT]
>
>基於安全考量，有些網站不允許您將網頁內嵌為iframe。 如果您要內嵌在控制面板中的網頁不允許此動作，該頁面不會顯示在控制面板中。 不過，您仍可以按一下控制面板的名稱來存取外部頁面。\
>![](assets/qs-empty-external-page-report-350x165.png)\
>若要允許內嵌您擁有的網站，請與網頁管理員合作調整 **X-Frame-Options** 設定。 如需詳細資訊，請參閱 [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對報表、控制面板和日曆的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>管理控制面板的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先建立控制面板，才能將外部頁面嵌入其中。

如需建立控制面板的詳細資訊，請參閱 [建立控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## 在控制面板中內嵌外部頁面

>[!IMPORTANT]
>
>如果不再需要外部頁面，您可以從控制面板中移除該頁面。 不過，在Workfront中建立外部頁面後，您就無法刪除該頁面。 您只能使用API刪除外部頁面。 如需詳細資訊，請參閱 [從控制面板移除外部頁面](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. 找出要在Workfront中顯示的頁面URL，並複製位於位址列的URL。

   >[!NOTE]
   >
   >如果您要與Workfront物件共用URL，請記住，有些URL會隨著時間而過期。 例如，檔案URL在開啟後就會過期。 這會設定為安全措施，且根據設計，這些URL會視為非靜態URL，因此不應共用。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下 **控制面板**.

1. 若要編輯現有的控制面板，請選取您要內嵌網站頁面的控制面板，然後按一下 **控制面板動作**，然後選取 **編輯** 的上界。\
   或\
   若要建立新控制面板，請按一下 **新控制面板**.\
   如需建立控制面板的詳細資訊，請參閱 [建立控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. 按一下 **新增外部頁面**.

   ![](assets/qs-add-external-page-350x239.png)

1. 指定 **名稱** （外部頁面）。
1. 指定 **說明**.
1. 將您先前複製的URL貼入 **URL** 欄位。\
   您可以指定下列URL類型：

   * 網頁的https（加密）URL。\
      URL只會載入https（加密）頁面。\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * 包含特定網站之工作階段資訊的範本URL。\
      例如： *https://localhost/?session=$$SESSION}*
您必須登入指定的網站才會顯示外部頁面。\
      如需如何從Workfront取得SessionID的相關資訊，請參閱 [API基本介紹](../../../wf-api/general/api-basics.md).\
      出於安全原因，Workfront管理員可能會以不允許在外部頁面中使用工作階段資訊的方式來設定您的系統偏好設定。 在此情況下，控制面板上不會載入外部頁面。\
      有關係統安全首選項的詳細資訊，請參見 [配置系統安全首選項](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. 按一下&#x200B;**儲存**。\
   頁面會自動新增至控制面板。 如果已建立未來的控制面板，則可新增外部頁面。 外部頁面將可在「可用報表」中找到。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## 更新控制面板中的外部頁面

若要更新控制面板中使用之外部頁面的資訊：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下 **控制面板**.
1. 選取您要更新的控制面板，然後按一下 **編輯** ![](assets/edit-icon.png).

   ![選取「編輯」圖示。](assets/nwe-editdashboard2021-350x188.png)

1. 在畫面右側，找出您要更新的外部頁面，然後按一下 **編輯** 表徵圖。\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. 在 **編輯外部頁面** 對話框，更新要更改的欄位，然後按一下 **儲存**.
1. （選用）按一下 **刪除** 圖示 ![](assets/delete.png) 從控制面板移除外部頁面。 如需詳細資訊，請參閱 [從控制面板移除外部頁面](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. 在左下角，按一下 **儲存+關閉**.

## 在報表中檢視外部頁面

您可以在「外部頁面」報表中檢視Workfront中的所有外部頁面。

1. 前往 **主菜單** 圖示 ![](assets/main-menu-icon.png) > **報表**.
1. 按一下 **新增報表** >選取 **外部頁面**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. （可選）更新報表的「檢視」、「篩選」或「群組」標籤。

   如需詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 按一下 **儲存並關閉**.

   您可以在新報表中檢視與系統外部頁面相關聯的名稱和URL。

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
