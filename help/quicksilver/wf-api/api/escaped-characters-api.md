---
content-type: api
navigation-topic: api-navigation-topic
title: API回應中的逸出字元
description: API回應中的逸出字元
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 5%

---

# API回應中的逸出字元

某些API回應的語法可能包含逸出字元`\` （反斜線）。 逸出字元表示緊接在逸出字元之後的字元或字串具有特殊值。 例如，`\t`告訴讀取裝置`t`應該解譯為`tab`，而不是解譯為字母「t」。 反斜線後面一或多個字元的字串稱為逸出序列。

十六進位逸出序列需要使用有效的十六進位數字。 下表列出在Adobe Workfront API回應中編碼的逸出序列：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>逸出順序</strong> </th> 
   <th><strong>Unicode字元</strong> </th> 
   <th><strong>代表</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>其中，<em>x</em>是數字0到7的十六進位代碼</p> </td> 
   <td>0-7</td> 
   <td>由代碼點0到7表示的Unicode字元</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>退格字元</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>標籤</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>換行</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>垂直索引標籤</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>換頁字元</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>歸位</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>其中， xx是十六進位程式碼  數字14到31</em> </p> </td> 
   <td>14 - 31</td> 
   <td>由代碼點14到31表示的Unicode字元</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ （正斜線）</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; （小於）</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ （反斜線）</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>其中，<em>xxxx</em>是127以上任何數字的十六進位代碼</p> </td> 
   <td>128+</td> 
   <td>任何超過127的程式碼點均使用Unicode字元</td> 
  </tr> 
 </tbody> 
</table>
