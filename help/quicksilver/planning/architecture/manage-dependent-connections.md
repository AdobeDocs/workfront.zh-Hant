---
title: 管理相依連線
description: 作為工作區管理員，您可以在Adobe Workfront Planning中建立記錄型別之間的連線欄位時定義相依連線。 新增連線欄位時，您可以開啟設定，指示當兩個欄位一起出現在第三個記錄型別時，連線記錄型別的值取決於來源記錄型別的值（您正在新增連線的值）。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6f64c3e6ebb8407c38ad3a1d46b2fc63b534879e
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 1%

---


# 管理相依連線

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 在「預覽」版發行後，啟用的客戶每月可在「生產」環境中使用相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

作為工作區管理員，您可以在Adobe Workfront Planning中建立記錄型別之間的連線欄位時定義相依連線。

新增連線欄位時，您可以開啟設定，指示當兩個欄位一起出現在第三個記錄型別時，連線記錄型別的值取決於來源記錄型別的值（您正在新增連線的值）。

例如，您可能想要確保區域欄位僅顯示與所選地理繫結的值。 這直接在連線欄位設定中設定：當從地域記錄型別新增連線到相依記錄型別（例如地區）時，新設定可讓工作區管理員使用在這些記錄型別之間已建立的關係，將其標籤為相依於地域記錄型別。

設定之後，參考這兩個欄位（例如促銷活動）的任何記錄型別都會立即看到效果：選取地理值會將區域選擇器縮小為僅包含實際連結至該地理的區域。 這會自動強制執行您的記錄結構，消除不相符的組合，並減少手動清除作業。

## 存取權要求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>若要從相同工作區連線記錄型別： </p>
<ul> 
<li><p>任何Workfront或工作流程套件和任何Planning套件</p></li>
<p>或</p>
<li><p>以獨立產品形式購買時的任何Planning套件</p></li>
</ul>

<p>若要從不同的工作區連線記錄型別：</p>

<ul>

<li><p>任何工作流程和Planning Prime或Ultimate套件</p></li>
<p>或</p>
<li><p>任何以獨立產品形式購買的Planning Prime或Ultimate套件</p></li>
</ul>
   </td> 
<tr> 
<td> 
   <p> 其他產品</p> </td> 
   <td> 
   <p> 除了Adobe Workfront之外，如果您想要將記錄型別與下列應用程式的物件連線，也必須具備下列專案：</p>
   <ul><li><p>Adobe Experience Manager Assets授權及AEM Assets與Workfront之間的整合，用於連結AEM資產與Planning記錄型別。</p>
   <p>如需詳細資訊，請參閱<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">適用於Experience Manager Assets和Assets Essentials的Adobe Workfront：文章索引</a>。 </p></li>
   <li><p> 連線記錄型別與GenStudio物件和品牌的Adobe GenStudio for Performance Marketing授權</p>
   <p>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">開始使用Adobe GenStudio for Performance Marketing</a>。</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>規劃標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>擁有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到存取層級</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Sent a slack message to Norayr, Predator, Snowstorm, Armine for info for this section: 
-->

## 相關連線欄位的考量事項


* 相依的連線欄位只能在已建立連線欄位關係的記錄型別之間設定。 您無法在不相關的記錄型別之間定義相依性邏輯。

* 在不同的工作區中，記錄型別之間可以有相依的連線欄位。

* Planning記錄型別與Workfront或AEM物件型別之間不能有相依的連線欄位。

* 相依性設定是在連線欄位設定本身中一次設定一個連線，而不是設定為全域規則。

* 只有當來源和相依欄位同時出現在第三個記錄型別時，才會啟用兩個連線記錄之間的篩選行為。 如果記錄型別上只顯示兩個欄位中的一個，則相依性沒有作用。

* 相依欄位的選擇器僅限於在記錄層級已連結到所選來源值的值；它無法顯示或建議未連結的值。

* 如果來源欄位的值變更，相依欄位會自動清除，而不是保留在無效狀態，以防止不相符的組合持續存在。

  您會收到內嵌或快顯通知訊息，說明為何已清除相依欄位。

* 每個相依欄位最多可以有3個直接控制欄位。

* 相依性層級限製為6個連線。 這表示最多可以連線7個記錄型別。

* 為了讓相依性鏈結運作，所有相依欄位必須同時存在於相同的記錄型別上。

## 建立相依連線

