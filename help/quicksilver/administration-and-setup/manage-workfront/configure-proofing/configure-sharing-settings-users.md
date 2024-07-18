---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 設定使用者的共用設定
description: 身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定可共用校樣的使用者帳戶、使用者是否可以檢視所有版本的校樣，以及使用者取得共用專案存取權的時間。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# 設定使用者的共用設定

身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定可共用校樣的使用者帳戶、使用者是否可以檢視所有版本的校樣，以及使用者取得共用專案存取權的時間。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：Premium或選取</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須在校訂許可權設定檔中選取管理員。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">設定使用者的校訂存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 設定與其他帳戶的共用

1. 在Workfront中，按一下主要功能表![](assets/main-menu-icon.png)，然後按一下校樣![](assets/proofing-in-main-menu.png)以存取Workfront Proof。

1. 按一下「**設定**」>「**帳戶設定**」，然後按一下「**設定**」標籤。

1. 在&#x200B;**共用**&#x200B;區段中，**允許與**&#x200B;共用，按一下&#x200B;**設定**。

1. 在出現的下拉式清單中，選取選項以指定您是否希望校訂可供任何使用者使用、將校訂共用限制在您自己的帳戶，或將其限制在您自己的帳戶以及您正在共同作業的任何合作夥伴帳戶。
1. 按一下&#x200B;**儲存。**

## 設定共用校訂所有版本的可見度

1. 在Workfront中，按一下主要功能表![](assets/main-menu-icon.png)，然後按一下校樣![](assets/proofing-in-main-menu.png)以存取Workfront Proof。

1. 按一下「**設定**」>「**帳戶設定**」，然後按一下「**設定**」標籤。

1. 在&#x200B;**共用**&#x200B;區段中，在&#x200B;**收件者可以檢視所有版本**&#x200B;的右側，選取&#x200B;**啟用**&#x200B;或&#x200B;**停用**&#x200B;以指示當校訂URL啟用時，是否要允許收件者檢視校訂檢視器中的所有校訂版本。

## 根據工作流程階段活動設定校訂可見度

您可以指定與指定階段相關聯的使用者何時可看到具有自動化工作流程的校樣。

>[!NOTE]
>
>* 此選項僅適用於使用獨立Workfront Proof應用程式；無法使用與Workfront整合的Workfront Proof執行個體或在Workfront中進行校訂。
>* 無論此設定為何，使用者只有在進入與使用者相關聯的階段後，才會收到校訂的電子郵件通知。
>

若要設定使用者何時可看到具有自動化工作流程的校樣：

1. 在Workfront中，按一下主要功能表![](assets/main-menu-icon.png)，然後按一下校樣![](assets/proofing-in-main-menu.png)以存取Workfront Proof。

1. 按一下「**設定**」>「**帳戶設定**」，然後按一下「**設定**」標籤。

1. 在&#x200B;**共用**&#x200B;區段中，根據階段啟用&#x200B;**啟用或停用**&#x200B;校訂可見度。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>已停用</strong> （預設）</td> 
      <td>建立校訂時，使用者可以看到校訂。<br><p>與校訂工作流程中某個階段關聯的任何使用者都可以在建立校訂後立即在搜尋結果中檢視校訂。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>已啟用</strong> </td> 
      <td> <p>只有在使用者關聯的階段變成<strong>作用中後，使用者才能看到校樣。</strong></p> <p><b>附註</b>：   
        <ul> 
         <li><em style="font-style: normal;">啟用此選項後，使用者仍可檢視現有的校訂，只要在建立校訂時即可檢視。</em> </li> 
         <li>在使用者獲得對校訂版本的存取權後（因為與使用者關聯的階段變為使用中），使用者只能看到啟用階段的版本。 如果先前版本從未到達使用者關聯的階段，使用者將無法看到該版本的校訂。</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
