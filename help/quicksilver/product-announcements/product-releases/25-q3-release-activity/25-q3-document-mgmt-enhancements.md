---
title: 2025年第三季檔案管理增強功能
description: 2025年第三季檔案管理增強功能
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4829d487-7041-447f-9a68-fb1acf467734
source-git-commit: c8222e177d7e1ab9f62f5a520a2a941ca87cc27a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 2025年第三季檔案管理增強功能

本頁說明2025年第三季度版本對預覽環境所做的所有檔案管理增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2025年第三季度發行週期中目前可用的所有變更清單，請參閱[2025年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)。

## 案頭校訂檢視器更新

案頭校訂檢視器已更新至2.1.48版。

此更新是修正問題，以保持Desktop Viewer與Mac作業系統相容。 Electron已降級為34.4.0，而Chromium已降級為132。

此更新同時適用於Mac和Windows。


## 已連結Google資料夾中的Assets必須個別新增，才能在Workfront中顯示

>[!NOTE]
>
>* 預覽版本： 2025年5月31日；適用於所有客戶的生產版本： 2025年5月31日

Google針對存取Google Drive的協力廠商應用程式[加強安全性控制](https://workspace.google.com/blog/product-announcements/enhancing-security-controls-for-google-drive-third-party-apps)，要求應用程式採用每位使用者的同意模式。 因此，個別資產必須一次連結一個資產，才能在Workfront中顯示。 如需詳細資訊，請參閱[設定檔案整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md)。

維持不變的主要功能：

* 在Google磁碟機模式中搜尋並篩選資產和資料夾
* 從Google Drive將資產連結至Workfront物件
* 透過檔案頁面上的「傳送至」下拉式清單，將資產上傳至Google Drive
* 在使用者的「我的磁碟機」區域中檢視及存取資料夾結構
* 從Google Drive將資產的新版本連結至Workfront中的現有檔案
* 從Google Drive將資料夾連結至Workfront物件
* 將檔案拖放至連結資料夾，即可將資產上傳至Google Drive
* 在Workfront中建立新的Google Drive檔案


## 校訂檢視器中可用的新檔案核准決定按鈕

>[!IMPORTANT]
>
>此功能屬於分階段發行，僅供特定客戶使用。

>[!NOTE]
>
>* 預覽版本： 2025年4月10日；適用於所有客戶的生產版本： 2025年4月17日

新檔案核准決定按鈕現在會出現在校訂檢視器中。 現在，當您建立簡單的校訂，然後從檔案摘要新增核准者和稽核者時，他們可以直接在校訂檢視器中做出決定。

之前，您必須退出校訂檢視器才能做出決定。

在此版本之前建立的核准將不會在校訂檢視器中顯示按鈕。

如需詳細資訊，請參閱[一起使用新檔案核准和校訂](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)。
