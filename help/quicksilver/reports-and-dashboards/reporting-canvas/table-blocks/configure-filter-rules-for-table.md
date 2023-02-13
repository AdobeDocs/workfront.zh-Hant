---
title: 在報表畫布中篩選表格
description: 在報表畫布中篩選表格
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---


# 在報表畫布中篩選表格

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
   <td> <p>篩選器決定要在表格中納入或排除哪些欄位值的方式。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">值</td> 
   <td> <p>根據運算子評估的所選欄位內的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

**範例：** 如果您想要將報表中的結果限制為只顯示Jane Doe擁有的專案，可以建立篩選規則，其欄位為「專案擁有者」、運算子為「等於」，且值為「Jane Doe」。

或者，您只能顯示已分配項目所有者的項目，該項目將具有「項目所有者」欄位和運算子「不為空」。

## 必要條件

開始之前，您必須註冊「報表畫布測試版」。 如需詳細資訊，請參閱 [報表畫布測試版：概述](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 配置表的篩選規則

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下&#x200B;**報表**.

1. 按一下 **新報表**.

   或

   前往現有報表，按一下 **更多功能表** 圖示 ![](assets/more-icon.png) 在報表標題中，然後選取 **編輯**.

1. 若要將新表格上的列分組，請拖曳或按兩下表格區塊至畫布。

   或

   要對現有表上的行進行分組，請按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在表格標題中。

1. 在右側面板中，找出您要依其篩選表格的欄位，然後將其拖曳至「篩選」區段。

   隨即顯示篩選規則集，其中包含您選取之欄位的名稱。

1. 從下拉式選單中選取您要的運算子：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>等於</strong> </td> 
      <td> <p>這只會傳回與所搜尋值完全相符的值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不等於</strong> </td> 
      <td> <p>這只會傳回與所搜尋值不完全相符的結果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>空白</strong> </td> 
      <td> <p>物件的欄位存在，但欄位尚未獲得值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不為空白</strong> </td> 
      <td> <p>您要篩選的欄位存在且已指定值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>小於</strong> </td> 
      <td> <p>這會搜尋值小於輸入值的所有結果，而不包含輸入的值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>小於或等於</strong> </td> 
      <td> <p>這會搜尋值小於或等於輸入值的所有結果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>大於</strong> </td> 
      <td> <p>這會搜尋大於輸入值的所有結果，但不包括輸入值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>大於或等於</strong> </td> 
      <td> <p>這會搜尋值大於或等於輸入值的所有結果。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>介於</strong> </td> 
      <td> <p>提供2個必填欄位值，並搜索兩個欄位範圍內的所有結果，包括輸入的值。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>包含</strong> </td> 
      <td> <p>這會在整個文字字串中搜尋指定的文字。</p> <p>例如，使用「包含Inf」可擷取其中包含「Inf」或「inf」的任何項目，例如「Infinity」。</p> <p>注意：Adobe Workfront會搜尋您為每個篩選規則輸入的整個字詞或片語。 例如，如果您搜尋的欄位名稱中有「new project」一詞，Workfront不會顯示名稱中只有「new」或「project」的專案，或是中間有額外字詞的片語，例如「new main project」。 篩選器只會尋找名稱中具有確切字句「新專案」的專案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不包含</strong> </td> 
      <td> <p>這會篩選掉缺少指定文字的項目。</p> <p>例如，"does not contain inf"會傳回名稱中沒有"Inf"或"inf"的任何欄位。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 根據您選取的運算子，輸入最後一個值以完成篩選規則。

   >[!NOTE]
   >
   >此處輸入的值為 **not** 區分大小寫。

1. （選用）若要新增其他篩選規則至您的規則集，請執行下列動作：

   1. 拖曳其他欄位至 **拖放以新增其他規則** 區域（位於其他規則下方的「篩選器」區段）。
   1. 重複步驟4-6。
   1. 在新規則的運算子下拉式清單中，選取 **和** 或 **或**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>與</p> </td> 
         <td> <p>使用AND運算子連接篩選規則或規則集時，您會指出您希望滿足相同層級的所有規則。</p> <p>依預設，篩選器中的陳述式會以AND運算子連結。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>或</p> </td> 
         <td> <p>使用OR運算子連結篩選規則或規則集時，您會指出您想要 <strong>至少</strong> 要滿足的一個規則（或規則集）。</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >同一層級的AND和OR運算子（將規則集內的多個規則或整個規則集連接在一起）將始終匹配。 例如，如果您在規則集內的兩個規則之間變更運算子，該規則集中的所有其他運算子都會自動變更以符合它。

1. （條件性）若要新增其他篩選規則集，請執行下列動作：

   1. 拖曳您要新增至的欄位 **新增規則集** 區域。
   1. 重複步驟4-7。
   1. 在新規則集的運算子下拉式清單中，選取 **和** 或 **或**. 這些運算子的功能與步驟7中所列的運算子相同，但會套用至整個規則集，而不是套用至集內的個別規則。****
