---
product-previous: workfront-proof
product-area: documents;system-administration;setup
navigation-topic: satellite-accounts
title: 在 [!DNL Workfront Proof]中設定附屬帳戶
description: 附屬帳戶是您從自己的 [!DNL Workfront] Proof帳戶中設定並管理的付費帳戶。 如需詳細資訊，請參閱「在 [!DNL Workfront] 校訂中的附屬帳戶」。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 82c6dff3-6187-4145-951c-3f5312049b59
source-git-commit: 5be053a6ee99404673f6f3258a423ef5e5c7f431
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中設定附屬帳戶

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

附屬帳戶是您從自己的[!DNL Workfront Proof]帳戶中設定並管理的付費帳戶。 如需詳細資訊，請參閱 [!DNL Workfront] 校訂](../../../workfront-proof/wp-acct-admin/satellite-accounts/sat-accts-in-wp.md)中的[附屬帳戶。

任何帳單管理員都可以建立Satellite帳戶。 如需有關帳單管理員的資訊，請參閱 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[[!UICONTROL 校訂許可權設定檔]。

>[!NOTE]
>
> 必須在我們的[!UICONTROL Standard]或更新計畫之一上設定附屬帳戶。

## 建立衛星帳戶 {#creating-a-satellite-account}

若要建立Satellite帳戶：

1. 移至[!UICONTROL 帳單]頁面。\
   如需帳單頁面的詳細資訊，請參閱[帳單 [!DNL Workfront Proof] [!UICONTROL 帳單]頁面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)。

1. 按一下&#x200B;**[!UICONTROL 新附屬帳戶]**&#x200B;帳戶按鈕。 (1)

   隨即顯示快顯視窗。

   ![New_Satellite_Account.png](assets/new-satellite-account-350x156.png)

1. 輸入使用者端的詳細資料，包括任何相關的促銷代碼。
1. 按一下「**[!UICONTROL 儲存]**」。Satellite帳戶會自動顯示在[!UICONTROL 帳單]頁面頂端的[!UICONTROL 帳戶]下拉式功能表中。
1. 從下拉式選單中選取新的Satellite帳戶。
1. 繼續[為您的衛星帳戶選取計畫](#selecting-a-plan-for-your-satellite-account)以升級您的衛星帳戶。

## 為您的Satellite帳戶選取計畫 {#selecting-a-plan-for-your-satellite-account}

在您依照[建立Satellite帳戶](#creating-a-satellite-account)中所述設定Satellite帳戶後，您需要將它升級至所需的計畫。

1. 移至[!UICONTROL 帳單]頁面。\
   如需帳單頁面的詳細資訊，請參閱[帳單 [!DNL Workfront Proof] [!UICONTROL 帳單]頁面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)。

1. 在頁面頂端的&#x200B;**[!UICONTROL 您的帳戶]**&#x200B;下拉式功能表中(1)，選擇相關的Satellite帳戶。

   Satellite帳戶的帳單頁面隨即顯示，並自動復寫您帳戶的帳單連絡人詳細資料。

   ![Satellite_Account_Change_Plan.png](assets/satellite-account-change-plan-350x156.png)

1. 按一下頁面右上角的&#x200B;**[!UICONTROL 變更計畫]**&#x200B;按鈕。 (2)\
   或\
   按一下目前或下一個計畫名稱以開啟快顯視窗。 (3)

1. 升級或降級您的計畫。

## 將使用者新增至您的Satellite帳戶

將Satellite帳戶升級至您選擇的計畫後，您需要將使用者新增至帳戶。

1. 以[!DNL Workfront Proof]管理員身分登入[!DNL Workfront Proof]。
1. 按一下&#x200B;**[!UICONTROL 帳戶設定]**。
1. 在頁面頂端的下拉式功能表中，選取相關的Satellite帳戶。 (1)\
   Satellite帳戶的帳戶設定頁面隨即顯示。
1. 按一下頁面右上角的&#x200B;**[!UICONTROL 新增使用者]**&#x200B;按鈕。 (2)\
   顯示[!DNL New User]頁面。

1. 輸入使用者的詳細資料，然後按一下[儲存]。****\
   使用者會收到電子郵件通知，告知其可存取該帳戶。

新增至Satellite帳戶的使用者會在中心帳戶的連絡人清單中顯示為成員。

同樣地，中心帳戶的使用者會顯示為Satellite帳戶聯絡人中的成員。

若要檢視Satellite帳戶中所有使用者的完整清單，請按一下&#x200B;**[!UICONTROL 使用者]**&#x200B;索引標籤。

![SA_New_User.png](assets/sa-new-user-350x156.png)

## 將現有的個別帳戶連結至您的中心帳戶

如果您先前為您的使用者端建立其他個別帳戶，這些帳戶可轉換為Satellite帳戶。

我們將透過連結至您的[!DNL Workfront Proof]帳戶（使其成為中心帳戶）為您解決此問題。

您只需要提供下列詳細資訊：

* 您的[!DNL Workfront Proof]帳戶名稱以及您用來設定它的電子郵件地址
* 您要連結至帳戶的個別帳戶名稱，以及用來設定個別帳戶的電子郵件地址。
