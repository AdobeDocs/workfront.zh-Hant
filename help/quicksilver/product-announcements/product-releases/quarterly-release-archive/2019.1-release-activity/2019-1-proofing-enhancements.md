---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1校訂增強功能
description: 本頁說明2019.1版包含的所有校訂增強功能。 此功能現在可在生產環境中使用。
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 2019.1校訂增強功能

本頁說明2019.1版包含的所有校訂增強功能。 此功能現在可在生產環境中使用。

如需2019.1年度所有變更的清單，請參閱[2019.1年度發行活動概觀](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md)。

## 適用於管理員

* [為開啟校訂的非收件者設定預設校訂角色](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## 適用於所有使用者

* [在網頁校訂檢視器中校訂互動式內容](#proof-interactive-content-in-the-web-proofing-viewer)
* [校訂檢視器中註解的預設排序順序現在為最舊到最新](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [在與視訊範圍相關的校訂檢視器中加強評論檢閱](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [從校訂通知或校訂檢視器連結到檔案詳細資訊](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [在校訂檢視器中變更您的電子郵件通知](#change-your-email-notifications-in-the-proofing-viewer)
* [變更案頭校訂檢視器中的背景顏色](#change-the-background-color-in-the-desktop-proofing-viewer)
* [清除案頭校訂檢視器中校訂的快取瀏覽器資料](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## 為開啟校訂的非收件者設定預設校訂角色 {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Workfront管理員現在可以為未在校訂工作流程中指定收件者，但可透過其Workfront物件（例如專案、任務或問題）存取校訂的使用者設定預設校訂角色。

先前，當使用者和訪客在未新增至其工作流程的情況下存取校訂時，其預設校訂角色為檢閱者。

此功能僅適用於在Workfront中建立的校訂，而不適用於Workfront Proof。

## 校訂網路校訂檢視器中的互動式內容 {#proof-interactive-content-in-the-web-proofing-viewer}

如果貴組織的安全原則不允許使用獨立的案頭校訂檢視器應用程式，您的Workfront管理員現在可以在網頁校訂檢視器中啟用互動式內容。 內容必須先整合在ZIP檔案中，才能建立校訂。

如需詳細資訊，請參閱文章中的。

視訊

## 校訂檢視器中註解的預設排序順序現在為最舊到最新  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

在校訂檢視器中，校訂上評論的預設排序順序現在是「最舊至最新」，就像口頭交談一樣。

先前的預設排序順序為「最新到最舊」。

您可以選取不同的排序選項，系統會記住您開啟的所有其他校樣。

如需詳細資訊，請參閱文章中的區段。

## 增強與視訊範圍相關聯的校訂檢視器中評論的檢閱 {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

當您在「校訂檢視器」中檢閱與某個範圍的視訊素材相關聯的註解時，現在可以按一下「播放」來檢視整個範圍的素材。 當播放達到範圍的結尾時，播放會暫停。 註解會保持開啟狀態，這樣您就不會遺失所在的位置。

先前，當您開啟一段視訊片段的註解時，您必須先檢視註解上顯示的影格編號，再按一下「播放」，以手動方式尋找範圍的起點。 否則，「校訂檢視器」會從您上次點按視訊時間軸的任何位置開始播放，且不會暫停在範圍結尾。 此外，當您按一下「播放」時，註解會摺疊，因此您無法再清楚看到您正在檢閱哪個註解。

如需關於檢閱視訊校訂的資訊，請參閱。

視訊

## 來自校樣通知或校樣檢視器的檔案詳細資訊連結 {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

當您收到電子郵件邀請您檢閱校訂，或您正在校訂檢視器中檢閱校訂時，您現在可以快速存取校訂的檔案詳細資訊頁面。 在此頁面上，您可以看到與校訂相關聯的Workfront物件（例如任務、專案或問題）。 這會提供相關內容，協助您瞭解校樣上需要做的工作。

此功能可能僅適用於您新增至系統的新使用者。 此為暫時性問題。

如需詳細資訊，請參閱文章。

視訊

## 在校訂檢視器中變更您的電子郵件通知 {#change-your-email-notifications-in-the-proofing-viewer}

現在，所有校訂檢閱者都可以指定他們要收到哪些校訂通知。 與外部利益關係人合作時，這一點尤其重要。

以前，只有校訂所有者或流量管理員可以為他們新增到校訂的稽核者設定校訂的電子郵件警報。 外部共同作業人員無法控制他們收到哪些有關校訂的電子郵件警示，因為他們沒有所需的Workfront存取權，或適當的許可權層級。

這些設定與您可在Workfront中設定的電子郵件警報設定不同。

如需詳細資訊，請參閱[管理校訂評論和決定的通知](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

視訊

## 變更案頭校訂檢視器中的背景顏色 {#change-the-background-color-in-the-desktop-proofing-viewer}

現在，您可以將「案頭校訂檢視器」的背景顏色，從預設的近黑色變更為白色。 這樣可讓您更容易看到具有透明背景的校訂內容。

如需詳細資訊，請參閱[設定校訂檢視器設定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)。

視訊

## 清除案頭校訂檢視器中校訂的快取瀏覽器資料 {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

當瀏覽器的Cookie和快取設定設為封鎖快顯視窗之類的內容時，這種封鎖行為也會發生在案頭校訂檢視器中，使得檢閱者無法看到您的校訂中的快顯視窗內容並做出評論。

現在您可以清除可能隨校訂一起儲存的瀏覽器快取資料，以便所有內容顯示在案頭校訂檢視器中，且稽核者可以檢視和評論。

如需詳細資訊，請參閱[設定校訂檢視器設定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)。

視訊
