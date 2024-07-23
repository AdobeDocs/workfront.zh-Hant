---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 為網站或其他網頁內容建立靜態校樣
description: 您可以為網頁內容產生新的靜態校樣或現有靜態校樣的新版本。 網路內容可能包括含有串流視訊、HTML動畫或互動橫幅的廣告，但會切割成多個熒幕擷取畫面，以便進行靜態校樣。
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 為網站或其他網頁內容建立靜態校樣

您可以為網頁內容產生新的靜態校樣或現有靜態校樣的新版本。 網路內容可能包括含有串流視訊、HTML動畫或互動橫幅的廣告，但會切割成多個熒幕擷取畫面，以便進行靜態校樣。

為網站或其他網路內容建立靜態校樣時，請考量下列事項：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

+++

## 為網站或其他網頁內容建立靜態校樣

若要建立靜態校樣，網站必須可供公開存取（不在防火牆內），或您組織的允許清單必須包含Workfront網域。 Workfront無法擷取受密碼保護的網站做為靜態校訂。

>[!TIP]
>
>建議對需要授權和密碼保護頁面的內部頁面使用互動式校樣，而非靜態校樣。 如需詳細資訊，請參閱[互動式內容校訂總覽](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)。

1. 前往您要建立新網站校訂或現有網站校訂新版本的專案、任務或問題。
1. 按一下左側面板中的&#x200B;**檔案**。
1. （視條件而定）如果您正在建立新校訂，請按一下&#x200B;**新增**，然後在出現的功能表中按一下&#x200B;**校訂**。
1. （視條件而定）如果您要建立現有校訂的新版本：

   1. 將游標移至您要建立新版本的URL校訂上，然後按一下周圍的淺藍色背景來選取它。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. 按一下&#x200B;**新增** > **版本** > **校訂**。

1. 在&#x200B;**新增檔案**&#x200B;區域輸入您要校訂的網站URL，然後按&#x200B;**Enter**。

   >[!NOTE]
   >
   > URL必須少於1,000個字元。

1. 按一下您新增的URL。

   設定網站校訂的選項隨即顯示。

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. （選擇性）如果要將網站URL的校訂名稱變更為其他名稱，請輸入&#x200B;**校訂名稱。**
1. 請確定已選取&#x200B;**擷取熒幕擷圖**，並使用下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>熒幕擷圖解析度</strong> </td> 
      <td> <p>在檢閱者檢視校樣時調整內容的解析度，讓他們檢視它在不同大小的裝置上的顯示方式，例如手機、平板電腦和顯示器。</p> <p>如果您選取多個解析度，則會為您選取的每個解析度建立個別的校樣。</p> <p>注意：當稽核者對校訂發表評論時，評論會包含顯示何時發表評論的解析度，讓其他稽核者知道哪個解析度與評論相關聯。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>尋找子頁面</strong> </td> 
      <td> <p>擷取網站的子頁面及其首頁面。 您可以按一下「全選」來包含所有頁面，或者只按一下要包含的特定頁面。 加號和減號按鈕可讓您展開並關閉網站中的子頁面區域。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >您無法針對您建立的任何後續校訂版本變更擷取熒幕擷取畫面設定。

1. 按一下&#x200B;**完成**。

   如果您在步驟8中選取了多個熒幕擷圖解析度，清單會包含每個解析度的一組熒幕擷圖。 您可以產生這些熒幕擷取畫面做為個別的校訂，或將其合併為單一校訂(請參閱  在。)。 建議您將兩者合併，尤其是當您要建立靜態網站校訂時。

   >[!NOTE]
   >
   >如果您將新版本新增至現有的URL校訂，任何在原始校訂或先前版本上設定的選項將保留在此版本中。

1. 按一下&#x200B;**建立校訂**&#x200B;以建立不含稽核程式的簡單校訂。\
   或\
   繼續設定進階校訂：

   * [使用基本工作流程建立進階校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自動化工作流程建立進階校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
