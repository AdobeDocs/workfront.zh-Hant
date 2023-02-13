---
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-workfront-proofing-viewer
title: 比較校對檢視器中的校樣
description: 您可以檢視兩個校樣的並排比較。 這可以是相同校樣的兩個版本，或是兩個完全不同的校樣。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d4ec0c53-1451-4475-aa38-2319c6432936
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---

# 比較校對檢視器中的校樣

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

您可以檢視兩個校樣的並排比較。 這可以是相同校樣的兩個版本，或是兩個完全不同的校樣。

## 比較校樣版本 {#compare-proof-versions}

1. 開啟您要比較多個版本的校樣。
1. 在顯示的校樣檢視器的左上角，按一下校樣的名稱。 然後，在顯示的版本清單中，按一下 **比較** 圖示。

   ![](assets/compare-proofs-choose-version-350x115.jpg)

   校樣會並排顯示，而較新版本會顯示在左側。

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Separate breadcrumbs above each proof allow you to view and go to the work item associated with the proof:</p>
   -->

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/compare-proofs-breadcrumbs-350x148.jpg" style="width: 350;height: 148;"> </p>
   -->

1. 繼續 [使用比較工具](#use-the-compare-tools).

## 比較個別校樣 {#compare-separate-proofs}

您可以比較兩個不同的校樣。

* [比較 [!DNL Workfront]](#compare-separate-proofs-in-workfront)
* [比較 [!DNL Workfront Proof]](#compare-separate-proofs-in-workfront-proof)

### 比較 [!DNL Workfront] {#compare-separate-proofs-in-workfront}

有關比較中單獨校樣的文檔清單的資訊 [!DNL Workfront]，請參閱 [比較兩個不同的校樣](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md#comparing-two-proofs-from-a-document-list) 區段 [比較校樣](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md) 文章。

### 比較 [!DNL Workfront Proof] {#compare-separate-proofs-in-workfront-proof}

>[!NOTE]
>
>您比較的校樣必須位於相同的資料夾中，且位於資料夾結構內的相同階層層級。 如需使用資料夾來分組您要比較的校樣的詳細資訊，請參閱 [在校對檢視器中使用多個校樣](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/work-with-multiple-proofs.md)

1. 在校對檢視器中開啟您要比較的校樣之一。
1. 按一下 **[!UICONTROL 比較模式]** 表徵圖。

   ![png](assets/proof-compare-icon.png)\
   檢視區域分成一半，校樣會同時顯示在校樣檢視器的左側和右側。

   ![Compare_doods-versions.png](assets/compare-proofs-versions-350x180.png)

1. 按一下 [!UICONTROL 資料夾] 圖示（位於左側或右側），列出相同資料夾中的其他校樣。

   ![Folder_icons_when_comparing_in_pooking_viewer.png](assets/folder-icons-when-comparing-in-proofing-viewer-350x121.png)

1. 在清單中，按一下您要與目前在校對檢視器中開啟的校樣進行比較的校樣名稱。

   ![Comparing_doods-list_of_doods_in_folder.png](assets/comparing-proofs-list-of-proofs-in-folder-350x89.png)

   兩個校樣都會出現。

1. 繼續 [使用比較工具](#use-the-compare-tools).

## 使用比較工具 {#use-the-compare-tools}

校樣檢視器提供各種工具，以有效和有效地比較校樣。

* [自動比較校樣](#auto-compare-proofs)
* [比較覆蓋圖中的校樣](#compare-proofs-in-an-overlay)
* [同步導覽比較](#simultaneous-navigation-comparison)

### 自動比較校樣 {#auto-compare-proofs}

自動比較會逐像素比較兩個靜態或視訊校樣。 偵測到的任何差異會在左側的校樣中以紅色強調顯示。

比較互動式校樣時無法使用自動比較功能。

要自動比較兩個校樣：

1. 以下列其中一種方式開始比較校樣：

   * 比較相同校樣的兩個版本(請參閱 [比較校樣版本](#compare-proof-versions) )。
   * 比較兩個不同的校樣(請參閱 [比較個別校樣](#compare-separate-proofs) )。

1. 按一下 **[!UICONTROL 自動比較]** 表徵圖。

   ![png.proof_autocompare_icon](assets/proof-autocompare-icon-31x32.png)

   兩個校樣之間的任何差異會在左側的校樣中以紅色強調顯示。

1. （選用）按一下 **[!UICONTROL 交換機]** 圖示來變更使用中側，以便在右側的校樣上顯示差異。 依預設，差異會顯示在左側的校樣上。

   ![proof_autocompare_changeactive.png](assets/proof-autocompare-changeactive.png)

1. （選用）按一下 **[!UICONTROL 顏色]** 表徵圖，更改突出顯示差異時使用的顏色和不透明度。

   ![proof_compare_color.png](assets/proof-compare-color.png)

### 比較覆蓋圖中的校樣 {#compare-proofs-in-an-overlay}

覆蓋圖比較可讓您以單一校樣來檢視兩個靜態校樣之間的差異，同時在校樣的中央下方提供垂直分隔線。 在垂直分隔線上平移校樣時，會顯示差異。

>[!NOTE]
>
>比較視訊或互動式校樣時，無法使用覆蓋圖比較。

若要啟用覆蓋比較：

1. 以下列其中一種方式開始比較校樣：

   * 比較相同校樣的兩個版本(請參閱 [比較校樣版本](#compare-proof-versions) )。
   * 比較兩個不同的校樣(請參閱 [比較個別校樣](#compare-separate-proofs) )。

1. 按一下 **[!UICONTROL 覆蓋]** 表徵圖。

   ![proof_compare_overlay_icon.png](assets/proof-compare-overlay-icon.png)

   這兩個校樣會顯示為單一校樣，並在校樣的中央下方加上垂直分隔線。

1. 執行下列任一操作：

   * 在垂直分隔線上平移校樣。 當您平移時，您會在垂直分隔線的左側看到校樣，而右側的校樣會顯示在右側。
   * 將垂直分隔線向左和向右移動。 當您移動分隔線時，您會在垂直分隔線的左側看到校樣，而右側的校樣會顯示在右側。

### 同步導覽比較 {#simultaneous-navigation-comparison}

比較校樣時，預設會啟用同時導覽。 比較靜態校樣和靜態校樣，或比較視訊校樣和視訊校樣時，都可使用此功能。 比較靜態校樣和視訊校樣時無法使用。

**靜態校樣：** 在靜態校樣上啟用時，同步導覽會在平移或捲動時鎖定兩個校樣的縮放等級和位置。 當校樣包含多個頁面且同時導覽已啟用時，變更一個校樣中的頁面會導致另一個校樣中的頁面變更。

**影片校樣：** 在視訊校樣上啟用時，同時導覽會記住兩個校樣時間軸上的時間差異。

要在尚未啟用時啟用同時導航，請執行以下操作：

1. 以下列其中一種方式開始比較校樣：

   * 比較相同校樣的兩個版本(請參閱 [比較校樣版本](#compare-proof-versions) )。
   * 比較兩個不同的校樣(請參閱 [比較個別校樣](#compare-separate-proofs) )。

1. 按一下 **[!UICONTROL 同步導覽]** 表徵圖。

   ![proof_compare_monitures_icon.png](assets/proof-compare-simultaneous-icon.png)

1. （選用）按一下 **[!UICONTROL 重設]** 圖示來重設縮放等級和位置（用於靜態校樣）或時間軸（用於視訊校樣）。

   ![proof_compare_monited_reset.png](assets/proof-compare-simultaneous-reset.png)

## 退出比較模式

1. 按一下校樣左上角的(x)圖示，關閉您不想再檢視的校樣。

   ![proof_compare_exit.png](assets/proof-compare-exit-350x163.png)

   未關閉的校樣會在校樣檢視器中開啟。
