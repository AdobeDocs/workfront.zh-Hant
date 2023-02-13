---
product-area: documents;setup
navigation-topic: review-a-proof
title: 配置校對查看器設定
description: 您可以為Web校對查看器和案頭校對查看器 — EDIT ME配置以下設定。
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 0%

---

# 配置校對查看器設定

您可以為Web校對查看器和案頭校對查看器配置以下設定：

* 註解標籤和銷釘是否顯示在校樣上。
* 標注工具是否顯示在校對檢視器的頂端或下拉式選單中。
* 您在已開啟校樣時，會收到哪些電子郵件通知作為審核者。

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

您可以為案頭校對檢視器配置下列設定：

* 您希望在檢視器中開啟網站內容內連結的方式。

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* 當您按一下在新瀏覽器索引標籤或視窗中設定為開啟的連結時，會發生什麼事。
* 清除可能與您正在檢視的校樣一起儲存的快取資料，以便讓快顯視窗（可由瀏覽器快取資料封鎖）等內容顯示在檢視器中。

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 配置校對查看器設定

要配置校對查看器設定：

1. 以下列其中一種方式開啟Web Pooting Viewer或Desktop Pooting Viewer:

   * 如果您在Adobe Workfront內進行校樣，請前往包含您要檢視校樣的檔案清單，將游標暫留在檔案上，然後按一下 **開啟校樣**.
   * 如果您使用Workfront校樣，請按一下 **前往校樣** 「控制面板」或「檢視」清單中的校樣圖示 ![](assets/go-to-proof-blue-icon.png).

1. 如果左側工具列未顯示，請按一下 **功能表** 表徵圖，位於Web校對查看器的左上角。

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 在左側工具列中，按一下 **設定** 圖示 ![](assets/settings-icon-in-pv.png).

1. 設定下列任一項 **設定** 顯示。

   可用的設定可能會因您開啟的校樣類型而異。

   * **顯示標籤** （「Web校對查看器」和「Desktop Pooting Viewer」中始終提供）:這些是審閱者使用標注工具時添加到校樣的注釋標籤。 如果禁用它們，則按一下注釋清單中的注釋時仍可以查看它們。

      此設定會影響您開啟的所有校樣。

   * **顯示銷釘** （「Web校對查看器」和「Desktop Pooting Viewer」中始終提供）:這些是審閱者使用標籤工具時添加到校樣的編號銷。 它們會指出審核者新增評論的位置和順序。 如果禁用它們，則按一下注釋清單中的注釋時仍可以查看它們。

      此設定會影響您開啟的所有校樣。

   * **使用擴展的標籤工具** （「Web校對查看器」和「Desktop Pooting Viewer」中始終提供）:依預設，校對檢視器的頂端會顯示標籤工具選項。 您可以將它們設定為顯示在垂直功能表中，而垂直功能表只會在您按一下時開啟。

      此設定對您開啟的所有校樣有效。

   * **傳送有關** （「Web校對查看器」和「Desktop Pooting Viewer」中始終提供）:按一下下方的其中一個選項。 此設定只會影響已開啟的校樣。 如需詳細資訊，請參閱 [校樣意見和決策通知概述](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">所有活動</td> 
        <td>Workfront會在每次校樣有任何活動（例如新留言、回覆或決定）時，傳送電子郵件給審核者。 <p>對於管理校對程式的人員來說，這是絕佳選項，因為這可讓他們查看活動發生的時間。 </p><p>使用者不會收到有關其自身活動的電子郵件警報。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">對我評論的答復</td> 
        <td>只有當有人明確回覆其留言時，系統才會傳送電子郵件給審閱者（這會排除其對其留言的回覆）。 這表示如果校樣上的某人發表新意見，則不會通知審核者。<p>建議您的用戶端使用此設定，以便他們不會收到關於證明的任何其他意見的通知，而且只會收到對其意見的回覆通知。</p><p>雖然具有此電子郵件警報設定的審核者不會收到其他新留言的通知，但他們仍可在校對檢視器中檢視校樣上的所有留言。</p><p>如需註解的相關資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校樣留言</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">決策</td> 
        <td>Workfront僅在有人作出決定時，才會傳送電子郵件給審核者。<p>這對於管理審批流程的人員（如項目經理）來說非常有用，他們需要監控校樣的進度，並查看哪些用戶已做出決策。</p><p>除非您在提交決策時選取電子郵件確認選項，否則系統不會通知您自己的決策。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">最終決定</td> 
        <td>Workfront會在校樣的最後核准者做出決定時傳送電子郵件。<p>此警報常由設計人員使用，他們通常不需要參與實際的審閱討論。 當做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。</p><p>此警報對於只有在審核流程完成時才需要通知的部門主管也很有用。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每小時摘要</td> 
        <td>Workfront每小時會傳送電子郵件給審核者，內含該小時內發生的所有留言、回覆和決定的摘要。<p>只有在過去一小時內發生您自己以外的活動時，才會傳送電子郵件。 </p><p>此警報是查看專案概覽的好方法。</p><p>此摘要的範例使用案例是需要專案概覽但不需要立即收到校樣上所有活動的通知的資深審核者。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每日摘要</td> 
        <td>Workfront只會在您自己的活動以外的日子，傳送一封電子郵件，其中列出所有留言、回覆和決策。<p>此警報是您查看專案摘要的好方法，不會在一天中多次更新。</p><p>此摘要的使用案例範例是部門主管，他想要監控專案的整體進度。</p><p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校樣意見和決策的通知</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">無電子郵件</td> 
        <td>Workfront不會傳送任何電子郵件警報。<br>對於只為了參考而新增至校樣，且不需要收到任何變更通知的人，這個用法很有幫助。<p>系統預設值為「每日摘要」（也顯示為「未設定」）。 如果您或您的審核者未進行任何其他更改，則所有校樣都具有此設定。</p></td> 
       </tr> 
      </tbody> 
     </table>

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **在校樣中按一下超連結時** （僅在案頭校對查看器中可用）:選取一個選項，以指定當您按一下在新瀏覽器索引標籤或視窗中設定為開啟的連結時，案頭校對檢視器中會發生什麼。

      此設定對您開啟的所有互動式校樣有效。

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">在校對檢視器中開啟</td> 
        <td>連結一律會在案頭打樣檢視器中開啟，您可以校樣連結的內容。 </td> 
       </tr> 
       <tr> 
        <td role="rowheader">在瀏覽器中開啟</td> 
        <td>連結一律會在瀏覽器中開啟，而不是在校對檢視器中。 您無法校樣連結的內容。</td> 
       </tr> 
       <tr> 
        <td role="rowheader">每次都問我</td> 
        <td> <p>每次在案頭打樣檢視器或瀏覽器中開啟連結時，都會提示您。 如果您在案頭打樣檢視器中開啟連結，可以校樣連結的內容。 如果您在瀏覽器中開啟連結，便無法校樣連結的內容。</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>此設定只會影響已開啟的校樣。</p> </td> 
       </tr> 
      </tbody> 
     </table>

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **清除快取**:清除可能與您檢視的互動式校樣一起儲存的瀏覽器快取資料。 這樣，彈出式視窗（可由瀏覽器快取資料封鎖）等內容就能顯示在案頭校對檢視器中。

      清除的資料包括HTTP快取（例如下次頁面重新整理後要重複使用的影像）和Web儲存資料快取（例如識別使用者的Cookie和資料）。

      此設定只會影響已開啟的校樣。
