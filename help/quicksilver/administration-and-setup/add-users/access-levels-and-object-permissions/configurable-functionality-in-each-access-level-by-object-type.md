---
title: 可針對每種對象類型配置對功能的舊版訪問
description: 本文說明在每個舊版存取層級中，可允許以Adobe Workfront管理員身分管理每個物件類型。 它也說明每種舊式存取層級的預設設定。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: e3211ac5801c1318978427bc0a48d9b3a3028984
workflow-type: tm+mt
source-wordcount: '3456'
ht-degree: 10%

---

# 可針對每種對象類型配置對功能的舊版訪問

本文說明在每個舊版存取層級中，可允許以Adobe Workfront管理員身分管理每個物件類型。 它也說明每種舊式存取層級的預設設定。

有關每個訪問級別中對象類型可用的所有功能的資訊，請參見 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 專案

在每個舊版存取層級中，您可以為專案設定下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計畫員（計畫許可證類型）</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此項目，您可以設定共用專案的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯專案的存取權。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>複製</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>檢視</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此項目，您可以設定共用專案的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對專案進行有限的編輯存取。 要了解與計畫員訪問級別（允許對項目進行完全編輯訪問）相比，在員工訪問級別中如何限制編輯訪問，請參閱節 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">專案</a> 在文章中 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">每種物件類型皆可使用的功能</a>.</p> <p>若要微調此項目，您可以設定共用專案的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「編輯」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <b>檢視</b> （預設選取項目） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> （預設選取項目） <p>檢視存取權限有限，因為您無法對其進行微調以啟用或停用專案共用。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取專案。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 任務

在每個舊版存取層級中，您可以為任務配置下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此功能，您可以配置共用任務的能力。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完全編輯對任務的訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此功能，您可以配置共用任務的能力。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完全編輯對任務的訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <b>檢視</b> （預設選取項目） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> （預設選取項目）<p>檢視存取權限有限，因為您無法對其進行微調以啟用或停用專案共用。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法訪問任務。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

在每個舊版存取層級中，您都可以針對問題設定下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <p><b>檢視</b></p><p>若要微調此問題，您可以設定共用問題的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯問題的存取權。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此問題，您可以設定共用問題的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯問題的存取權。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此問題，您可以設定共用問題的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯問題的存取權。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此問題，您可以設定共用問題的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯問題的存取權。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取問題。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 專案組合

在每個舊版存取層級中，您可以為產品組合設定下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此功能，您可以設定共用產品組合的能力。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:可完整編輯產品組合的存取權。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <b>檢視</b> （預設選取項目） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <b>檢視</b> （預設選取項目）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> <p>無法存取產品組合。</p> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取產品組合。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 計劃

在每個舊版存取層級中，您可以為程式配置下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此功能，您可以配置共用程式的能力。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對程式進行完全編輯訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <b>檢視</b> （預設選取項目） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <b>檢視</b> （預設選取項目）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> <p>無法訪問程式。</p> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法訪問程式。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 報表、控制面板和日曆

在每個舊版存取層級中，您可以為報表、控制面板和日曆設定下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <p><b>檢視</b></p><p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕)，然後禁用或啟用以下任一操作。 預設會啟用這兩項功能：</p> 
      <ul> 
       <li> <p>檢視內建報告</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯對報告、控制面板和日曆的存取。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有功能， <b>檢視內建報表</b>, <b>公開共用報表</b>，和 <b>共用全系統</b>.</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>檢視內建報告</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>公開（外部）共用報告</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> （預設選取項目）<p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任何操作。 預設會啟用這兩項功能：</p> 
      <ul> 
       <li> <p>檢視內建報告</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <p><b>檢視</b> （預設選取項目）<p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任何操作。 預設僅啟用「購股權」。</p> 
      <ul> 
       <li> <p>檢視內建報告</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <p><b>檢視</b> （預設選取）:允許僅限檢視的存取已與其共用的報表、控制面板和日曆。</p> <p>若要微調此功能，您可以設定檢視內建報表的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用 <b>檢視內建</b>（預設為停用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取報表、控制面板和日曆。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 篩選器、檢視和群組

