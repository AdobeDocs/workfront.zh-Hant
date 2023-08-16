---
title: 在報告畫布中篩選表格
description: 在報告畫布中篩選表格
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 2%

---


# 在報告畫布中篩選表格

將表格區塊新增至報表後，您可以設定篩選器以限制表格中顯示的資訊。

篩選規則中有3個元件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">欄位</td> 
   <td> <p>包含您要用來篩選表格之資訊的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">運算子</td> 
   <td> <p>篩選器決定哪些欄位值包含在表格中或從表格中排除的方式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">值</td> 
   <td> <p>根據運運算元評估的所選欄位中的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

**範例：** 如果您想要將報告中的結果限製為僅顯示Jane Doe擁有的專案，則可以使用「專案所有者」欄位、運運算元「等於」和值「Jane Doe」來建立篩選規則。

或者，您只能顯示已指派專案所有者的專案，該專案所有者會有「專案所有者」欄位且運運算元「非空白」。

## 必要條件

開始之前，您必須先註冊Reporting Canvas測試版。 如需詳細資訊，請參閱 [報告畫布Beta版：概觀](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 設定表格的篩選規則

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下&#x200B;**報告**.

1. 按一下 **新報告**.

   或

   前往現有報表，按一下 **更多選單** 圖示 ![](assets/more-icon.png) 在報表標題中，然後選取 **編輯**.

1. 若要將新表格上的列分組，請將表格區塊拖曳或連按兩下至畫布。

   或

   若要將現有表格上的列分組，請按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在表格標題中。

1. 在右側面板中，找到您要用來篩選表格的欄位，然後將其拖曳至篩選區段。

   隨即顯示篩選規則集，其中包含您選取的欄位名稱。

1. 從下拉式選單中選取您想要的運運算元：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>等於</strong> </td> 
      <td> <p>這只會傳回與搜尋值完全相符的值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不等於</strong> </td> 
      <td> <p>這只會傳回與搜尋值不完全相符的結果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>空白</strong> </td> 
      <td> <p>物件的欄位存在，但欄位尚未指定值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不為空白</strong> </td> 
      <td> <p>您正在篩選的欄位已存在，且已被指定值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>小於</strong> </td> 
      <td> <p>這會搜尋值小於輸入值的所有結果，不包含輸入值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>小於或等於</strong> </td> 
      <td> <p>這會搜尋值小於或等於輸入值的所有結果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>大於</strong> </td> 
      <td> <p>這會搜尋值大於輸入值的所有結果，不包含輸入值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>大於或等於</strong> </td> 
      <td> <p>這會搜尋值大於或等於輸入值的所有結果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>介於</strong> </td> 
      <td> <p>提供2個必要欄位值，並搜尋兩個欄位範圍中的所有結果，包括輸入的值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>包含</strong> </td> 
      <td> <p>這會在整個文字字串中搜尋指定的文字。</p> <p>例如，使用「包含Inf」會擷取任何含有「Inf」或「inf」的內容，例如「Infinity」一詞。</p> <p>附註： Adobe Workfront會搜尋您為每個篩選規則輸入的整個單字或片語。 例如，如果您在搜尋名稱中包含「new project」片語的欄位，Workfront不會顯示名稱中只有「new」或「project」的專案，也不會顯示包含「new main project」等額外字詞的片語。 此篩選只會尋找名稱中包含「新專案」確切片語的專案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不包含</strong> </td> 
      <td> <p>這樣會篩選掉缺少指定文字的專案。</p> <p>例如，「不包含inf」會傳回名稱中沒有「Inf」或「inf」的任何欄位。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 根據您選取的運運算元，輸入完成篩選規則的最後一個值。

   >[!NOTE]
   >
   >此處輸入的值為 **非** 區分大小寫。

1. （可選）若要將另一個篩選規則新增至規則集，請執行下列動作：

   1. 將另一個欄位拖放至 **放置以新增另一個規則** 區段中其他規則下方的區域。
   1. 重複步驟4-6。
   1. 在新規則的左側運運算元下拉式清單中，選取 **和** 或 **或**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>且</p> </td> 
         <td> <p>使用AND運運算元聯結篩選規則或規則集時，您會指出希望符合相同層級的所有規則。</p> <p>依預設，篩選器中的陳述式會由AND運運算元連線。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>或</p> </td> 
         <td> <p>使用OR運運算元聯結篩選規則或規則集時，您會指定您要 <strong>至少</strong> 一個規則（或規則集），在該層級上滿足。</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >同一層級的AND和OR運運算元（連線一個規則集內的多個規則或整個規則集）永遠相符。 例如，如果您變更規則集中兩個規則之間的運運算元，該規則集中的所有其他運運算元將自動變更以符合該規則。

1. （視條件而定）若要新增其他篩選規則集，請執行下列動作：

   1. 拖曳您要新增至的欄位 **新增規則集** 區塊。
   1. 重複步驟4-7。
   1. 在新規則集左側的運運算元下拉式清單中，選取 **和** 或 **或**. 這些運運算元的功能與步驟7所列相同，但適用於整個規則集，而非規則集中的個別規則。****
