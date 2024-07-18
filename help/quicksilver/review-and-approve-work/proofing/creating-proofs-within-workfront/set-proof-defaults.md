---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 設定個人校訂預設值
description: 您可以定義個人校訂預設設定，以套用至您建立的校訂。 每次您在Workfront中產生首次校訂或上傳新校訂版本時，都會套用這些預設值。
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 設定個人校訂預設值

您可以定義個人校訂預設設定，以套用至您建立的校訂。 每次您在Workfront中產生首次校訂或上傳新校訂版本時，都會套用這些預設值。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：選取或更高</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

## 設定個人校訂預設值

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**校訂**。

1. 在右上角，按一下您的虛擬人偶，然後選取&#x200B;**個人設定**。
1. 選擇&#x200B;**校訂預設值**&#x200B;標籤，然後指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>預設電子郵件通知設定</strong> </td> 
     </tr> 
     <tr> 
      <td>預設電子郵件警報</td> 
      <td>選取使用者接收電子郵件更新的頻率。 選取所有活動、回覆我的意見、決定、最終決定、每小時摘要、每日摘要或停用。</td> 
     </tr> 
     <tr> 
      <td>新訪客稽核者的預設電子郵件警報</td> 
      <td>選取訪客檢閱者接收電子郵件更新的頻率。 選項與預設電子郵件警示的選項相同。</td> 
     </tr> 
     <tr> 
      <td>新校訂通知</td> 
      <td>選擇在您新增到校訂時接收通知。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>訊息設定</strong> </td> 
     </tr> 
     <tr> 
      <td>校訂主旨範本</td> 
      <td>輸入您與使用者共用校樣時希望在電子郵件主旨中看到的內容。</td> 
     </tr> 
     <tr> 
      <td>校樣訊息範本</td> 
      <td>輸入當您與使用者共用校樣時，您希望在電子郵件內看到的內容。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>預設校訂設定</strong> </td> 
     </tr> 
     <tr> 
      <td>完成所有決定時鎖定校訂</td> 
      <td>選擇以在所有決定做出後自動鎖定校樣，以免進一步變更。</td> 
     </tr> 
     <tr> 
      <td>只需要一個決定</td> 
      <td>選擇在校訂上只需要一個決定。</td> 
     </tr> 
     <tr> 
      <td>需要登入</td> 
      <td> <p>選擇讓校訂僅供擁有Workfront Proof登入憑證的使用者使用。</p> <p>注意：Workfront Proof憑證可能與您的Workfront憑證不同，除非您的公司使用者使用SSO。 我們建議僅在您的公司使用者SSO時才使用此功能。</p> </td> 
     </tr> 
     <tr> 
      <td>啟用訂閱</td> 
      <td>允許組織外部的檢閱者透過公開URL或內嵌程式碼註冊校訂。 選取此選項時，訂閱者必須按一下電子郵件中的連結，才能存取也可使用的校訂。 選取此選項可要求外部檢閱者按一下電子郵件內的連結以存取校訂。 如果選取了「公開共用」選項，且已套用至此使用者建立的所有校訂，則此選項預設為啟用。 </td> 
     </tr> 
     <tr> 
      <td>新來賓檢閱者的預設角色</td> 
      <td>選取訪客檢閱者的預設校訂角色。 選項與預設校樣角色中的選項相同。</td> 
     </tr> 
     <tr> 
      <td>封鎖原始檔案的下載</td> 
      <td>選擇以封鎖使用者下載原始檔案。 </td> 
     </tr> 
     <tr> 
      <td>我的預設校訂角色</td> 
      <td>選擇您的預設校訂角色。 </td> 
     </tr> 
     <tr> 
      <td>我的預設標籤顏色</td> 
      <td>選擇您的預設標籤顏色。 </td> 
     </tr> 
    </tbody> 
   </table>
