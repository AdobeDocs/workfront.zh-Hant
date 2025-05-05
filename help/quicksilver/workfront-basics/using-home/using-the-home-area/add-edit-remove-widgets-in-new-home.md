---
product-area: home
navigation-topic: new-home
title: 新增、編輯或移除首頁中的Widget
description: 您可以從多個Widget中進行選擇，以自訂首頁上顯示的內容。 這些Widget可以調整大小並重新排列。
author: Courtney
feature: Get Started with Workfront
exl-id: 81f32dfe-cde0-4e61-a542-9b99a18a3953
source-git-commit: c1f5e11c6327ef86bd3f89eb383b3bf06bd4981f
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 6%

---


# 新增、編輯或移除首頁中的Widget

<!-- Audited: 4/2025 -->

您可以從多個Widget中進行選擇，以自訂首頁上顯示的內容。 這些Widget可以調整大小並重新排列。

## 適用於特定授權型別的Widget

依預設，首頁會根據您的授權型別填入特定的Widget。

+++ 展開以檢視每種授權型別的可用小工具

<table border="1" class="inlineTable">
    <tr>
        <td><b>新授權型別</b></td>
        <td><b>預設Widget</b></td>
    </tr>
    <tr>
        <td>標準</td>
        <td>我的專案、我的工作、提及內容、待辦事項</td>
    </tr>
    <tr>
        <td>精簡</td>
        <td>我的工作，我的核准</td>
    </tr>
    <tr>
        <td>貢獻者</td>
        <td>我的請求、提及、我的核准、面板</td>
    </tr>
    <tr>
        <td>外部</td>
        <td>我的核准</td>
    </tr>
</table>

<table border="1" class="inlineTable">
    <tr>
        <td><b>目前授權型別</b></td>
        <td><b>預設Widget</b></td>
    </tr>
    <tr>
        <td>規劃</td>
        <td>我的專案、提及內容、待辦事項</td>
    </tr>
    <tr>
        <td>工作</td>
        <td>我的工作、提及、待辦事項</td>
    </tr>
    <tr>
        <td>檢閱</td>
        <td>我的工作，提及</td>
    </tr>
    <tr>
        <td>請求</td>
        <td>我的專案、我的核准</td>
    </tr>
    <tr>
        <td>參與</td>
        <td>我的工作，提及</td>
    </tr>
    <tr>
        <td>外部</td>
        <td>我的核准</td>
    </tr>
</table>

+++

## 將Widget新增至首頁

