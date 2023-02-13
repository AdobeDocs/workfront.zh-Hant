---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: 使用在帳戶之間移動使用者 [!DNL Workfront Proof]
description: 如果您是 [!DNL Workfront Proof] 管理員，並且您有一個或多個與主帳戶連接的衛星帳戶，則可以在所有這些帳戶之間移動用戶。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# 使用在帳戶之間移動使用者 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

如果您是 [!DNL Workfront] 校樣管理員，且您有一或多個衛星帳戶連線至您的主帳戶，即可在所有這些帳戶之間移動使用者。

## 在已連接的帳戶之間移動用戶

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 帳戶設定]**.

1. 開啟 **[!UICONTROL 使用者]** 標籤。
1. 按一下 **[!UICONTROL 移動用戶]** 表徵圖(1)。 ![Move_user2.png](assets/move-user2-350x95.png)

1. 在顯示的「移動」使用者方塊中，確認您要移動的使用者(1)。
1. 從連接的帳戶清單(2)中選擇目標帳戶。
1. 指派此使用者在新帳戶上應擁有的設定檔權限(3)。
1. 選擇應對不移動的項目擁有所有權的用戶(4)。
這包括您決定保留在舊帳戶的項目，以及無法移動的項目(請參閱 [無法移動的項目](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) )。

1. 如果您想要與使用者一起移動校樣(5)和檔案(6)，請核取核取方塊。
1. 為資料夾(7)建立名稱，新帳戶中將放置所有移動的項目。
1. 按一下 **[!UICONTROL 移動用戶]** （八）啟動過程。
   ![Moving_users_pop-up.png](assets/moving-users-pop-up-350x380.png)

如果您選擇移動用戶，而不帶校樣和檔案，則此操作將立即執行。 如果您選擇隨校樣和檔案移動使用者，系統會立即重新指派使用者的設定檔，但校樣和檔案會逐漸顯示在目的地帳戶上，因為此操作需要時間傳輸資料。

根據檔案和校樣移動程式的數量，可能需要幾分鐘到數小時的時間。

>[!NOTE]
>
>如果您懷疑此程式所需時間超過預期，或移動的校樣和/或檔案未出現在新帳戶中，請聯絡我們的支援團隊。

## 無法移動的項目

### 被移動的用戶建立或擁有的資料夾

由於套用至資料夾及其內容的各種權限性質（例如，這些權限可能與其他使用者和帳戶共用），我們無法與使用者移動資料夾結構。

如果移動的用戶擁有資料夾，則在「移動用戶」彈出窗口中，所有權將轉移給選定的用戶(4)。

>[!NOTE]
>
>如果已移動的用戶已建立資料夾，則資料夾將保留其建立者 — 僅轉移所有權。 移動的使用者在新帳戶的側邊欄中仍可看到該資料夾。 被移動的使用者仍可以「唯讀」存取這些資料夾內的項目。

如果您不希望被移動的使用者保留這些權限，或被移動的使用者不想在舊帳戶上看到其舊資料夾，此處的解決方案是依下列方式刪除資料夾：

1. 在舊帳戶上建立新資料夾。
1. 將移動的使用者資料夾中的所有項目移至新建立的資料夾。
1. 刪除移動的用戶所留的所有資料夾。

### 具有不同所有者的版本集

如果校樣有幾個版本，且每個版本都由不同使用者擁有，則已移動使用者擁有的版本將不會隨之移動。 這些版本的所有權將根據您在「移動用戶」框中的選擇(4)轉移給其他用戶。 （如需詳細資訊，請參閱。）

>[!NOTE]
>
>已移動的使用者必須擁有集中的所有校樣版本，校樣才能繼續移動。

### 群組

移動的使用者必須在其新帳戶上重新建立群組。 如需詳細資訊，請參閱 [使用建立校對群組 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### 自訂檢視

移動的使用者在新帳戶上需要重新建立個人自訂檢視。 如需詳細資訊，請參閱 [在中建立和管理自訂檢視 [!DNL Workfront Proof] 校樣](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### 自訂欄位

無法移動自訂欄位，且自訂欄位中的資料會遺失，因此請務必在移動前產生所需項目的報表。

### 自動化工作流程範本

需要在新帳戶上重新建立自動化工作流程範本，但使用範本建立的移動校樣上會保留階段。

### 註解動作

註解的動作會保留在校樣上，但無法再依校樣進行篩選。 解決方案是在新帳戶上建立相符的動作，並視需要以新動作重新標幟註解。
