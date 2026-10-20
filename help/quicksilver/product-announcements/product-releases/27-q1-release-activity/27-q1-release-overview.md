---
title: 2027年第一季度發行概觀
description: 本頁提供2027年第一季度版本中包含的功能相關資訊。 這些增強功能預計會在整個季度內於生產環境中提供。
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a8c35fd2f1059bd91de7d6d59db7e447ec6af6a9
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 5%
---

# 2027年第一季度發行概觀

本頁提供預定於2027年1月發行的2027年第一季度版本中包含的功能相關資訊。

此頁面上的增強功能可在預覽環境中取得。 當2027年第一季版本接近其計畫生產版本時，此頁面將透過其他增強功能進行更新。

>[!IMPORTANT]
>
>
>除非另有指定，否則每月和每季發行計畫於每月第二整週的星期四提供。
>
>| 每月發行 | 每季發行 |
>|----|----|
>| <ul><li>2026.11 （2026年11月12日）</li><li>2026.12 （2026年12月17日）</li><li>2027.01 （2027年1月21日）</li></ul> | <ul><li>2027.01 （2027年1月21日）</li></ul> |
>
>如需快速發行程式的詳細資訊，請參閱[啟用或停用快速發行程式](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。

## Adobe Workfront增強功能

* [專案增強功能](#project-enhancements)

### 專案增強功能

<table>
    <tbody>
        <tr>
            <td><strong>功能</strong>
            </td>
            <td><strong>預覽</strong></td>
            <td><strong>快速發行</strong></td>
            <td><strong>每季</strong></td>
        </tr>
        <tr>
            <td>
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">將執行緒釘選到更新頂端</a></p>
                <p>您現在可以將最重要的對話串釘選到專案、任務、問題或請求的「更新」區域頂端，讓您的團隊仍然可以看到關鍵資訊。</p>
            </td>
            <td><p>2026年10月15日</p></td>
            <td><p>2026年11月12日</p></td>
            <td><p>2027年1月21日</p></td>
        </tr>
    </tbody>
</table>

## 其他區域發行說明

* [Adobe Workfront Fusion發行活動](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。
* [Adobe Workfront規劃發行活動](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

此版本尚無下列專案的更新：

* 情境規劃工具
* 校樣
* 目標

## 公告

### 棄用工作角色清單檢視中的舊版帳單和成本費率欄位

隨著時間推移，我們引進了更強大的費率管理功能以及專屬的工作角色體驗，可提供更完整且可擴充的費率資訊維護方法。 因此，費率管理開始轉向這些專屬的體驗，而非清單式管理工作流程。

在2027年1月版本中，舊欄位&#x200B;**每小時計費**&#x200B;和&#x200B;**每小時成本**&#x200B;將不再在Workfront API或工作角色清單檢視中可用，包括篩選/檢視/分組設定（直接參考和文字模式計算欄）。

作為報表中的替代專案，您可以使用建議的文字模式代碼（視需要使用`costRates`或`billingRates`）：

    ``
    displayname=Test
    listdelimiter=&lt;br>
    listmethod=nested(costRates)。lists
    type=iterate
    valueexpression=CONCAT({startDate}，&quot; - &quot;，{endDate}，&quot;： &quot;，{value})
    valueformat=HTML
    ``

若要管理和檢閱工作角色費率，請使用專用的費率管理體驗：

* 直接從「工作角色>費率」頁面存取和管理工作角色費率。
* 使用費率報表可複查、分析及報告各職務角色的費率資訊。

不需要執行任何動作即可準備變更。 不過，目前在工作角色清單檢視中顯示&#x200B;**每小時計費**&#x200B;和&#x200B;**每小時成本**&#x200B;欄位的管理員應更新其工作流程，以使用上述建議的費率管理體驗。

有關工作角色費率的資訊，請參閱[建立和管理工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

-->

### 訓練更新

探索每個Adobe Workfront產品版本的學習計畫、學習路徑、影片和指南的最新更新。 如需詳細資訊，請參閱[Workfront教學課程頁面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)的「新增功能」一節。
