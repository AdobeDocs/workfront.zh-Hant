---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3整合與行動增強功能
description: 本頁說明2019.3版本的所有變更整合及行動裝置增強功能。 它在2019年8月19日當週的生產環境中可用。
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 2019.3整合與行動增強功能

本頁說明2019.3版本的所有變更整合及行動裝置增強功能。 它在2019年8月19日當週的生產環境中可用。

如需2019.3年所有變更的清單，請參閱[2019.3發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md)。

## 在MS OneDrive整合中支援共用專案

現在您可以將共用的OneDrive檔案和資料夾連結至Workfront物件。 反之，您可以在Workfront中將檔案上傳到OneDrive中的共用資料夾。

如需詳細資訊，請參閱文章[連結外部應用程式的檔案](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)中的[連結外部檔案至Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents)、[連結一或多個外部資料夾](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder)以及[更新並連結檔案至Workfront的外部雲端提供者](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents)等章節。

如需詳細資訊，請參閱文章[從外部應用程式連結檔案](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)中的[將外部檔案連結至Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents)一節。

## 所有Workfront登入都需要網域規格

如果Workfront URL中未指定網域，則所有Workfront登入現在都會要求使用者指定網域。 要求提供此資訊可讓您的Workfront執行個體更安全。 此外，如果您的Workfront實作有多個例項，此增強功能可讓您將相同使用者新增至實作中的每個Workfront例項。

此變更可能會同時影響使用者登入和API整合：

* **使用者登入**

  如果您的公司網域未包含在Workfront URL中，您現在除了在「使用者名稱」和「密碼」欄位中看到外，還在登入畫面上看到新的「網域」欄位。

  對於大部分的客戶而言，不需要變更，因為網域資訊已包含在Workfront URL中。 例如，「*網域*.my.workfront.com」。

* **API整合**

  如果您有任何API程式碼前往不含網域名稱的位址，該API程式碼將不再運作。

如需詳細資訊，請參閱[登入Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md)。

## 在iOS上使用行動應用程式將任務和問題轉換為專案

您現在可以在iOS上的Workfront行動應用程式中，將個別任務和問題轉換為專案。

## 使用指紋或面容ID登入行動應用程式

視您的裝置而定，您可以選擇使用指紋或面容ID技術登入Workfront行動應用程式。 當您登入行動應用程式時，系統會詢問您是否要使用手機支援的任何驗證方法登入。

如需有關如何管理此功能的詳細資訊，請參閱[適用於iOS的Adobe Workfront](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md)或[適用於Android的Adobe Workfront](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md)。

## 新設定，可自動將使用者從行動裝置登出

為了讓您和貴公司更安全，Workfront行動應用程式15天未使用後就會自動將使用者登出。 Workfront管理員可以在「設定>系統>偏好設定」下的Web應用程式中自訂此時間限制。

如需詳細資訊，請參閱[設定系統安全性偏好設定](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

## 行動應用程式登入時需要網域

為了改善安全性，如果您未使用單一登入憑證登入，Workfront行動應用程式現在需要您提供網域。

>[!NOTE]
>
>iOS推出日期： 2019年6月12日
>
>生產可用性： 2019年6月17日

## 在iOS上使用行動應用程式刪除物件

>[!NOTE]
>
>此功能已在2019年8月19日當週的iOS應用程式商店中推出。

您現在可以在iOS行動應用程式中刪除任務、問題和時程表等物件。 您必須擁有物件的正確許可權才能刪除它。

## 在行動應用程式中依已終止專案篩選

>[!NOTE]
>
>此功能將在2019年8月19日當週的iOS和Android應用程式商店中提供。

我們已在行動應用程式的「專案」索引標籤上新增「廢棄專案」作為篩選選項。

## 使用行動應用程式重設您的密碼

如果您忘記密碼，可以使用Workfront行動應用程式來重設密碼。 點選「忘記密碼？」 並依照畫面上的提示操作。 您無法在行動應用程式上重設您的SSO密碼。

## 行動裝置的新外觀

我們已新增下列外觀和感覺改善專案，以增強您在Workfront行動應用程式中的體驗。

* 將下列專案從「詳細資訊」頁面的頂端列移至熒幕上更顯眼的區域：

   * 加號圖示現在位於畫面的左下角
   * 開始處理專案的核取記號現在是畫面中上方的「處理它」按鈕

* 您現在可以點選「詳細資訊」頁面底部的「顯示更多」 ，檢視附加的自訂表單。
* 已變更您用來提交任務、問題和請求的頁面外觀。

