---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront中共用校訂
description: 您可以透過共用檔案或將使用者新增到校訂來在Adobe Workfront中共用校訂檔案。
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: aaf5beb8692b2fdbb797ba908796d78b4ee8866c
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 0%

---

# 在Adobe Workfront中共用校訂

您可以透過共用檔案或將使用者新增到校訂來在Adobe Workfront中共用校訂檔案。

如果您依照本文所述共用校訂，則您的收件者對檔案和校訂具有相同的存取權。 此外，您可以向收件者要求核准證明。

>[!TIP]
>
>您也可以從校訂檢視器共用校訂。 如需指示，請參閱[從校訂檢視器共用校訂](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：選擇或Premium</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣角色</td> 
   <td>作者或版主</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

+++

## 共用校訂連結

共用校訂連結可授予Workfront使用者檢視存取許可權。 使用者可以使用其Workfront登入憑證來評論校訂及訂閱校訂的電子郵件通知。 非校訂使用者可以使用電子郵件地址和顯示名稱進行評論和訂閱。

>[!IMPORTANT]
>
>必須啟用「允許透過公開URL或內嵌程式碼共用校訂」設定。

1. 選取包含您要與使用者共用的校訂的檔案。

   您只能選取一個檔案。 您無法同時共用多個檔案的連結。

1. 按一下&#x200B;**共用** > **校訂連結**。
1. 在出現的&#x200B;**校訂連結**&#x200B;方塊中，執行下列其中一項作業：

   * 若要將連結複製到剪貼簿，請按一下[複製連結]。**&#x200B;**

     您現在可以透過第三方工具（例如聊天或電子郵件應用程式）發佈連結。

   * 若要直接從Adobe Workfront透過電子郵件傳送連結，請執行下列動作：

      1. 在&#x200B;**或電子郵件連結至**&#x200B;欄位中，開始輸入並選取收件者的名稱。 或指定要與其共用的外部使用者的電子郵件地址。

         >[!NOTE]
         >
         >如果您在共用校訂時看到別名電子郵件，請勿在存在對應的別名電子郵件時輸入原始電子郵件來建立新的訪客使用者。

      1. 從下列選項中選取：

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">傳送公開連結</td>
            <td><p>在電子郵件通知中包含一個按鈕，可將使用者導向到他們使用的校訂檢視器內的校訂並授予檢視存取權。</p><p>如果<strong>透過公開URL或內嵌程式碼訂閱校訂</strong>已針對校訂關閉，使用者可以使用其Workfront登入認證登入，以在校訂中加入註解。 如果已開啟，則提供其電子郵件地址和名稱（不需要密碼）的任何人都可以簽署並在校訂中新增註解。</p></td>
           </tr>
           <tr>
            <td role="rowheader">傳送下載連結</td>
            <td>在電子郵件通知中包含一個按鈕，可將使用者引導至下載頁面，其中提供檔案詳細資訊、檔案名稱和檔案大小，並內嵌顯示檔案。 使用者可以從下載頁面按一下下載連結來下載檔案。</td>
           </tr>
           <tr>
            <td role="rowheader">新增自訂訊息</td>
            <td>可讓您指定電子郵件通知的自訂主旨與內文。</td>
           </tr>
          </tbody>
         </table>

      1. 按一下「**傳送**」。

         收件者會收到電子郵件通知，其中包含有關校樣和您選擇加入之按鈕的資訊。

         ![](assets/proof-share-email-350x87.png)

## 將使用者新增到校訂

如果您有校訂的編輯許可權，您可以將任何Workfront使用者新增到校訂中。 如果校訂有多個階段，您可以將使用者新增到個別階段

>[!WARNING]
>
>除了本文中所列的方法之外，還可以在現有校訂的更新索引標籤中的評論中標籤使用者，以將使用者新增到校訂中。 但是，以這種方式新增到校訂的使用者將不會收到電子郵件通知，除非他們在被新增到校訂的工作流程後再次被標籤。
>
>因此，我們建議透過下列其中一種方法將使用者新增到校訂中，而不是在評論中標籤他們。
>

>[!NOTE]
>
>如果您使用舊版Workfront計畫，且其中校訂可為使用者啟用和停用，請記住下列事項：
>
>* 您的收件者不需要啟用校訂即可檢閱校訂。
>* 當啟用自動工作流程且您將使用者新增到Workfront中未啟用校訂的校訂時，會在自動工作流程中建立新階段。 您新增的使用者第一次檢視校訂時，會自動新增到此新階段。 （如需詳細資訊，請參閱[自動化工作流程概觀](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)。）
>

### 從檔案索引標籤新增使用者到現有校訂

1. 選取包含您要新增使用者的校訂的檔案。
1. 如果校訂沒有自動化工作流程（階段），請按一下「階段1」區段右上角的&#x200B;**更多**&#x200B;圖示，然後在下拉式功能表中按一下&#x200B;**共用**。

   或

   如果校訂確實有自動化工作流程，請按一下您想要新增檢閱者之階段右上角的&#x200B;**更多**&#x200B;圖示，然後在下拉式功能表中按一下&#x200B;**共用**。

1. 在出現的&#x200B;**共用此版本**&#x200B;方塊中，在&#x200B;**共用**&#x200B;下，開始輸入您要與其共用校樣的使用者名稱或電子郵件地址，然後在其出現在下拉式清單中時按一下該名稱。

1. （選用）重複此步驟以新增多個使用者至校樣。
1. （選用）設定稽核者的截止日期。
1. （選擇性）如果您想要讓檢閱者知道您已將他們新增至校訂，請確定已選取&#x200B;**透過電子郵件通知人員**。
1. （選擇性） **新增自訂訊息**&#x200B;至電子郵件。
1. 新增所有檢閱者後，請按一下[共用]。**&#x200B;**

### 從校訂檢視器將使用者新增到現有校訂

當您在網路校訂檢視器和案頭校訂檢視器中檢閱校訂時，可以將使用者新增到校訂中。

如需詳細資訊，請參閱文章[從校訂檢視器共用校訂](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)中的[新增使用者以共用校訂](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users)

## 校訂核准報表

您可以建立報告Workfront內共用的校訂核准的報告。 此報表提供您系統中的下列校訂核准資訊：

* 已提交核准的檔案
* 核准者的名稱
* 校訂版本
* 校訂 ID
* 校訂建立日期

您在根據物件建立報告時存取此核准，如[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中所述。

如需校訂核准物件報告的詳細資訊，請參閱[瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[物件報告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects)區段

## 核准共用校訂

當使用者將您新增到校訂並使用Automated Workflow授予核准者角色或檢閱者和核准者角色時，核准請求將顯示在首頁區域的我的核准Widget中。 然後您可以直接從Workfront檢視校樣並對校樣做出核准決定。

如需如何從我的核准Widget做出核准決定的相關資訊，請參閱[從首頁區域核准工作](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area)或[&#128279;](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area)在[核准工作](../../../review-and-approve-work/manage-approvals/approving-work.md)中核准工作。
