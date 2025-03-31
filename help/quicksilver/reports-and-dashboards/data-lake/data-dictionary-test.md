---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: 建立Snowflake的讀者帳戶
description: 若要存取Data Connect資料，您必須先建立Snowflake讀取器帳戶。
author: Courtney
feature: Reports and Dashboards
hide: true
hidefromtoc: true
source-git-commit: a42c13804b0463af27bac6f9166bc6e3c41d3fda
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 8%

---


# 測試

## 存取層級

<table>
  <thead>
    <tr>
        <th>Workfront實體名稱</th>
        <th>介面參考</th>
        <th>API參考 | 標籤</th>
        <th>資料湖檢視</th>
    </tr>
  </thead>
 <tr>
        <td>存取層級</td>
         <td>存取層級</td>
        <td>ACSLVL | 存取層級</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong>關聯性欄位</strong> <br>
         ACCESSLEVELID （自我）：自我<br>
         APPGLOBALID：不是關聯性；用於內部應用程式<br>
         LASTUPDATEDBYID： USER_CURRENT | 使用者ID<br>
         LEGACYACCESSLEVELID：不是關聯性；用於內部應用程式<br>
         OBJID： OBJCODE欄位<br>中識別的物件識別碼
         SYSID：不是關聯性；用於內部應用程式</td>
    </tr>
</table>

## 存取層級

<table>
  <thead>
    <tr>
        <th>Workfront實體名稱</th>
        <th>介面參考</th>
        <th>API參考 | 標籤</th>
        <th>資料湖檢視</th>
    </tr>
  </thead>
 <tr>
        <td>存取層級</td>
         <td>存取層級</td>
        <td>ACSLVL | 存取層級</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong>關聯性欄位</strong> <br>
         <ul>
            <li>ACCESSLEVELID (self)： Self</li>
            <li>APPGLOBALID：不是關係；用於內部應用程式用途</li>
            <li>LASTUPDATEDBYID： USER_CURRENT | 使用者ID</li>
            <li>LEGACYACCESSLEVELID：不是關係；用於內部應用程式用途</li>
            <li>OBJID：在OBJCODE欄位中識別的物件識別碼</li>
            <li>SYSID：不是關聯性；用於內部應用程式</li>
        </ul>
    </tr>
</table>