Widget是Home的基礎。 將Widget新增至首頁後，您就可以選擇最符合您工作需求的資訊型別。 某些Widget僅適用於特定授權型別，因為它們追蹤的物件僅適用於這些授權。 如需詳細資訊，請參閱上面特定授權型別[&#128279;](#widgets-available-for-specific-license-types)可用的Widget。

新增Widget：

1. 如果將「首頁」設定為著陸頁面，請按一下熒幕上方的Adobe Workfront圖示![Adobe Workfront圖示](assets/home-icon-30x29.png)，或按一下主功能表圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**首頁**，以瀏覽您的首頁。

1. 在熒幕的右上角，按一下&#x200B;**自訂**。

   ![自訂按鈕](assets/customize-button.png)
1. 捲動至&#x200B;**Widget**&#x200B;區段，然後選取您要新增的Widget。

+++ 展開以檢視可用Widget的詳細清單

   * **我的工作**\
       在一個位置顯示所有指派的任務、問題和請求。 您可以按一下「處理它」按鈕開始處理專案，或按一下「完成」按鈕將其標籤為完成。 您也可以更新有關任務和問題的資訊（狀態、條件、完成百分比）、記錄時間，以及從「我的工作」Widget新增更新。

   * **展示板**\
       顯示您已建立或受邀使用的任何面板。 您也可以根據下列範本建立新面板：基本面板、看板、回顧面板和動態面板。

   * **我的專案**\
       顯示您擁有的專案或您在清單中的專案。 您可以使用現有的篩選器、檢視或分組來自訂清單，或直接從介面工具集建立專案。

   * **我的任務**\
       在清單中顯示指派給您的任務。 您可以使用現有的篩選器、檢視或分組來自訂清單，也可以直接從Widget建立任務。 您也可以在外出時委派工作。

   * **我的問題**\
       顯示清單中指派給您的問題。 您可以使用現有的篩選器、檢視或分組來自訂清單，或直接從Widget建立問題。 此Widget僅包含關聯專案設為「目前」的問題，不包含已完成的專案。 您也可以在外出時委派問題。

   * **我的要求**\
       顯示您已提交的所有請求、僅顯示已開啟請求的篩選條件，以及可開啟請求摘要面板的按鈕。

   * **團隊要求**\
       顯示您所在團隊的所有待處理請求 (依團隊排序)，以及用於直接將請求指派給使用者或自行處理請求的按鈕。

   * **我的核准**\
       顯示所有待指派或委派的核准、用於委派核准的按鈕，以及用於直接在小工具中做出核准決策的按鈕。

   * **所有核准**\
           顯示2個圖表，內含平均核准時間和決定的相關資訊，以及擱置和逾期核准的清單檢視。 <span style="color: #ff0000;">此功能是分階段發行的一部分，目前僅供特定客戶使用。</span>

   * **提及次數**\
       顯示來自Workfront的最近評論對話串，類似於「我的更新」頁面。 您可以使用回覆按鈕在Widget中撰寫回覆。 只要任務或問題在過去30天內已更新，此Widget也會顯示針對您指派給、您指派給其他使用者、您擁有、您是主要連絡人或您建立之任務或問題所做的評論。

   * **待辦事項**\
       這個獨特的Widget可讓您將專案新增至您可自由編輯的個人檢查清單。 會將待辦事項作為個人專案中的任務進行追蹤，並在完成後保留最多兩週。

     >[!NOTE]
     >
     >您必須有建立工作的許可權，才能在待辦事項Widget中建立待辦事項，而且只有目前使用者輸入的個人工作才會出現。

+++

1. 按一下&#x200B;**新增Widget**。


## 移動首頁上的Widget或調整其大小

1. 如果將「首頁」設定為著陸頁面，請按一下熒幕上方的Adobe Workfront圖示![Adobe Workfront圖示](assets/home-icon-30x29.png)，或按一下主功能表圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**首頁**，以瀏覽您的首頁。

1. 在首頁上尋找您要移動或調整大小的Widget。

1. 將游標暫留在Widget的頂端邊緣上，直到它變成手形，然後按一下並拖曳Widget，直到它位於您想要的位置。 當您移動Widget時，其他Widget將會在該工具周圍移動。

1. 按一下並拖曳Widget右下角的「調整大小」圖示![調整圖示](assets/resize-icon.png)，以調整Widget大小。

## 從首頁中移除Widget

1. 如果將「首頁」設定為著陸頁面，請按一下熒幕上方的Adobe Workfront圖示![Adobe Workfront圖示](assets/home-icon-30x29.png)，或按一下主功能表圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**首頁**，以瀏覽您的首頁。

1. 在首頁上尋找您要移除的Widget，然後按一下Widget右上角的&#x200B;**更多**&#x200B;圖示![更多圖示](assets/more-icon.png)。

1. 按一下&#x200B;**移除**。


## 變更背景的色彩

1. 如果「首頁」已設定為登陸頁面，請按一下熒幕上方的Adobe Workfront圖示![Adobe Workfront圖示](assets/home-icon-30x29.png)，或按一下主功能表圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**首頁**，以瀏覽您的首頁。

1. 在熒幕的右上角，按一下&#x200B;**自訂**。

   ![自訂按鈕](assets/customize-button.png)

1. 在「**自訂**」面板的「**背景**」區段中，按一下您要為「首頁」背景選取的色彩。 您也可以按一下[無]來移除背景。**&#x200B;**
