---
title: 每個物件型別可設定的功能存取權
description: 本文說明您可以允許作為Adobe Workfront管理員，在每個存取層級中用於每個物件型別的內容。 本檔案也會說明每種存取層級型別的預設設定。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '3508'
ht-degree: 10%

---

# 可設定的每種物件型別功能存取權

>[!NOTE]
>
>本文資訊參考舊版存取層級。 如需新存取層級的資訊，請參閱[新存取層級概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。

為組織設定存取層級時，您可以決定哪些特定動作可供存取層級使用。

本文說明Adobe Workfront管理員可以在每個存取層級中為每個物件型別選取的選項。 本檔案也會說明每種存取層級型別的預設設定。

例如，如果Workfront管理員針對指定存取層級的專案選取「檢視」，具有該存取層級的使用者將只能檢視專案，不能編輯專案。

如需每個存取層級中物件型別所有可用功能的相關資訊，請參閱[每個物件型別可用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)。

## 專案

在每個存取層級中，您可以為專案設定下列選項：

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
   <td>供需規劃員（計畫授權型別）</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用專案的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對專案的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>複製</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>檢視</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用專案的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對專案的有限編輯存取權。 若要瞭解相較於供需規劃員存取層級（允許專案的完整編輯存取權），工作者存取層級中的編輯存取權如何受到限制，請參閱每個物件型別<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">可用的文章</a>功能中的<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">專案</a>小節。</p> <p>若要微調此專案，您可以設定共用專案的功能。 按一下[編輯]按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <b>檢視</b> （預設選項） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> （預設選項） <p>檢視存取權受到限制，因為您無法微調以啟用或停用專案共用。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取專案。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 任務

在每個存取層級中，您可以為工作設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用工作的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取範圍）：允許完整編輯任務存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用工作的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選取範圍）：允許完整編輯任務存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <b>檢視</b> （預設選項） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> （預設選項）<p>檢視存取權受到限制，因為您無法微調以啟用或停用專案共用。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取任務。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

在每個存取層級中，您可以設定問題的下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <p><b>檢視</b></p><p>若要微調此專案，您可以設定共用問題的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對問題進行完整的編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用問題的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對問題進行完整的編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用問題的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對問題進行完整的編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用問題的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對問題進行完整的編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取問題。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 專案組合

在每個存取層級中，您可以為投資組合設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用投資組合的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選擇）：允許對投資組合的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <b>檢視</b> （預設選項） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <b>檢視</b> （預設選項）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> <p>無法使用投資組合的存取權。</p> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法使用投資組合的存取權。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 計劃

在每個存取層級中，您可以為程式設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用程式的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許完整編輯程式。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <b>檢視</b> （預設選項） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <b>檢視</b> （預設選項）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> <p>無法存取程式。</p> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取程式。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 報告、儀表板和行事曆

在每個存取層級中，您可以為報告、控制面板和行事曆設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <p><b>檢視</b></p><p>若要微調此專案，請按一下<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上的齒輪圖示</b>，然後停用或啟用下列任何動作。 兩者預設為啟用：</p> 
      <ul> 
       <li> <p>檢視內建報告</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對報告、儀表板和行事曆的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 除了<b>檢視內建報告</b>、<b>公開共用報告</b>和<b>在整個系統內共用報告</b>之外，預設會啟用這些功能。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>檢視內建報告</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>公開共用報表（外部）</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> （預設選項）<p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何動作。 兩者預設為啟用：</p> 
      <ul> 
       <li> <p>檢視內建報告</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <p><b>檢視</b> （預設選項）<p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何動作。 預設只會啟用「共用」選項。</p> 
      <ul> 
       <li> <p>檢視內建報告</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <p><b>檢視</b> （預設選項）：允許僅供檢視存取已與他們共用的報告、儀表板和行事曆。</p> <p>若要微調此專案，您可以設定檢視內建報表的功能。 按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用<b>檢視內建</b>（預設為停用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取報告、儀表板和行事曆。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 篩選器、視圖和分組

在每個存取層級中，您可以為篩選器、檢視和群組設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b></p><p>若要微調此專案，您可以設定共用篩選器、檢視和群組的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對篩選器、檢視和群組的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b></p><p>若要微調此專案，您可以設定共用篩選器、檢視和群組的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對篩選器、檢視和群組的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用篩選器、檢視和群組的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對篩選器、檢視和群組的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b>：</p> <p>若要微調此專案，您可以設定共用篩選器、檢視和群組的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對篩選器、檢視和群組的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取篩選器、檢視和群組。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 文件

在每個存取層級中，您可以為檔案設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用檔案的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對檔案的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 除了<b>共用公開檔案</b>和<b>共用系統範圍</b>之外，預設會啟用這些功能。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>公開共用檔案（外部）</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <p><b>檢視</b></p><p>若要微調此專案，您可以設定共用檔案的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對檔案的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 除了<b>共用公開檔案</b>和<b>共用系統範圍</b>之外，預設會啟用這些功能。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>公開共用檔案（外部）</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用檔案的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對檔案的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何動作。 除了最後兩個（<b>共用公開檔案</b>和<b>共用系統範圍</b>）之外，預設會啟用所有這些URL。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>公開共用檔案（外部）</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <p><b>檢視</b></p><p>若要微調此專案，您可以設定共用檔案的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對檔案的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>在此存取層級中無法設定對檔案的存取。 但外部使用者可以使用Workfront來檢視、檢閱和下載檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用者

在每個存取層級中，您可以為使用者設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b></p><p>若要微調此專案，您可以設定檢視使用者連絡資訊的功能。 按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用<b>檢視連絡人資訊</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許使用者擁有完整的編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何動作。 預設只會啟用前兩個選項，<b>建立</b>和<b>刪除</b>。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li>使用者管理 (所有使用者)</li> 
       <li> <p>管理使用者 (所有使用者)</p> </li> 
      </ul> <p>如需有關兩個使用者管理員選項的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">授予使用者存取權</a>一文中的<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">設定使用者存取權，以使用自訂存取層級編輯使用者</a>一節。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li><p> <b>檢視</b> （只有選項可用）</p><p>若要微調此專案，您可以設定檢視使用者連絡資訊的功能。 按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用<b>檢視連絡人資訊</b>選項（預設為啟用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li><p> <b>檢視</b> （只有選項可用）</p> <p>若要微調此專案，您可以設定檢視使用者連絡資訊的功能。 按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後啟用或停用<b>檢視連絡人資訊</b>選項（預設為停用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b> （只有選項可用）</p><p>若要微調此專案，您可以設定檢視使用者連絡資訊的功能。 按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後啟用或停用<b>檢視連絡人資訊</b>選項（預設為停用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取使用者。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 團隊

在每個存取層級中，您可以為團隊設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li><b>檢視</b> <p>若要微調此專案，請按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用下列任何選項*。 兩者預設為停用。</p> 
      <ul> 
       <li>檢視所有團隊</li> 
       <li> <p>檢視與我的群組相關聯的團隊</p> </li> 
      </ul> </li> 
     <li> <p><b>編輯</b> （預設選取範圍）：允許團隊的完整編輯存取權。</p> <p>若要微調此專案，請按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用下列任何選項*。 預設會啟用所有專案，但<b>編輯我所在的團隊</b>除外。</p> 
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
      <p>若要微調此專案，請按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用下列任何選項*。 兩者預設為啟用。</p> 
      <ul> 
       <li>檢視所有團隊</li> 
       <li> <p>檢視與我的群組相關聯的團隊</p> </li> 
      </ul> </li> 
     <li> <p><b>編輯</b> （預設選取範圍）：允許團隊的完整編輯存取權。</p> <p>若要微調此專案，請按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用下列任何選項*。 預設只會停用第一個選項<b>編輯我所在的團隊</b>。</p> 
      <ul> 
       <li> <p>編輯我所在的團隊</p> </li> 
       <li> <p>檢視所有團隊</p> </li> 
       <li> <p>檢視與我的群組相關聯的團隊</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b> （只有選項可用）</p> <p>若要微調此專案，請按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用下列任何選項*。 兩者預設為啟用。</p> 
      <ul> 
       <li> <p>檢視所有團隊</p> </li> 
       <li>檢視與我的群組相關聯的團隊</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <p><b>檢視</b> （只有選項可用）</p> <p>若要微調此專案，請按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用下列任何選項*。 兩者預設為啟用。</p> 
      <ul> 
       <li> <p>檢視所有團隊</p> </li> 
       <li>檢視與我的群組相關聯的團隊</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>團隊的存取權無法使用。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>


## 範本

在每個存取層級中，您可以為範本設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li><p> <b>檢視</b></p> <p>若要微調此專案，您可以設定共用範本的功能。 按一下檢視按鈕上的齒輪圖示<img src="assets/gear-icon-in-access-levels.png">，然後停用或啟用<b>共用</b>選項（預設為啟用）。</p> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對範本的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設會啟用所有這些「 」。</p> 
      <ul> 
       <li> <p>建立</p> </li> 
       <li> <p>刪除</p> </li> 
       <li> <p>共用</p> </li> 
       <li> <p>共用系統範圍</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li> <p><b>無存取權</b> （只有可用選項）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <p><b>無存取權</b> （只有可用選項）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <p><b>無存取權</b> （只有可用選項）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取範本。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 財務資料

在每個存取層級中，您可以為財務資料設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <p><b>檢視</b>：</p> <p>若要微調此專案，請按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用下列任何選項*。 兩者預設為啟用。</p> 
      <ul> 
       <li>檢視角色帳單與成本費率</li> 
       <li> <p>檢視使用者帳單與成本費率</p> </li> 
      </ul> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對財務資料進行完整編輯存取。</p> <p>若要微調此專案，請按一下<img src="assets/gear-icon-in-access-levels.png">檢視<b>按鈕上的齒輪圖示</b>，然後停用或啟用下列任何選項*。 預設只會啟用最後兩個選項，<b>檢視角色帳單與成本費率</b>和<b>檢視使用者帳單與成本費率</b>。</p> 
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
     <li> <p><b>無存取權</b> （預設選項）</p> </li> 
     <li> <b>檢視</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <p><b>無存取權</b> （預設選項）</p> </li> 
     <li><b>檢視</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <p><b>無存取權</b> （只有可用選項）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>無法存取財務資料。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如需這些選項的相關資訊，請參閱[帳單與收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)。

## 資源管理

在每個存取層級中，您可以為Resource Management設定下列選項：

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
   <td>規劃者 </td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <b>檢視</b> </li> 
     <li> <p><b>編輯</b> （預設選項）：允許對資源管理的完整編輯存取權。</p> <p>若要微調此專案，請在<img src="assets/gear-icon-in-access-levels.png">編輯<b>按鈕上按一下齒輪圖示</b>，然後停用或啟用下列任何選項。 預設只會啟用第一個選項<b>，也就是在規劃工具</b>中編輯優先順序和預算時數。</p> 
      <ul> 
       <li> <p> 在規劃工具中編輯優先順序和預算</p> </li> 
       <li> <p>管理資源集區</p> <p><b>注意</b>：為了管理資源集區，使用者需要額外的財務資料存取權以及專案財務的許可權。 如果您將「資源管理」存取權授與無權存取財務資料的「供需規劃員」使用者，則該使用者仍可在「資源供需規劃員」中看到每小時配置，但無法切換至「成本」檢視或檢視「業務案例」。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予財務資料的存取權</a>以及<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共用物件的財務許可權</a>。</p> </li> 
       <li> <p>更新工作量平衡工具中的計畫時數</p> <p><b>注意</b>：為了更新工作負載平衡器中的計畫時數，使用者需要貢獻物件的許可權，且在「進階設定」下啟用「進行指派」。 如需詳細資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">物件共用許可權簡介</a>。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工作者 </td> 
   <td> 
    <ul> 
     <li><b>無存取權</b> </li> 
     <li> <b>檢視</b> （預設選項） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>審閱者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> </li> 
     <li> <b>檢視</b> （預設選項）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求者</td> 
   <td> 
    <ul> 
     <li> <b>無存取權</b> （只有可用選項） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部使用者</td> 
   <td> <p>存取權無法使用。 外部使用者只能使用Workfront來檢閱和下載檔案，以及檢視共用給他們的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 情境規劃工具區域

所有存取層級的預設設定為「無存取」。 Workfront管理員可將其變更為任何供需規劃員、工作人員和檢閱者存取層級的檢視或編輯存取權。

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>只有當計畫的連結與其共用時，使用者才能檢視其他使用者建立的計畫。

## Workfront目標區域

全部6個預設存取層級（以及全部4個授權型別）都可以編輯和檢視Workfront目標。

「編輯」為預設選項。
