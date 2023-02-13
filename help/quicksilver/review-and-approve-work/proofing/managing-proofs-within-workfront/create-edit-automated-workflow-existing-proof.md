---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 為現有校樣建立或編輯自動化工作流程
description: 如果您的流程複雜，或您定期將內容傳送給相同的人員群組進行審核，自動化工作流程可讓您更輕鬆地管理審核流程。 當您使用自動化工作流程建立校樣時，校樣會從階段移至階段，直到最終核准。 當參與者需要審閱該文檔時，將通知他們。
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 0%

---

# 為現有校樣建立或編輯自動化工作流程

如果您的流程複雜，或您定期將內容傳送給相同的人員群組進行審核，自動化工作流程可讓您更輕鬆地管理審核流程。 當您使用自動化工作流程建立校樣時，校樣會從階段移至階段，直到最終核准。 當參與者需要審閱該文檔時，將通知他們。

如需建立新校樣自動化工作流程的相關資訊，請參閱 [使用自動化工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 為現有校樣建立或編輯自動化工作流程：

1. 將滑鼠指標暫留在「檔案」區域的檔案上，然後按一下「校對工作流程」。

   或

   如果您正在校對檢視器中檢閱校樣，請按一下 **工作流程** ![](assets/workflow-icon-proofing-viewer.png) 在左側面板中，按一下「編輯」圖示 ![](assets/edit-icon-proofing-viewer.png) 以開啟校樣的「自動化工作流程」設定。

1. （條件性）如果校樣目前使用基本工作流程（沒有階段），請按一下 **轉換為自動化工作流程** 在畫面中顯示。

   >[!NOTE]
   >
   >從基本工作流轉換為自動工作流時無法編輯第一個階段，但可以添加和配置新階段。

1. 條件性)若要使用您的Adobe Workfront管理員建立並與您共用的「自動化工作流程」範本，請按一下 **新增範本**，在出現的方塊中選取範本，然後按一下 **新增範本**.

   如需詳細資訊，請參閱 [關於使用自動化工作流模板](#about-using-automated-workflow-templates) 這篇文章。

1. 將階段新增至自動化工作流程：

   1. 按一下 **新階段** 在右上角。
   1. 在顯示的方塊中，輸入 **名稱** 為了舞台。
   1. （可選）設定階段的截止時間。
   1. 在 **啟動階段** 部分，選擇要如何激活舞台：


      <table>
      <tbody>
      <tr>
      <td><strong>論校樣建立</strong></td>
      <td>由於校樣已建立，舞台自動變為活動狀態。</td>
      </tr>
      <tr>
      <td><strong>當前階段的截止期超過</strong></td>
      <td>按一下 <strong>父階段</strong> 下拉式清單。</td>
      </tr>
      <tr>
      <td><strong>在特定日期和時間</strong></td>
      <td>按一下 <strong>開啟</strong> 方塊以選取日期，然後按一下右側的方塊以選取時間。</td>
      </tr>
      <tr>
      <td><strong>所有決策均為「已核准」或「已核准」，且父級階段有所變更</strong></td>
      <td>按一下 <strong>父階段</strong> 下拉式清單。</td>
      </tr>
      <tr>
      <td><strong>所有決策在父級階段都經過核准</strong></td>
      <td>按一下 <strong>父階段</strong> 下拉式清單。</td>
      </tr>
      <tr>
      <td><strong>所有決定都是</strong></td>
      <td>按一下 <strong>父階段</strong> 下拉式清單。</td>
      </tr>
      </tbody>
      </table>


   1. 輸入聯繫人姓名或電子郵件地址，並為舞台的審閱者配置設定。

      有關添加審核者的資訊，請參閱 [關於將審核者添加到舞台](#about-adding-reviewers-to-a-stage) 這篇文章。

   1. 使用下列任一選項來進一步配置階段：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>期限選項</strong> </td>
         <td><p>若要設定階段的截止時間，請按一下 <strong>期限選項</strong> 下拉式清單。 然後，在 <strong>截止時間</strong>，執行下列其中一項操作：</p>
          <ul>
           <li>如果您選擇 <strong>設定特定日期</strong>:選擇所需的截止日期和時間。</li>
           <li>如果您選擇 <strong>從階段激活日期計算</strong>:選擇要添加到階段激活日期的工作天數，以確定截止日期。</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">鎖台</td>
         <td>指定何時可以鎖定舞台。 </td>
        </tr>
        <tr>
         <td role="rowheader">主要決策進行者</td>
         <td><p>在舞台上選擇主決策者（僅在向舞台上添加至少一個具有「批准者」或更高「證明」角色的人員後可用）。 如果選擇主決策者，則 <strong>只需一個決定</strong> 選項。</p></td>
        </tr>
        <tr>
         <td role="rowheader">只需要一個決定</td>
         <td>當某個決策者做出決策時，結束整個審查過程。<p>如果您在 <strong>主要決策者</strong> 下拉式功能表。</p></td>
        </tr>
        <tr>
         <td role="rowheader">私人舞台</td>
         <td>僅允許以下人員查看此階段中做出的評論和決策：監事、Adobe Workfront管理員和Workfront Proof管理員</td>
        </tr>
        <tr>
         <td role="rowheader">通過電子郵件通知人</td>
         <td>輪到審核人員處理校樣時，向審核人員發出電子郵件通知。</td>
        </tr>
       </tbody>
      </table>

   1. 按一下 **添加階段**.

1. 視需要重複上一步，以新增更多階段。

   將階段新增至自動化工作流程時，畫面上會顯示圖表，以表示這些階段：

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. 完成添加階段後，按一下 **完成**.

## 關於使用自動化工作流模板 {#about-using-automated-workflow-templates}

使用「自動化工作流程」範本時，請考量下列事項：

1. 「自動化工作流程」範本的設定決定了您可以對「自動化工作流程」執行哪些校樣。 例如，如果在範本中停用了「新增階段」按鈕，當您使用校樣的「自動化工作流程」設定時，該按鈕將不會顯示。
1. 將人員添加到「自動化工作流」模板中的某個頁面，但同時已作為校樣的審閱者出現時，應用模板會將審閱者從舞台中刪除。 如果您未將另一個審核者添加到舞台，則會出現一條消息提示您添加一個審核者。
1. 您修改「自動化工作流程」範本的能力取決於Workfront管理員所設定的範本設定，如中所述。 如果禁用了修改模板的功能，則只有模板的所有者才能修改它。

## 關於將審核者添加到舞台 {#about-adding-reviewers-to-a-stage}

將審核者添加到階段時，請考慮以下事項：

* 將使用者新增到舞台後，您可以設定該使用者的校樣設定，例如校樣角色和他們應該擁有的任何其他權限，以及當人們對校樣發表意見和做出決策時，他們將收到的電子郵件警報類型。
* 您可以將一或多個使用者從一個階段拖曳至另一個階段。 您可以直接將使用者拖曳至另一個階段，或將使用者拖曳至 **階段** 圖表。 要選擇多個用戶，請按Shift + Ctrl（在Windows上）或Shift + Command(在Mac上)。
* 只能將審核者添加到校樣一次，這意味著您不能將同一人添加到校樣的多個階段。
* 未添加到私人舞台的審閱者無法看到該舞台上在該舞台上所做的校樣或評論。
* 依預設，將使用者新增至階段會授予使用者從建立校樣開始即可檢視校樣的存取權。

   您的Workfront管理員可以限制使用者存取校樣，直到工作流程進入新增使用者的階段為止。 如需詳細資訊，請參閱中的。
