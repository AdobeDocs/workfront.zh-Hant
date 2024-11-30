---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: 排程自動報告傳送
description: 排程自動報告傳送
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '1197'
ht-degree: 2%

---

# 排程自動報告傳送

<!-- Audited: 11/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

您可以排程報表，以按照定義的排程自動傳送給使用者，或者也可以手動傳送一次性報表。 當您從Adobe Workfront傳送報告時，使用者會收到一封電子郵件，其中包含個別附件中的Workfront報告。

如需詳細資訊，包括可能影響報表傳送的大小限制，請參閱[報表傳送概覽](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
      <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須建立報表。 若要進一步瞭解如何建立報告，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 排程報表傳送

若要排程報表自動傳送，或編輯或刪除現有的報表傳送，請執行下列步&#x200B;驟：

1. 移至您要排程傳送的報告。

   >[!NOTE]
   >
   >報告傳送不包含提示。 如果您想要限制報告傳送中的資料，我們建議您將篩選器套用至您要傳送的報告。

1. 按一下&#x200B;**報告動作**，然後按一下&#x200B;**傳送報告**。

   顯示&#x200B;**傳送報告**&#x200B;對話方塊。

   >[!TIP]
   >
   >若要在指定時間手動傳送報告，請移至報告，然後按一下&#x200B;**報告動作** > **傳送報告** > **立即傳送**。

1. 選取&#x200B;**重複傳遞**&#x200B;索引標籤。
1. （視條件而定）若要修改現有的重複報告傳遞，請在&#x200B;**重複傳遞**&#x200B;區段中選取報告傳遞。
1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>傳送至</p> </td> 
      <td> <p>開始輸入您要傳送報告的目標使用者、群組、團隊或角色的名稱，然後當名稱出現在下拉式清單中時按一下該名稱。</p> <p>或</p> <p>指定您希望存取報表的Workfront系統外部人員電子郵件地址。</p> <p>重複此程式，將報告傳送給多個使用者、群組、團隊或角色。</p> <p>注意：  <p>新增報告傳送收件者時，請考量下列事項：</p> 
        <ul> 
         <li>如果貴組織將Workfront通知限制在特定電子郵件網域，您只能將報告傳送至電子郵件允許清單中列出的電子郵件地址。<p>如需Workfront管理員如何更新電子郵件允許清單的詳細資訊，請參閱<a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">設定您的電子郵件允許清單</a>區段。</p></li> 
         <li> <p>將大量使用者新增為收件者可能會導致傳遞失敗。 如果您遇到傳送失敗，您可以以較小的使用者群組排程多個報表傳送。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>電子郵件主題</p> </td> 
      <td> <p>指定電子郵件通知的主旨。</p> <p>依預設，電子郵件主旨為：</p> <p><em>Workfront報告： [報告名稱] [日期]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>電子郵件訊息</p> </td> 
      <td> <p>指定要包含在電子郵件中的訊息。</p> <p>依預設，電子郵件訊息為：</p> <p><em>附加是Workfront於[日期].</em>產生的[報告頻率]報告[報告名稱] </p> <p>注意：僅針對以Excel檔案傳送的報表，也會在電子郵件中新增下列訊息：「請注意，若使用MS Excel (XLS)檔案型別，這些檔案型別支援的超連結會有數量限制(65,530)。 如果超過這些限制，您的檔案將無法開啟，建議您在不使用超連結的情況下重新傳送。 請返回報告排程器，移除超連結並重新傳送報告。」 「請回到報告排程器」片語是回到報告的連結。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>提供此報告並具備以下存取許可權：</p> </td> 
      <td> <p>開始輸入可存取報表的使用者名稱，然後在名稱出現在下拉式清單中時按一下名稱。 收到報表的使用者將被授予與您在此指定的使用者相同層級的報表存取權。<br>如需詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">使用其他使用者的存取權執行並傳遞報告</a>。</p> <p>注意：此欄位不支援萬用字元。 例如，使用萬用字元$$User.ID不會以接收報表之使用者的存取許可權執行報表。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>格式</p> </td> 
      <td> <p>選取您要用於傳送報表的格式：</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>如果選取此專案，您可以使用額外顯示的<strong>紙張大小</strong>和<strong>方向</strong>選項來格式化輸出。</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>包括連結</p> </td> 
      <td> <p>只有在<strong>格式</strong>下拉式功能表中選取<strong>MS Excel</strong>時，才能使用此選項。 啟用此選項後，所有超連結都會包含在匯出的Excel檔案中。</p> <p>無法開啟包含超過65,530個連結的檔案。 如果匯出的檔案包含超過65,530個連結，請取消選取此選項。</p> <p>此選項預設為啟用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>摘要</p> </td> 
      <td> <p>顯示傳遞重複時間的摘要。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重覆</p> </td> 
      <td> <p>選取報表應每日傳送、每週傳送、每月傳送或每年傳送。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重覆於每</p> </td> 
      <td> <p>選取您要重複傳送的頻率。 您為此選項選取的值是根據<strong>重複</strong>下拉式清單中選取的選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>時間</p> </td> 
      <td> <p>選取一天中要傳送傳遞的時間。</p> <p>提示：由於系統載入會影響報表傳送時間，因此排程時間與實際傳送時間之間最多可能有24小時的延遲。 如果您需要在特定時間之前傳送報表，建議在需要的時間之前排程傳送。 一般而言，我們建議將傳送排程至少早於所需日期一天。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重覆於</p> </td> 
      <td> <p>當<strong>重複</strong>選項設定為<strong>每週</strong>或<strong>每月</strong>時，此選項可供使用：</p> 
       <ul> 
        <li> <p>當<strong>重複</strong>選項設定為<strong>每週</strong>時：選取傳送的星期幾。</p> </li> 
        <li> <p>當<strong>重複</strong>選項設為<strong>每月</strong>：選取傳送是在當月、當週或當月最後一天進行（這些選項會運用您在<strong>開始於</strong>欄位中選取的日期）。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>開始於</p> </td> 
      <td>選取排程傳遞的開始日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>結束日期</p> </td> 
      <td>選取排程傳遞的結束日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>絕不</p> </td> 
      <td>若要讓排程的傳遞無限期持續，請選取<strong>永不</strong>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**&#x200B;以儲存報告傳遞。

   報告會顯示在&#x200B;**重複傳遞**&#x200B;區段（在&#x200B;**傳送報告**&#x200B;對話方塊中）中，並將於排程時間傳送。

   如需可能影響報表傳送之大小限制的相關資訊，請參閱[報表傳送限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits)與[匯出限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export)小節。

>[!IMPORTANT]
>
>處理排程報表以進行傳送時，受內部時間限制。 如果報告花費的時間超過傳送限制，您將收到通知，且無論剩餘的任何排程傳送，都將不再傳送報告。 若要繼續傳送報告，請先嘗試透過篩選器和檢視縮小報告大小，然後建立新的排程傳送。
>
>如果您使用排程報表傳送來透過BI工具分析Workfront資料，建議您改用Workfront Data Connect 。 如需詳細資訊，請參閱[Workfront Data Connect總覽](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md)。

1. （選擇性）若要刪除排程的傳送：

   1. 在&#x200B;**重複傳遞**&#x200B;面板中，按一下排定的傳遞，然後按一下&#x200B;**刪除**。
   1. 按一下&#x200B;**刪除**&#x200B;確認。

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
