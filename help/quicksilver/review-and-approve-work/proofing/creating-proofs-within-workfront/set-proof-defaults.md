---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 配置個人校對預設值
description: 您可以定義套用至您建立之校樣的個人校樣預設設定。 每當您在Workfront中產生首次校樣或上傳新校樣版本時，就會套用這些預設值。
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 配置個人校對預設值

您可以定義套用至您建立之校樣的個人校樣預設設定。 每當您在Workfront中產生首次校樣或上傳新校樣版本時，就會套用這些預設值。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：選擇或更高</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>管理員或更高</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 配置個人校對預設值

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **校對**.

1. 在右上角，按一下您的頭像，然後選取 **個人設定**.
1. 選擇 **校對預設值** ，然後指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>預設電子郵件通知設定</strong> </td> 
     </tr> 
     <tr> 
      <td>預設電子郵件警報</td> 
      <td>選取使用者收到電子郵件更新的頻率。 選擇「所有活動」、「對我的評論的回覆」、「決策」、「最終決策」、「每小時摘要」、「每日摘要」或「禁用」。</td> 
     </tr> 
     <tr> 
      <td>新來賓審核者的預設電子郵件警報</td> 
      <td>選擇來賓審核者接收電子郵件更新的頻率。 選項與預設電子郵件警報的選項相同。</td> 
     </tr> 
     <tr> 
      <td>新校樣通知</td> 
      <td>將您新增至校樣時，選擇接收通知。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>訊息設定</strong> </td> 
     </tr> 
     <tr> 
      <td>校樣主題範本</td> 
      <td>在您與使用者共用校樣時，輸入您希望使用者在電子郵件主旨中看到的內容。</td> 
     </tr> 
     <tr> 
      <td>校樣訊息範本</td> 
      <td>在您與使用者共用校樣時，輸入您希望使用者在電子郵件內文中看到的內容。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>預設校樣設定</strong> </td> 
     </tr> 
     <tr> 
      <td>做出所有決定時鎖定證明</td> 
      <td>選擇在做出所有決策後，自動鎖定校樣，使其不再進行更改。</td> 
     </tr> 
     <tr> 
      <td>只需要一個決定</td> 
      <td>選擇僅要求對證明作出一個決定。</td> 
     </tr> 
     <tr> 
      <td>需要登入</td> 
      <td> <p>選擇讓校樣僅供具有Workfront Proof登入憑證的使用者使用。</p> <p>注意：Workfront校樣憑證可能與您的Workfront憑證不同，除非您的公司使用者是SSO。 建議您只在公司使用者執行SSO時才使用此功能。</p> </td> 
     </tr> 
     <tr> 
      <td>已啟用訂閱</td> 
      <td>允許組織外部的審核者透過公開URL或內嵌程式碼註冊校樣。 選取此選項時，訂閱者必須按一下電子郵件中的連結，才能存取校樣。 選取此選項，要求外部審核者按一下電子郵件中的連結以存取校樣。 如果選取了「公用共用」選項，並套用至此使用者建立的所有校樣，系統就會預設啟用此選項。 </td> 
     </tr> 
     <tr> 
      <td>新來賓審核者的預設角色</td> 
      <td>為來賓審核者選擇預設校樣角色。 選項與預設校樣角色中的選項相同。</td> 
     </tr> 
     <tr> 
      <td>阻止下載原始檔案</td> 
      <td>選擇阻止用戶下載原始檔案。 </td> 
     </tr> 
     <tr> 
      <td>我的預設校樣角色</td> 
      <td>選擇預設校樣角色。 </td> 
     </tr> 
     <tr> 
      <td>我的預設標籤顏色</td> 
      <td>選擇預設標籤顏色。 </td> 
     </tr> 
    </tbody> 
   </table>
