---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 配置用戶的共用設定
description: 身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定可以共用校樣的使用者帳戶、使用者是否能看到所有版本的校樣，以及使用者何時能存取共用項目。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# 配置用戶的共用設定

身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定可以共用校樣的使用者帳戶、使用者是否能看到所有版本的校樣，以及使用者何時能存取共用項目。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Premium或Select</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須在校樣權限設定檔中選取管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">設定使用者的校對存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 配置與其他帳戶的共用

1. 在Workfront中，按一下主功能表 ![](assets/main-menu-icon.png)，然後按一下「校對」 ![](assets/proofing-in-main-menu.png) 存取Workfront校樣。

1. 按一下 **設定** > **帳戶設定**，然後按一下 **設定** 標籤。

1. 在 **共用** 部分，在 **允許與共用**，按一下 **設定**.

1. 在隨即顯示的下拉式清單中，選取選項以指定您是否要讓校樣可供任何人使用、限制將校樣共用給您的帳戶，或限制將校樣共用給您的帳戶，或限制為您的帳戶以及您正在合作的任何合作夥伴帳戶。
1. 按一下 **儲存。**

## 配置共用校樣的所有版本的可見性

1. 在Workfront中，按一下主功能表 ![](assets/main-menu-icon.png)，然後按一下「校對」 ![](assets/proofing-in-main-menu.png) 存取Workfront校樣。

1. 按一下 **設定** > **帳戶設定**，然後按一下 **設定** 標籤。

1. 在 **共用** 部分，在 **收件者可以檢視所有版本**，選取 **啟用** 或 **停用** 以指出您是否要在啟用「校樣URL」時，允許收件者在校樣檢視器中檢視校樣的所有版本。

## 根據工作流程階段活動設定校樣可見性

您可以指定與指定階段相關聯的使用者何時可看見具有自動化工作流程的校樣。

>[!NOTE]
>
>* 只有使用獨立Workfront Proof應用程式時，才能使用此選項；若使用與Workfront整合的Workfront Proof例項，或在Workfront內進行校對，則無法使用。
>* 使用者只有在進入與使用者相關聯的階段後，才會收到校樣的電子郵件通知，無論此設定為何。
>


若要設定使用者何時可看到具有自動化工作流程的校樣：

1. 在Workfront中，按一下主功能表 ![](assets/main-menu-icon.png)，然後按一下「校對」 ![](assets/proofing-in-main-menu.png) 存取Workfront校樣。

1. 按一下 **設定** > **帳戶設定**，然後按一下 **設定** 標籤。

1. 在 **共用** 部分，啟用或禁用 **基於階段激活的校樣可見性**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>已停用</strong> （預設）</td> 
      <td>建立校樣時，使用者會看到校樣。<br><p>任何與校樣工作流程中的階段相關聯的使用者，都可以在建立校樣後，立即在搜尋結果中看到校樣。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>已啟用</strong> </td> 
      <td> <p>只有在使用者關聯的舞台變成之後，校樣才會顯示給使用者 <strong>活動。</strong></p> <p><b>附註</b>:   
        <ul> 
         <li><em style="font-style: normal;">啟用此選項後，建立時仍會顯示現有校樣的使用者。</em> </li> 
         <li>在使用者取得校樣版本的存取權後（因為使用者關聯的階段會變成使用中），使用者只看得到啟動該階段的版本。 如果上一個版本從未達到使用者所關聯的階段，則使用者看不到該版本的校樣。</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
