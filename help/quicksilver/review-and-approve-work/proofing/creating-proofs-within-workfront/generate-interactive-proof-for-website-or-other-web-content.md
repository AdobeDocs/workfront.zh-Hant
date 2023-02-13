---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 為網站或其他網路內容建立互動式校樣
description: 您可以為網頁內容產生新的互動式校樣，或產生現有互動式校樣的新版本。 這可以是網站或其他類型的互動式內容，例如具有串流視訊或音訊、HTML動畫和互動式橫幅的廣告。
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 為網站或其他網路內容建立互動式校樣

您可以為網頁內容產生新的互動式校樣，或產生現有互動式校樣的新版本。 這可以是網站或其他類型的互動式內容，例如具有串流視訊或音訊、HTML動畫和互動式橫幅的廣告。

在互動式校樣中，審核者可像平常一樣導覽及互動網站或其他網頁內容。

>[!IMPORTANT]
>
>請確定網站或互動式內容可供要檢閱的人存取。 只有在他們也能在網際網路上存取時，才能在校對程式中存取。

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

## 為網站或其他網路內容建立互動式校樣

1. 前往您要建立新網站校樣或現有網站的新版本的專案、工作或問題。
1. 按一下 **檔案** 中。
1. （條件性）如果要建立新校樣，請按一下 **新增**，然後按一下 **校樣** 中。

1. （視條件而定） **新校樣** 頁面時，如果要建立現有校樣的新版本：

   1. 將滑鼠指標暫留在您要建立新版本的URL校樣上，然後按一下其周圍淺藍色背景中的，以選取它。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. 在 **新增** 下拉式清單，按一下 **版本** > **校樣**.

1. 在 **新增檔案** 區段，輸入您要校樣的網站URL，然後按 **輸入**.

   ![proof_website.png](assets/proof-website-350x65.png)

   您可以重複此程式，新增多個要校驗的網站。

1. 按一下您新增的URL。

   ![](assets/click-url-350x137.png)

1. （選用）如果您想要將校樣名稱從網站URL變更為其他名稱，請輸入 **校樣名稱**.
1. 選擇 **互動式**，然後按一下 **完成**.

   >[!NOTE]
   >
   >如果您要將新版本新增至現有的URL校樣，在原始校樣或舊版上設定的任何選項都會保留在此版本中。

1. 按一下 **建立校樣** 建立簡單校樣，而不需進行審核程式。\
   或\
   繼續操作，方法是配置高級校樣：

   * [使用基本工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自動化工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
