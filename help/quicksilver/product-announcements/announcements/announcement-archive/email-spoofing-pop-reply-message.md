---
content-type: reference
navigation-topic: announcements
title: 電子郵件詐騙和POP回覆移除
description: 我們對Adobe Workfront在20.3版（目標為2020年8月）中傳送和接收電子郵件的方式進行了兩項變更。
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# 電子郵件詐騙和POP回覆

我們對Adobe Workfront在20.3版（目標為2020年8月）中傳送和接收電子郵件的方式進行了兩項變更。

## 來自Workfront的傳出電子郵件

為了提高電子郵件的成功傳送，我們將消除經常被標籤為垃圾郵件的詐騙電子郵件（請參閱電子郵件詐騙）。 所有來自Workfront的電子郵件都會從notifications@my.workfront.com傳送，包括自動警報和使用者與使用者的通訊。 Joan Harris的電子郵件範例在電子郵件的寄件者區域看起來像這樣：

![](assets/noreply.png)

*我們強烈建議您連絡您的IT團隊*，以確保不會封鎖來自notifications@my.workfront.com的電子郵件，以接收您系統的電子郵件。 您也可以參考[設定防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)，以取得流量和電子郵件來自哪些IP位址的詳細資訊。

## 通知的傳入電子郵件回覆（POP回覆）

某些電子郵件通知可讓使用者透過電子郵件回覆，並將回覆複製至Workfront，作為Workfront系統中的評論回覆。 Workfront中的系統管理員傳統上可以選擇提供自己的POP電子郵件伺服器來接收這些回覆，或是使用內建的Workfront回覆系統。 自訂POP電子郵件伺服器選擇將在20.3版本中移除。 所有設定為使用自訂伺服器的帳戶都會自動轉換為使用原生Workfront電子郵件回覆系統。 系統管理員或其他Workfront使用者無需採取任何動作。

直接來自Workfront Proof系統的電子郵件不會有任何變更。 您將會繼續收到這些電子郵件，一如以往。

如果您有任何其他問題或顧慮，請聯絡[Workfront支援團隊](https://one.workfront.com/s/support?language=en_US)。