在每個舊版存取層級中，您可以針對篩選器、檢視和群組設定下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b></p><p>若要微調此項目，您可以設定共用篩選器、檢視和群組的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯對篩選器、檢視和群組的存取。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b></p><p>若要微調此項目，您可以設定共用篩選器、檢視和群組的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯對篩選器、檢視和群組的存取。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li><p> <b>檢視</b></p> <p>若要微調此項目，您可以設定共用篩選器、檢視和群組的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯對篩選器、檢視和群組的存取。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b>:</p> <p>若要微調此項目，您可以設定共用篩選器、檢視和群組的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完整編輯對篩選器、檢視和群組的存取。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取篩選器、檢視和群組。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 文件

在每個舊版訪問級別中，可為文檔配置以下選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此功能，您可以配置共用文檔的能力。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對文檔進行完全編輯訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有功能， <b>公開共用檔案</b> 和 <b>共用全系統</b>.</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>公開（外部）共用文檔</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <p><b>檢視</b></p><p>若要微調此功能，您可以配置共用文檔的能力。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對文檔進行完全編輯訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有功能， <b>公開共用檔案</b> 和 <b>共用全系統</b>.</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>公開（外部）共用文檔</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此功能，您可以配置共用文檔的能力。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對文檔進行完全編輯訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任何操作。 除了前兩個外，預設會啟用所有選項， <b>公開共用檔案</b> 和 <b>共用全系統</b>.</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>公開（外部）共用文檔</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <p><b>檢視</b></p><p>若要微調此功能，您可以配置共用文檔的能力。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對文檔進行完全編輯訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>在此訪問級別中無法配置對文檔的訪問。 但外部使用者可以使用Workfront來檢視、檢閱和下載檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用者

在每個舊版存取層級中，您可以為使用者設定下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b></p><p>若要微調此功能，您可以設定檢視使用者聯絡資訊的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用 <b>查看聯繫資訊</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對用戶進行完全編輯訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任何操作。 只有前兩個選項， <b>建立</b> 和 <b>刪除</b>，則預設為啟用。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li>使用者管理 (所有使用者)</li> 
       <li> <p>管理使用者 (所有使用者)</p> </li> 
      </ul> <p>如需兩個「使用者管理」選項的相關資訊，請參閱區段 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">使用自訂存取層級設定使用者的存取權以編輯使用者</a> 在文章中 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li><p> <b>檢視</b> （僅可用選項）</p><p>若要微調此功能，您可以設定檢視使用者聯絡資訊的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用 <b>查看聯繫資訊</b> 選項（預設為啟用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li><p> <b>檢視</b> （僅可用選項）</p> <p>若要微調此功能，您可以設定檢視使用者聯絡資訊的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後啟用或禁用 <b>查看聯繫資訊</b> 選項（預設為停用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b> （僅可用選項）</p><p>若要微調此功能，您可以設定檢視使用者聯絡資訊的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後啟用或禁用 <b>查看聯繫資訊</b> 選項（預設為停用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法訪問用戶。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 團隊

在每個舊版存取層級中，您可以為團隊設定下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li><b>檢視</b> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用以下任一選項*。 預設會停用兩者。</p> 
      <ul> 
       <li>檢視所有團隊</li> 
       <li> <p>檢視與我的群組相關聯的團隊</p> </li> 
      </ul> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對團隊進行完整編輯存取。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用以下任一選項*。 預設會啟用所有功能， <b>編輯我所在的團隊</b>.</p> 
      <ul> 
       <li>建立</li> 
       <li>刪除</li> 
       <li> <p>編輯我所在的團隊</p> </li> 
       <li> <p>在我管理的群組中編輯團隊 (僅限群組管理員)</p> </li> 
       <li> <p>檢視所有團隊</p> </li> 
       <li> <p>檢視與我的群組相關聯的團隊</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>檢視</b>
      <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用以下任一選項*。 預設會啟用兩者。</p> 
      <ul> 
       <li>檢視所有團隊</li> 
       <li> <p>檢視與我的群組相關聯的團隊</p> </li> 
      </ul> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對團隊進行完整編輯存取。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用以下任一選項*。 只有第一個選項， <b>編輯我所在的團隊</b>，預設為停用。</p> 
      <ul> 
       <li> <p>編輯我所在的團隊</p> </li> 
       <li> <p>檢視所有團隊</p> </li> 
       <li> <p>檢視與我的群組相關聯的團隊</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b> （僅可用選項）</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用以下任一選項*。 預設會啟用兩者。</p> 
      <ul> 
       <li> <p>檢視所有團隊</p> </li> 
       <li>檢視與我的群組相關聯的團隊</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b> （僅可用選項）</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用以下任一選項*。 預設會啟用兩者。</p> 
      <ul> 
       <li> <p>檢視所有團隊</p> </li> 
       <li>檢視與我的群組相關聯的團隊</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取團隊。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>


