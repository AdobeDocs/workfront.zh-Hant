---
user-type: administrator
product-area: system-administration
keywords: kickstart,kickstart,kickstarts,kickstarts
navigation-topic: use-kick-starts
title: 透過Kick-Starts從Adobe Workfront匯出資料
description: 身為Adobe Workfront管理員，您可以使用Kick-Starts資料匯出工具，從Workfront匯出資料。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 9%

---

# 透過Kick-Starts從Adobe Workfront匯出資料

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

身為Adobe Workfront管理員，您可以使用Kick-Starts資料匯出工具，從Workfront匯出資料。 匯出後，您就可以在其他應用程式中使用它。

透過「啟動」匯出資料也有助於了解哪些欄位與每個物件相關聯、這些欄位的編碼方式，以及這些欄位的值在資料庫中的格式化方式。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用啟動匯出資料的優點和缺點

在Workfront中匯出資料有兩種方式：

* 從報表或清單匯出資料

   如需從報表或清單匯出資料的詳細資訊，請參閱 [匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* 透過啟動匯出資料

下表顯示了每種方法的優缺點：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>匯出的資料包含物件和欄位值</p> </th> 
   <th> <p>可同時匯出多個物件類型的資料</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>從清單檢視匯出資料</strong> </p> <p>如需從清單匯出資料的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">匯出資料</a></p> </td> 
   <td> <p>是</p> <p>會匯出與物件相關聯的Workfront原生欄位和自訂欄位。</p> </td> 
   <td> <p>否</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>透過Kick-Start匯出資料</strong> </p> </td> 
   <td> <p>是（有限）</p> <p>與物件相關聯的大部分Workfront原生欄位都會匯出，但有些則否。 例如，您不能通過項目啟動導出導出導出「計畫」、「項目所有者」或「項目贊助商」欄位。</p> <p>在已附加自訂表單的專案中，表單欄位中輸入的任何資料都不會匯出。</p> <p>但您可以匯出自訂表單。 產生的檔案會列出表單中設定的欄位，例如文字方塊和選項按鈕。</p> </td> 
   <td> <p>是</p> <p>使用「啟動」來匯出Workfront資料，可讓您在單一匯出中匯出與多個物件類型相關的資料。 例如，您可以在單一匯出中包含工作、問題和專案。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 匯出限制

透過開始匯出資料時（資料會以Excel檔案格式匯出）存在下列限制：

* **50,000列：** 檔案中允許的行數。
* **65,530個超連結：** 這是Excel對包含65,530個以上超連結的檔案所施加的限制。 這些文檔在導出後無法開啟。 請注意， Excel文檔可能只有200行資料，但如果文檔內有65,530個以上的連結，則該文檔不會開啟。

## 透過啟動匯出資料

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **開球，** 然後按一下 **匯出資料。**

1. 選取要匯出的物件。
1. 按一下 **更多選項** 以查看對象的完整清單。

   此處列出的所有物件也可用來將資料匯入Workfront。

   唯一的例外是 **存取層級** 物件。 導出中包含的「訪問級別」資料表僅供參考。 它可讓您依ID將存取層級指派給新使用者帳戶。

   如需有關透過啟動將資料匯入Workfront的詳細資訊，請參閱 [使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). 以下是可通過啟動導出的所有對象的清單：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>物件</p> </th> 
      <th> <p>導出的Excel檔案工作表</p> </th> 
      <th> <p>匯出格式</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">存取層級</td> 
      <td scope="col" valign="top">存取層級<br>偏好設定</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">指派</td> 
      <td scope="col" valign="top">分配<br>偏好設定</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">公司</td> 
      <td scope="col" valign="top"> 公司<br>偏好設定 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">電子郵件範本</td> 
      <td scope="col" valign="top"> 電子郵件範本<br>偏好設定 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">費用</td> 
      <td valign="top"> 費用<br>偏好設定 </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">外部頁面</td> 
      <td valign="top"> 外部頁面<br>偏好設定 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">篩選器</td> 
      <td valign="top"> 篩選<br>偏好設定 </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">群組</td> 
      <td valign="top"> 群組<br>偏好設定  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">分組</td> 
      <td valign="top"> 分組<br>偏好設定 </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">時數</td> 
      <td valign="top"> 小時<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">問題</td> 
      <td valign="top"> 問題<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">職務角色</td> 
      <td valign="top"> 工作角色<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">里程碑路徑</td> 
      <td valign="top"> 里程碑<br>里程碑路徑<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">備註</td> 
      <td valign="top"> 附註<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">專案組合</td> 
      <td valign="top"> Portfolio<br>偏好設定  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">專案</td> 
      <td valign="top"> 佇列<br>專案<br>路由規則<br>隊列主題<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">資源估計</td> 
      <td valign="top"> 資源估計<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">資源集區</td> 
      <td valign="top"> 資源池<br>偏好設定 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">風險</td> 
      <td valign="top"> 風險<br>偏好設定  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">風險類型</td> 
      <td valign="top"> 風險類型<br>偏好設定  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">計分卡</td> 
      <td valign="top">計分卡問題<br>記分卡選項<br>計分卡<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">任務</td> 
      <td valign="top"> 任務<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">範本</td> 
      <td valign="top"> 佇列<br>範本<br>路由規則<br>隊列主題<br>偏好設定 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">範本指派</td> 
      <td valign="top"> 模板分配<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">範本任務</td> 
      <td valign="top"> 模板任務<br>偏好設定 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">時程表</td> 
      <td valign="top"> 時間表配置檔案<br>工時單<br>偏好設定 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> 檢視 </td> 
      <td valign="top"> 檢視<br>偏好設定  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **下載。**

   匯出的啟動檔案會以Excel檔案或的形式下載至您的電腦。 包含多個Excel和屬性檔案的zip檔案。 每個Excel檔案都是工作表的集合，其中每個工作表都代表與所選物件相關聯的欄位。 有 **屬性** 與每個導出關聯的工作表。

   此 **控制面板** 和 **報表** 選項可讓您選取要包含在下載中的特定控制面板和報表。 您只能匯出在全系統共用的控制面板。

   無法導出矩陣報表。 如需矩陣報表的詳細資訊，請參閱 [建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   在單次匯出中，最多可選取100個控制面板和100個報表。

   ![](assets/kickstart-export-350x381.png)

   您可以一次匯出多個物件。

   依預設，下列物件會顯示在 **應包含的內容** 標籤(在點按 **更多選項**):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>物件</strong> </p> </th> 
      <th> <p><strong>導出的Excel檔案工作表</strong> </p> </th> 
      <th> <p> <strong>匯出格式</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>儀表板</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>參數<br>參數選項<br>參陣列<br>類別參數<br>類別<br>報表<br>門戶頁簽部分<br>控制面板<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>報告</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">參數<br>參數選項<br>參陣列<br>類別參數<br>類別<br>報表<br>偏好設定</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>核准</p> </td> 
      <td scope="col" valign="top"> <p>步驟核准者<br>核准步驟<br>核准<br>核准程式<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>自訂資料</p> </td> 
      <td scope="col" valign="top"> <p>參數<br>參數選項<br>參陣列<br>類別參數<br>類別<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>費用類型</p> </td> 
      <td valign="top"> <p>費用類型<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>時數類型</p> </td> 
      <td valign="top"> <p>小時類型<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>團隊</p> </td> 
      <td valign="top"> 團隊成員<br>團隊<br>偏好設定 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>使用者</p> </td> 
      <td valign="top"> <p>使用者<br>偏好設定</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong></strong> </p> </th> 
      <th> <p><strong>導出的Excel檔案工作表</strong> </p> </th> 
      <th> <p> <strong>匯出格式</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>儀表板</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>參數<br>參數選項<br>參陣列<br>類別參數<br>類別<br>報表<br>門戶頁簽部分<br>控制面板<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>報告</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">參數<br>參數選項<br>參陣列<br>類別參數<br>類別<br>報表<br>偏好設定</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>核准</p> </td> 
      <td scope="col" valign="top"> <p>步驟核准者<br>核准步驟<br>核准<br>核准程式<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>自訂資料</p> </td> 
      <td scope="col" valign="top"> <p>參數<br>參數選項<br>參陣列<br>類別參數<br>類別<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>費用類型</p> </td> 
      <td valign="top"> <p>費用類型<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>時數類型</p> </td> 
      <td valign="top"> <p>小時類型<br>偏好設定</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>團隊</p> </td> 
      <td valign="top"> 團隊成員<br>團隊<br>偏好設定 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>使用者</p> </td> 
      <td valign="top"> <p>使用者<br>偏好設定</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （建議）分析匯出的資料，確保您預期會看到的所有資訊皆已匯出。

   若是大型匯出項目，Workfront會在背景工作以產生Excel檔案，並針對延遲提供警告訊息。 下載完成時，啟動檔案會以電子郵件傳送給您。

   ![](assets/large-kick-start-file-warning-350x65.png)
