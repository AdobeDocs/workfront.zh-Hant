---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 向校樣的審核者發送電子郵件
description: 在審核和批准過程中，您可以向校樣的一個或多個審核者發送一條消息。 訊息是提醒審核者完成校樣審核或提供與校樣相關的其他資訊的簡單方式。
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# 向校樣的審核者發送電子郵件

在審核和批准過程中，您可以向校樣的一個或多個審核者發送一條消息。 訊息是提醒審核者完成校樣審核或提供與校樣相關的其他資訊的簡單方式。

您可以選擇發送一般提醒電子郵件或向與指定階段相關聯的一個或多個用戶發送自定義郵件。

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
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 透過校樣傳送電子郵件訊息給使用者

1. 查找包含要發送消息的用戶的校樣的文檔。
1. 將滑鼠指標暫留在檔案上，然後按一下 **校對工作流程**.

   ![](assets/proof-workflow-doc-list-350x92.png)

1. 若要傳送訊息給舞台上的所有使用者，請按一下 **更多** 菜單，然後選擇 **全部消息**.

   ![](assets/message-stage-350x122.png)

1. 若要傳送訊息給個別使用者，請按一下 **更多** 功能表，然後選擇 **訊息**.

   ![](assets/message-user-350x121.png)

1. 在 **訊息詳細資訊** 區段，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">通過電子郵件通知人</td> 
      <td>無法取消選取此選項。 所有使用者都會透過電子郵件接收訊息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">捨棄自訂訊息</td> 
      <td> <p>按一下 <strong>捨棄自訂訊息</strong> 如果您只想包含預設的電子郵件內容。</p> <p>預設提醒電子郵件包含下列資訊：</p> 
       <ul> 
        <li>證明的個人連結<br>校樣影像的縮圖<br></li> 
        <li>下列校樣詳細資料：校樣名稱、版本號、資料夾名稱（如果適用），以及審核者清單及其校樣進度。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">主旨</td> 
      <td>輸入訊息主旨。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">訊息</td> 
      <td>輸入您的訊息內容。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **傳送。**
