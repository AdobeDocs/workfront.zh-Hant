---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront中共用校訂
description: 您可以共用檔案或將使用者新增到校樣中，以在Adobe Workfront中共用校樣檔案。
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 5c0cd18074cffdf0a4fe15affaf61add7314a83a
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 0%

---

# 在Adobe Workfront中共用校訂

您可以共用檔案或將使用者新增到校樣中，以在Adobe Workfront中共用校樣檔案。

如果您共用校訂，如本文所述，您的收件者對檔案和校訂具有相同的存取權。 此外，您可以向收件者要求核准證明。

>[!TIP]
>
>您也可以從校訂檢視器內共用校訂。 如需指示，請參閱 [從校訂檢視器共用校訂](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：選擇或Premium</p> <p>如需有關校訂不同計畫的存取許可權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校樣）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂角色</td> 
   <td>作者或版主</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 共用校訂連結

共用校訂連結可授予Workfront使用者檢視存取許可權。 使用者可以使用其Workfront登入憑證對校訂進行評論並訂閱校訂的電子郵件通知。 非校訂使用者可以使用電子郵件地址和顯示名稱進行評論和訂閱。

>[!IMPORTANT]
>
>必須啟用「允許透過公開URL或內嵌程式碼共用校訂」設定。

1. 選取包含您要與使用者共用的校樣的檔案。

   您只能選取一個檔案。 您無法同時共用多個檔案的連結。

1. 按一下 **共用** > **校訂連結**.
1. 在 **校訂連結** 方塊中，執行下列任一項作業：

   * 若要將連結複製到剪貼簿，請按一下 **複製連結**.

     您現在可以透過第三方工具（例如聊天或電子郵件應用程式）散佈連結。

   * 若要直接從Adobe Workfront透過電子郵件傳送連結，請執行下列動作：

      1. 在 **或以電子郵件傳送連結至** 欄位，開始輸入並選取收件者的名稱。 或指定要與其共用的外部使用者的電子郵件地址。

         >[!NOTE]
         >
         >如果您在共用校樣時看到別名電子郵件，請勿在存在對應的別名電子郵件時輸入原始電子郵件來建立新的訪客使用者。

      1. 從下列選項中選取：

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">傳送公開連結</td>
            <td><p>在電子郵件通知中包含一個按鈕，可將使用者導向到他們使用的校訂檢視器內的校訂並授予檢視存取權。</p><p>若 <strong>透過公開URL或內嵌程式碼訂閱校訂</strong> 已針對校訂關閉，使用者可以使用其Workfront登入憑證登入以在校訂中新增評論。 如果已開啟，則提供其電子郵件地址和名稱（不需要密碼）的任何人都可以簽署並在校樣中新增註解。</p></td>
           </tr>
           <tr>
            <td role="rowheader">傳送下載連結</td>
            <td>在電子郵件通知中包含一個按鈕，可將使用者引導至下載頁面，該頁面提供檔案詳細資訊、檔案名稱和檔案大小，且檔案顯示為內嵌。 使用者可以從下載頁面按一下下載連結來下載檔案。</td>
           </tr>
           <tr>
            <td role="rowheader">新增自訂訊息</td>
            <td>可讓您指定電子郵件通知的自訂主旨和內文。</td>
           </tr>
          </tbody>
         </table>

      1. 按一下 **傳送**.

         收件者會收到電子郵件通知，其中包含有關校樣和您選擇加入之按鈕的資訊。

         ![](assets/proof-share-email-350x87.png)

## 將使用者新增至校訂

如果您有校訂的編輯許可權，可以將任何Workfront使用者新增到校訂中。 如果校訂具有多個階段，您可以將使用者新增到個別階段

>[!WARNING]
>
>除了本文列出的方法外，還可以在現有校訂的更新索引標籤中的評論中標籤使用者，以將使用者新增到校訂中。 但是，以這種方式新增到校樣的使用者將不會收到電子郵件通知，除非他們在被新增到校樣的工作流程後再次被標籤。
>
>因此，我們建議透過下列其中一種方法將使用者新增到校樣中，而不是在評論中標籤他們。
>

>[!NOTE]
>
>如果您使用可為使用者啟用和停用校訂的舊版Workfront計畫，請記住以下事項：
>
>* 您的收件者不需要啟用校樣即可檢閱校樣。
>* 當啟用自動工作流程且您將使用者新增到校訂時，未在Workfront中啟用校訂，新的階段會在自動工作流程中建立。 您新增的使用者第一次檢視校訂時，會自動新增到此新階段。 (如需詳細資訊，請參閱 [自動化工作流程總覽](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>

### 從檔案索引標籤新增使用者到現有校訂

1. 選取包含您要新增使用者的校訂的檔案。
1. 如果校樣沒有自動化工作流程（階段），請按一下 **更多** 圖示加以檢視，然後按一下 **共用** （在下拉式功能表中）。

   或

   如果校樣確實有自動化工作流程，請按一下 **更多** 圖示並按一下「 」，此圖示位於您想要新增稽核者的舞台右上角 **共用** （在下拉式功能表中）。

1. 在 **共用此版本** 方塊，位於 **共用**，開始輸入您要與其共用校訂之使用者的名稱或電子郵件地址，然後在其出現在下拉式清單中時按一下該名稱。

1. （可選）重複此步驟以新增多個使用者至校樣。
1. （選用）設定稽核者的截止日期。
1. （可選）請確定 **透過電子郵件通知人員** 如果要讓稽核者知道您已將其新增到校樣中，請選取。
1. （可選） **新增自訂訊息** 至電子郵件。
1. 新增所有稽核者後，按一下 **共用**.

### 從校訂檢視器將使用者新增到現有校訂

當您在網頁校訂檢視器和案頭校訂檢視器中檢閱校訂時，可以將使用者新增到校訂中。

如需詳細資訊，請參閱 [新增使用者以共用校訂](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) 在文章中 [從校訂檢視器共用校訂](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## 校訂核准報告

您可以建立報告Workfront內已共用的校訂核准的報告。 此報表提供您系統中的下列校訂核准資訊：

* 已提交供核准的檔案
* 核准者的名稱
* 校訂版本
* 校訂 ID
* 校訂建立日期

當您根據物件建立報告時，可存取此核准，如所述 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

如需校訂核准物件報告的詳細資訊，請參閱 [物件報告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 中的區段 [瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## 核准共用校訂

當使用者將您新增到校樣並使用Automated Workflow授予核准者角色或檢視者和核准者角色時，核准請求將顯示在您的「首頁」或「我的工作」區域的「核准」索引標籤上。 然後，您可以直接從Workfront檢視校樣並對校樣做出核准決定。

如需如何從「我的工作」區域做出核准決定的相關資訊，請參閱 [核准來自首頁區域的工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) 或 [核准工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) 在 [核准工作](../../../review-and-approve-work/manage-approvals/approving-work.md).