1. 以工作區管理員的身分，前往Workfront Planning中的記錄型別，並在表格檢視中開啟它。
1. 按一下表格檢視右上角的&#x200B;**+**&#x200B;圖示以新增欄位。
1. 按一下&#x200B;**新增連線**，然後開始為第二個記錄型別新增連線。

   >[!TIP]
   >
   >您只能在兩個Planning記錄型別之間建立相依連線。 您無法在Workfront或AEM的記錄型別和物件之間建立相依連線。
1. 在&#x200B;**連線設定**&#x200B;區段中，開啟&#x200B;**讓此連線相依**。

   >[!TIP]
   >
   >開啟&#x200B;**讓此連線相依**&#x200B;設定會自動開啟&#x200B;**在連結的記錄型別上建立對應欄位**。 每個記錄型別有500個欄位的限制。

   ![已啟用相依連線的新連線標籤](assets/dependent-connection-enabled-setting.png)

1. 繼續設定連線，如文章[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)所述。
1. 按一下「**儲存**」。

   會發生下列情況：

   * 兩個記錄型別之間的連線已建立，當它們在相同記錄型別上一起顯示時，它們的值將彼此相依。
   * 為第二個記錄型別建立顯示第一個記錄型別的對應欄位。
   * 當兩個記錄型別都連線到第三記錄型別時，顯示為第二個連線的記錄欄位選項的值是連線到第一個記錄的值。 作為第一個記錄型別的選擇顯示的值是連線到第二個記錄型別的值。

     如需相關資訊，請參閱本文章中的[相依連線記錄型別](#example-of-dependent-connected-record-types)範例。
   * 已連線記錄欄位的欄標題中有一個指示，說明該欄位處於相依連線關係。

     欄標題](assets/dependent-icon-tooltip-in-column-header.png)中的![相依圖示工具提示
1. （選擇性）按一下「**記錄篩選規則**」，並從您要連線的記錄型別中選取欄位，以限制該欄位值的選項，然後按一下「**完成**」。

   當這兩個欄位出現在第三個記錄型別上時，連線的欄位記錄型別的選項將受到您在此處選取的篩選條件的限制。
1. （選用且建議使用）移至第三個記錄型別，並將第一個和第二個記錄型別新增為連線的記錄欄位。

   ![第三個記錄型別上的相依已連線欄位指標](assets/dependent-connected-field-indicator-on-a-third-record-type.png)

## 相依連線記錄型別的範例

本節提供如何設定相依記錄型別的簡單範例，以及這些型別如何用於第三個記錄型別。

1. 在您可以管理的工作區中，建立下列記錄型別：

   * 促銷活動
   * 國家/地區
   * 大陸

1. 在&#x200B;**國家/地區**&#x200B;記錄型別中，新增下列記錄：

   * 法國
   * 美國
   * 日本
1. 在&#x200B;**大陸**&#x200B;記錄型別中，新增下列記錄：

   * 歐洲
   * 美洲
   * 亞洲

1. 從&#x200B;**國家**&#x200B;記錄型別，為&#x200B;**大陸**&#x200B;建立連線的相依欄位。

   這會新增下列連線的記錄欄位：

   * **大陸**&#x200B;記錄型別的&#x200B;**國家/地區**&#x200B;已連線記錄欄位。
   * **國家/地區**&#x200B;記錄型別的&#x200B;**大陸**&#x200B;連線記錄欄位。

1. 執行下列其中一項：

   * 從&#x200B;**國家**&#x200B;記錄型別資料表檢視中，為「大陸連線」記錄欄位新增下列值：

     * 法國的歐洲
     * 適用於美國的美洲
     * 日本的亞洲
   * 從&#x200B;**大陸**&#x200B;記錄型別資料表檢視，為&#x200B;**國家**&#x200B;連線的記錄欄位新增下列值：

     * 歐洲法國
     * 美國
     * 日本代表亞洲
1. 將&#x200B;**國家**&#x200B;和&#x200B;**大陸**&#x200B;連線的欄位新增至&#x200B;**促銷活動**&#x200B;記錄型別資料表檢視。
1. 在&#x200B;**促銷活動**&#x200B;記錄型別上，為&#x200B;**國家/地區**&#x200B;欄位選取&#x200B;**日本**。 請注意，行銷活動上&#x200B;**大陸**&#x200B;已連線欄位唯一可用的值是&#x200B;**亞洲**。

   或

   在行銷活動記錄型別上選取&#x200B;**大陸**&#x200B;欄位的&#x200B;**歐洲**。

   請注意，行銷活動上&#x200B;**國家/地區**&#x200B;已連線欄位唯一可用的值是&#x200B;**法國**。



