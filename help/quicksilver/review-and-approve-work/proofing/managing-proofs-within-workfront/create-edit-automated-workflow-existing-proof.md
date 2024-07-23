---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 建立或編輯現有校訂的自動化工作流程
description: 如果您的程式複雜或您定期傳送內容給相同的人員群組進行稽核，自動化工作流程可讓您更輕鬆地管理稽核流程。 使用自動化工作流程建立校訂時，校訂會從不同階段移至不同階段，直到最終核准為止。 輪到參與者檢閱檔案時，會通知他們。
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# 建立或編輯現有校訂的自動化工作流程

如果您的程式複雜或您定期傳送內容給相同的人員群組進行稽核，自動化工作流程可讓您更輕鬆地管理稽核流程。 使用自動化工作流程建立校訂時，校訂會從不同階段移至不同階段，直到最終核准為止。 輪到參與者檢閱檔案時，會通知他們。

如需有關為新校訂建立自動化工作流程的資訊，請參閱[使用自動化工作流程建立進階校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：Premium</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

+++

## 建立或編輯現有校訂的自動化工作流程：

1. 將滑鼠懸停在「檔案」區域中的檔案上，然後按一下「校訂工作流程」。

   或

   如果您正在校訂檢視器中檢閱校訂，請按一下左側面板中的&#x200B;**工作流程** ![](assets/workflow-icon-proofing-viewer.png)，然後按一下「編輯」圖示![](assets/edit-icon-proofing-viewer.png)以開啟校訂的自動工作流程設定。

1. （視條件而定）如果校訂目前使用基本工作流程（沒有分段），請在顯示的畫面中按一下&#x200B;**「轉換為自動化工作流程」**。

   >[!NOTE]
   >
   >當您從基本工作流程轉換為自動化工作流程時，無法編輯第一個階段，但您可以新增和設定新階段。

1. 條件式)若要使用您的Adobe Workfront管理員建立並共用給您的自動工作流程範本，請按一下&#x200B;**新增範本**，在出現的方塊中選取範本，然後按一下&#x200B;**新增範本**。

   如需詳細資訊，請參閱本文中的[關於使用自動化工作流程範本](#about-using-automated-workflow-templates)。

1. 將階段新增至自動化工作流程：

   1. 按一下右上角附近的&#x200B;**新舞台**。
   1. 在出現的方塊中，輸入階段的&#x200B;**名稱**。
   1. （選用）設定階段的截止日期。
   1. 在&#x200B;**啟動階段**&#x200B;區段中，選擇您要如何啟動階段：


      <table>
      <tbody>
      <tr>
      <td><strong>建立校訂時</strong></td>
      <td>此階段會自動變成使用中，因為校訂已建立。</td>
      </tr>
      <tr>
      <td><strong>當上一個階段的截止日期過去時</strong></td>
      <td>按一下<strong>父級階段</strong>下拉式清單中的上一個階段。</td>
      </tr>
      <tr>
      <td><strong>在特定日期和時間</strong></td>
      <td>按一下「<strong>日期</strong>」方塊以選取日期，然後按一下右邊的方塊以選取時間。</td>
      </tr>
      <tr>
      <td><strong>所有決定皆已核准或已核准，且有上層階段的變更</strong></td>
      <td>按一下<strong>父階段</strong>下拉式清單中的父階段。</td>
      </tr>
      <tr>
      <td><strong>所有決定皆已在上層階段核准</strong></td>
      <td>按一下<strong>父階段</strong>下拉式清單中的父階段。</td>
      </tr>
      <tr>
      <td><strong>所有決定皆已作出</strong></td>
      <td>按一下<strong>父階段</strong>下拉式清單中的父階段。</td>
      </tr>
      </tbody>
      </table>


   1. 輸入連絡人名稱或電子郵件地址，並設定階段稽核者的設定。

      如需新增稽核者的相關資訊，請參閱本文中的[關於新增稽核者至階段](#about-adding-reviewers-to-a-stage)。

   1. 使用下列任一選項來進一步設定舞台：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>截止日期選項</strong> </td>
         <td><p>若要設定階段的截止日期，請按一下<strong>截止日期選項</strong>下拉式清單中的選項。 接著，在<strong>期限</strong>底下，執行下列其中一項作業：</p>
          <ul>
           <li>如果您選擇<strong>設定特定日期</strong>：請選取您想要的截止日期與時間。</li>
           <li>如果您選擇<strong>從階段啟用日期計算</strong>：選取要新增至階段啟用日期的工作日數以決定截止日期。</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">鎖定階段</td>
         <td>指定可以鎖定舞台的時間。 </td>
        </tr>
        <tr>
         <td role="rowheader">主要決策進行者</td>
         <td><p>選取階段上的主要決策者（只有在您將至少一個具有「核准者」或更高證明「 」角色的人新增到階段後，才能使用）。 如果您選取主要決策者，<strong>僅需要一個決策</strong>選項會在此階段上停用。</p></td>
        </tr>
        <tr>
         <td role="rowheader">只需要一個決定</td>
         <td>當其中一位決策者做出決定時，結束整個稽核程式。<p>如果您在<strong>主要決策者</strong>下拉式選單中指定了使用者，則此選項無法使用。</p></td>
        </tr>
        <tr>
         <td role="rowheader">私人階段</td>
         <td>僅允許下列人員檢視在此階段中作出的評論和決定：主管、Adobe Workfront管理員和Workfront Proof管理員</td>
        </tr>
        <tr>
         <td role="rowheader">透過電子郵件通知人員</td>
         <td>輪到檢閱者處理校訂時，透過電子郵件通知提醒檢閱者。</td>
        </tr>
       </tbody>
      </table>

   1. 按一下&#x200B;**新增階段**。

1. 視需要重複上一步驟以新增更多階段。

   當您新增階段至「自動化工作流程」時，畫面上的圖表會呈現這些階段：

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. 當您完成新增階段時，請按一下&#x200B;**完成**。

## 關於使用自動化工作流程範本 {#about-using-automated-workflow-templates}

使用自動化工作流程範本時，請考量下列事項：

1. 自動化工作流程範本的設定會決定您可以使用自動化工作流程做哪些事來校訂。 例如，如果範本中停用「新增階段」按鈕，當您使用校訂的「自動化工作流程」設定時，將無法看到該按鈕。
1. 當有人在自動化工作流程範本中新增到頁面，但已經在校樣上作為稽核者出現時，套用範本會從階段中移除稽核者。 如果您未將其他稽核者新增至階段，則會出現一則訊息，提示您新增稽核者。
1. 您修改自動化工作流程範本的能力取決於Workfront管理員設定的範本設定，如所述。 如果修改範本的功能已停用，則只有範本的擁有者可以修改它。

## 關於將檢閱者新增至階段 {#about-adding-reviewers-to-a-stage}

將稽核者新增至階段時，請考量下列事項：

* 將使用者新增到階段後，您可以在校訂上為該使用者設定設定，例如校訂角色和他們應具有的任何其他許可權，以及當人們對校訂做出評論和決定時將收到的電子郵件警報型別。
* 您可以將一個或多個使用者從一個階段拖曳到另一個階段。 您可以將使用者直接拖曳到另一個階段，也可以將使用者拖曳到&#x200B;**階段**&#x200B;圖表上的階段。 若要選取多個使用者，請按Shift+Ctrl鍵（在Windows上）或Shift+Command鍵(在Mac上)。
* 您只能將稽核者新增到校訂一次，這表示您無法將同一個人新增到校訂上的多個階段。
* 未新增至私人階段的稽核者在校訂上無法看到該階段，也無法在該階段中做出評論。
* 根據預設，將使用者新增到階段會授予該使用者從建立校訂開始檢視校訂的存取權。

  在工作流程進入新增使用者的階段之前，您的Workfront管理員可以限制使用者存取校訂。 如需詳細資訊，請參閱  中的。