## 範本

在每個舊版存取層級中，您可以為範本設定下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此功能，您可以設定共用範本的功能。 按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在「查看」按鈕上，禁用或啟用 <b>共用</b> 選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完全編輯對模板的訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 預設會啟用所有選項。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用全系統</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <p><b>無權存取</b> （僅可用選項）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <p><b>無權存取</b> （僅可用選項）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>無權存取</b> （僅可用選項）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取範本。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 財務資料

在每個舊版存取層級中，您可以為金融資料設定下列選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <p><b>檢視</b>:</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用以下任一選項*。 預設會啟用兩者。</p> 
      <ul> 
       <li>檢視角色帳單與成本費率</li> 
       <li> <p>檢視使用者帳單與成本費率</p> </li> 
      </ul> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許完全編輯對財務資料的訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>檢視</b> 按鈕，然後禁用或啟用以下任一選項*。 只有最後兩個選項， <b>查看職責開單和成本費率</b> 和 <b>查看用戶開單和成本費率</b>，則預設為啟用。</p> 
      <ul> 
       <li>編輯角色帳單與成本費率</li> 
       <li> <p>編輯使用者帳單與成本費率</p> </li> 
       <li>檢視角色帳單與成本費率</li> 
       <li> <p>檢視使用者帳單與成本費率</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <p><b>無權存取</b> （預設選取項目）</p> </li> 
     <li> <b>檢視</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <p><b>無權存取</b> （預設選取項目）</p> </li> 
     <li><b>檢視</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <p><b>無權存取</b> （僅可用選項）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法訪問財務資料。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 如需這些選項的相關資訊，請參閱 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 資源管理

在每個舊式訪問級別中，可以為資源管理配置以下選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>存取層級</th> 
   <th>選項</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>計劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <b>檢視</b> </li> 
     <li> <p><b>編輯</b> （預設選取）:允許對資源管理進行完全編輯訪問。</p> <p>若要微調此項，請按一下齒輪圖示 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>編輯</b> 按鈕，然後禁用或啟用以下任一選項。 只有第一個選項， <b>在計畫員中編輯優先順序和預算小時數</b>，則預設為啟用。</p> 
      <ul> 
       <li> <p> 在規劃工具中編輯優先順序和預算</p> </li> 
       <li> <p>管理資源集區</p> <p><b>注意</b>:為了管理資源池，用戶需要對財務資料的額外訪問和對項目財務的權限。 如果您將資源管理訪問權限授予無權訪問財務資料的計畫員用戶，則用戶仍可以在資源計畫員中查看每小時分配，但無法切換到「成本」視圖或查看業務案例。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予金融資料的存取權</a> 和 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共用物件的財務權限</a>.</p> </li> 
       <li> <p>更新工作量平衡工具中的計畫時數</p> <p><b>注意</b>:為了更新工作負載平衡器中的計畫小時數，用戶需要對對象有貢獻的權限，並在「高級設定」下啟用「進行分配」。 如需詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">對象共用權限概述</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li><b>無權存取</b> </li> 
     <li> <b>檢視</b> （預設選取項目） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檢閱者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> </li> 
     <li> <b>檢視</b> （預設選取項目）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>要求者</td> 
   <td> 
    <ul> 
     <li> <b>無權存取</b> （僅可用選項） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法訪問。 外部使用者只能使用Workfront來檢閱和下載檔案，以及查看與他們共用的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 方案計畫員區域

所有舊版存取層級的預設設定為「無存取權」。 Workfront管理員可將此更改為查看或編輯任何計畫員、員工和審核者訪問級別的訪問權限。

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>只有當共用到計畫的連結時，用戶才能查看其他用戶建立的計畫。

## Workfront目標區

所有6個預設舊版存取層級（以及所有4個授權類型）都可以編輯和檢視Workfront目標。

預設選項為編輯。
