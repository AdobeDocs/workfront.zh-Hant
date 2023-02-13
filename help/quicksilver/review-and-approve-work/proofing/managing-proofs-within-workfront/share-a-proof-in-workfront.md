---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront內共用證明
description: 您可以在Adobe Workfront中共用已校樣的檔案，方法是共用檔案或將使用者新增至校樣。
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# 在Adobe Workfront內共用證明

您可以在Adobe Workfront中共用已校樣的檔案，方法是共用檔案或將使用者新增至校樣。

如果您共用校樣（如本文所述），則收件者對檔案和校樣有相同的存取權。 此外，您也可以向收件者要求校樣的核准。

>[!TIP]
>
>您也可以從校對檢視器內共用校樣。 如需指示，請參閱 [從校對檢視器共用校樣](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Select或Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>管理員或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">證明角色</td> 
   <td>作者或協調者</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 共用校樣連結

共用證明連結可授予Workfront使用者檢視存取權。 使用者可以使用其Workfront登入憑證，對校樣加上註解，並訂閱校樣的電子郵件通知。 非校對的使用者可以使用電子郵件地址和顯示名稱來留言和訂閱。

>[!IMPORTANT]
>
>必須啟用「允許透過公用URL或內嵌程式碼共用校樣」設定。

1. 選擇包含要與用戶共用的校樣的文檔。

   只能選擇一個文檔。 不能同時共用多個文檔的連結。

1. 按一下 **共用** > **校樣連結**.
1. 在 **校樣連結** 框中，執行下列任一操作：

   * 若要將連結複製到剪貼簿，請按一下 **複製連結**.

      您現在可以透過協力廠商工具（例如聊天或電子郵件應用程式）來分發連結。

   * 若要直接從Adobe Workfront以電子郵件傳送連結，請執行下列動作：

      1. 在 **或以電子郵件連結至** 欄位，開始輸入並選取收件者的名稱。 或指定您要共用之外部使用者的電子郵件地址。

         >[!NOTE]
         >
         >如果您在共用校樣時看到別名電子郵件，如果相應的別名電子郵件存在，則不要輸入原始電子郵件來建立新的來賓用戶。

      1. 從下列選項中選取：

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">傳送公開連結</td>
            <td><p>在電子郵件通知中包含一個按鈕，可將使用者引導至其使用的校對檢視器內的校樣，並授予檢視存取權。</p><p>若 <strong>透過公開URL或內嵌程式碼訂閱校樣</strong> 為了校樣而關閉，使用者可以使用其Workfront登入憑證登入，以為校樣新增註解。 如果開啟，則提供其電子郵件地址和名稱（無需密碼）的任何人都可以簽名，並在校樣中添加註釋。</p></td>
           </tr>
           <tr>
            <td role="rowheader">傳送下載連結</td>
            <td>在電子郵件通知中包含一個按鈕，可將使用者引導至下載頁面，該頁面提供檔案詳細資訊、檔案名稱和檔案大小，並內嵌顯示檔案。 使用者可以按一下下載頁面中的下載連結來下載檔案。</td>
           </tr>
           <tr>
            <td role="rowheader">新增自訂訊息</td>
            <td>可讓您指定電子郵件通知的自訂主旨和內文。</td>
           </tr>
          </tbody>
         </table>

      1. 按一下 **傳送**.

         您的收件者會收到電子郵件通知，其中包含您選擇加入的校樣和按鈕的相關資訊。

         ![](assets/proof-share-email-350x87.png)

## 新增使用者至校樣

如果您對校樣具有「編輯」權限，則可將任何Workfront使用者新增至校樣。 如果校樣有多個階段，您會將使用者新增至個別階段

>[!NOTE]
>
>如果您使用舊版Workfront計畫，可為使用者啟用和停用校對功能，請記住下列事項：
>
>* 收件者不需要啟用校樣即可檢閱校樣。
>* 啟用「自動化工作流程」且您新增使用者至未在Workfront中啟用校樣的校樣時，「自動化工作流程」中會建立新階段。 當您新增的使用者第一次檢視校樣時，就會自動新增至此新階段。 (如需詳細資訊，請參閱 [自動化工作流程概觀](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>


### 從「文檔」頁簽將用戶添加到現有校樣

1. 選擇包含要添加用戶的校樣的文檔。
1. 如果校樣沒有自動化的工作流程（階段），請按一下 **更多** 表徵圖，然後按一下 **共用** 的下拉式清單。

   或

   如果校樣確實有「自動化工作流程」，請按一下 **更多** 表徵圖，在要添加審核者的舞台右上角，按一下 **共用** 的下拉式清單。

1. 在 **共用此版本** 框，位於 **共用**，開始輸入您要共用校樣的使用者的名稱或電子郵件地址，然後在下拉式清單中出現時按一下名稱。

1. （選用）重複此步驟，將多個使用者新增至校樣。
1. （可選）為審核者設定最後期限。
1. （選用）請確定 **通過電子郵件通知人** 如果您想讓審核者知道您已將其新增至校樣，則會選取此選項。
1. （可選） **新增自訂訊息** 到電子郵件。
1. 添加所有審閱者後，按一下 **共用**.

### 從校對檢視器將使用者新增至現有校樣

您可以在Web校對檢視器和案頭校對檢視器中檢閱校樣時，將使用者新增至校樣。

如需詳細資訊，請參閱 [新增使用者以共用校樣](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) 在文章中 [從校對檢視器共用校樣](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## 校對核准報告

您可以建立報告，報告已在Workfront內共用的校對核准。 此報表在您的系統中提供下列證明核准資訊：

* 已提交供批准的文檔
* 核准者的名稱
* 校樣版本
* 校訂 ID
* 校樣建立日期

根據對象建立報表時，可以訪問此批准，如 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

如需「校樣核准」物件報表的詳細資訊，請參閱 [對象報告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 區段 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## 核准共用校樣

當用戶將您添加到校樣，並使用「自動化工作流」授予「批准者」角色或「審核者和批准者」角色時，「首頁」或「我的工作」區域的「批准」頁簽上會顯示批准請求。 然後，您就可以直接從Workfront檢視證明，並對證明做出核准決定。

有關如何從「我的工作」區域做出審批決策的資訊，請參閱 [從首頁批准工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) 或 [核准工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) in [核准工作](../../../review-and-approve-work/manage-approvals/approving-work.md).
