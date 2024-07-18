---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 在反複專案中建立敏捷劇本
description: 本文會說明如何在您已處於疊代時建立新的敏捷劇本。
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 在反複專案中建立敏捷劇本

本文會說明如何在您已處於疊代時建立新的敏捷劇本。 如需有關從任務、問題或[!DNL Adobe Workfront]的其他區域建立敏捷劇本的資訊，請參閱[將劇本新增到現有反複專案](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>[！UICONTROL Worker]或更高版本</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[！UICONTROL Manage]內文所在專案的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 在反複專案中建立敏捷劇本

1. 前往您要建立劇本的敏捷反複專案：

   1. 按一下[!DNL Adobe] Workfront右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 團隊]**。

   1. （選擇性）按一下&#x200B;**[!UICONTROL 切換群組]**&#x200B;圖示![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式功能表中選取新的Scrum群組或在搜尋列中搜尋群組。

   1. 在左側面板中，選取&#x200B;**[!UICONTROL 反複專案]**。
   1. 按一下要建立內文的特定反複專案名稱。
   1. 在左側面板中，選取&#x200B;**[!UICONTROL 劇本]**。

1.  按一下&#x200B;**[!UICONTROL 新增劇本].**
1. 指定下列資訊：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL劇本名稱]</strong></td>
      <td>輸入劇本的名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL說明]</strong></td>
      <td>輸入劇本的說明。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL就緒]</strong></td>
      <td>如果內文已準備好加入反複專案，請選取此選項。 選取此選項時，它會向使用者指出哪些待處理專案中的內文已準備好新增到疊代。<br>無論內文是否標示為<strong>[！UICONTROL就緒]，皆可新增至反複專案。</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL估計] （點）</strong></td>
      <td>指定劇本的預估。 如果您的敏捷團隊設定為以點為單位估計劇本，則預設的1點等於8小時。 預估會新增為內文上的[！UICONTROL計畫時數]。<br>例如，如果您估計劇本為3點，預設行為是新增24個計畫時數到劇本。<br>如果內文包含子任務，請記住，所有子任務的合併估計值會決定父內文的估計值。 如需詳細資訊，請參閱<a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">將子工作新增至[！UICONTROL Scrum]展示板</a>上的現有內文。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL父專案]</strong></td>
      <td>開始輸入此劇本將關聯的專案名稱。<br>預設情況下，內文顏色會顯示為此專案中其他內文的相同顏色。<br>專案狀態必須設定為[！UICONTROL目前]。 如果專案狀態不是[！UICONTROL目前]，則不會顯示在下拉式功能表中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL父系任務]</strong></td>
      <td>選擇父項專案後，您就可以選擇父項任務。 當您選取父系任務時，內文會建立為所選專案上父系任務的子任務。<br>開始輸入內文父系工作的名稱，然後當它出現在下拉式清單中時按一下它。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL自訂Forms]</strong></td>
      <td>選取任何自訂表單以新增到劇本中。</td>
     </tr>
    </tbody>
   </table>

1. 按一下&#x200B;**[!UICONTROL 儲存劇本]**。
