---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: 排程自動報表傳送
description: 排程自動報表傳送
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 2%

---

# 排程自動報表傳送

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

您可以排程報表，以依定義的排程自動傳送給使用者，或者也可以一次手動傳送報表。 從Adobe Workfront傳送報表時，使用者會收到另一個附件中含有Workfront報表的電子郵件。

如需詳細資訊，包括可能影響報表傳送的大小限制，請參閱 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，您必須建立報表。 若要進一步了解建立報表，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 排程報表傳送

若要排程報表自動傳送，或編輯或刪除現有的報表傳送： &#x200B;

1. 前往您要排程傳送的報表。

   >[!NOTE]
   >
   >報表傳送不包含提示。 如果您想要限制報表傳送中的資料，建議您將篩選套用至您要傳送的報表。

1. 按一下 **報表動作**，然後 **傳送報表**.

   此 **傳送報表** 對話框。

   >[!TIP]
   >
   >若要在任何指定時間手動傳送報表，請前往報表，然後按一下 **報表動作** > **傳送報表** > **立即發送**.

1. 選取 **重複傳送** 標籤。
1. （條件性）若要修改現有的重複報表傳送，請在 **重複傳送** 區段。
1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>傳送至</p> </td> 
      <td> <p>開始鍵入要將報告發送到的用戶、組、團隊或角色的名稱，然後在下拉清單中顯示該名稱時按一下。</p> <p>或</p> <p>指定您要存取報表之Workfront系統外部人員的電子郵件地址。</p> <p>重複此程式，將報表傳送給多個使用者、群組、團隊或角色。</p> <p>備註:  <p>新增報表傳送收件者時，請考量下列事項：</p> 
        <ul> 
         <li>如果貴組織將Workfront通知限制在特定電子郵件網域，則您只能將報表傳送至電子郵件允許清單中所列的電子郵件地址。<p>如需Workfront管理員如何更新電子郵件允許清單的詳細資訊，請參閱 <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">設定您的電子郵件允許清單</a>.</p></li> 
         <li> <p>將大量使用者新增為收件者，可能會導致傳送失敗。 如果您遇到傳送失敗的情況，您可以與較小的使用者群組一起排程多個報表傳送。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>電子郵件主題</p> </td> 
      <td> <p>指定電子郵件通知的主旨。</p> <p>依預設，電子郵件主旨為：</p> <p><em>Workfront報告：[報表名稱] [日期]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>電子郵件訊息</p> </td> 
      <td> <p>指定要包含在電子郵件中的訊息。</p> <p>依預設，電子郵件訊息為：</p> <p><em>附加的是Workfront在[Date]時產生的[報表頻率]報表[報表名稱]。</em> </p> <p>注意：僅以Excel檔案傳送的報表，也會在電子郵件中新增下列訊息：「請注意，若使用MS Excel(XLS)檔案類型，這些檔案類型支援的超連結數量會有限制(65,530)。 如果超過這些限制，您的檔案將不會開啟，建議您在沒有超連結的情況下重新傳送。 請返回報表排程器，移除超連結並重新傳送報表。」 「請返回報表排程器」片語是回報表的連結。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>以下內容提供此報表：</p> </td> 
      <td> <p>開始輸入有權存取報表的使用者名稱，然後在下拉式清單中出現時按一下名稱。 接收報表的使用者將獲得與您在此處指定之使用者相同的報表存取層級。<br> 如需詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">使用其他使用者的存取權限執行並傳送報表</a>.</p> <p>注意：此欄位不支援萬用字元。 例如，使用萬用字元$$User.ID時，不會執行具有接收報表之使用者存取權限的報表。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>格式</p> </td> 
      <td> <p>選取要傳送報表的格式：</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>如果您選取此選項，則可使用其他 <strong>紙張大小</strong> 和 <strong>方向</strong> 選項。</p> </li> 
        <li> <p>MS Excel(.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>包括連結</p> </td> 
      <td> <p>此選項僅在 <strong>MS Excel</strong> 在 <strong>格式</strong> 下拉式功能表。 啟用此選項時，匯出的Excel檔案中會包含任何超連結。</p> <p>包含65,530個以上連結的文檔無法開啟。 如果導出的文檔將包含65,530個以上的連結，請取消選擇此選項。</p> <p>預設會啟用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>摘要</p> </td> 
      <td> <p>顯示重複傳送時間的摘要。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重覆</p> </td> 
      <td> <p>選取報表應以每日、每週、每月或每年傳送。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重覆於每</p> </td> 
      <td> <p>選取您要傳送重複的頻率。 您為此選項選取的值是以 <strong>重複</strong> 下拉式清單。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>時間</p> </td> 
      <td> <p>選取要傳送的傳送時間。</p> <p>提示：由於系統載入可能會影響報表傳送時間，因此排程時間與實際傳送時間之間可能會有延遲。 如果您需要在特定時間傳送報表，建議您在需要傳送之前排程傳送。 例如，建議將傳送排程在需要的日期之前。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>重覆於</p> </td> 
      <td> <p>此選項可在 <strong>重複</strong> 選項設為 <strong>每週</strong> 或 <strong>每月</strong>:</p> 
       <ul> 
        <li> <p>當 <strong>重複</strong> 選項設為 <strong>每週</strong>:選取傳送的一週天數。</p> </li> 
        <li> <p>當 <strong>重複</strong> 選項設為 <strong>每月</strong>:選取傳送是在月份的某天、一週中的某天，還是當月的最後一天(這些選項會運用您在 <strong>開始於</strong> 欄位)。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>開始於</p> </td> 
      <td>選取排程傳送的開始日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>結束日期</p> </td> 
      <td>選取排程傳送要結束的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>絕不</p> </td> 
      <td>選擇 <strong>從不</strong> 如果您希望排程傳送無限期持續。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **儲存** 儲存報表傳送。

   報表會顯示在 **重複傳送** 區段(在 **傳送報表** 對話方塊)，且會在排程時間傳送。

   如需影響報表傳送之大小限制的相關資訊，請參閱區段 [報表傳送限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) 和 [匯出限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. （選用）若要刪除排程的傳送：

   1. 在 **重複傳送** 面板，按一下排程傳送，然後按一下 **刪除**.
   1. 按一下 **刪除** 確認。

## 影片逐步說明

觀看下列影片，了解如何排程報表傳送。 此影片已在Workfront Classic中錄制。 不過，內容也適用於新的Workfront體驗。

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
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
