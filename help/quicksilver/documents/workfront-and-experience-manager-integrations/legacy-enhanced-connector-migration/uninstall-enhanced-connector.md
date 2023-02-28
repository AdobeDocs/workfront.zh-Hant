---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 解除安裝Workfront for Adobe Experience Manager enhanced connector
description: 您必須將Workfront與Adobe Experience Manager Enhanced Connector解除安裝，以便連接Workfront和Adobe Experience Manager Assets的最新原生整合as a Cloud Service。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 9673009f12509b5e7051ee91e142d311f333f215
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 解除安裝Workfront與Adobe Experience Manager增強連接器

您必須將Workfront與Adobe Experience Manager Enhanced Connector解除安裝，以便連接Workfront和Adobe Experience Manager Assets的最新原生整合as a Cloud Service。

## 必要條件

* （選用）如有需要，請還原對Workfront防火牆設定和AEM Dispatcher設定所做的任何變更。

## 卸載增強連接器

1. 從Cloud Manager存取及複製AEMas a Cloud Service存放庫。

1. 在您選擇的IDE中，開啟您複製的Git存放庫。

1. 檢查安裝增強連接器的分支。

1. 導覽至下列路徑，並移除增強的連接器zip檔案：

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. 從專案根目錄的pom.xml檔案中移除下列相依性。

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >請確定上述程式碼區塊中參考的版本（即1.8.0）反映的是從程式碼中解除安裝的版本。

1. 從項目子模組的pom.xml檔案(名為 **all**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. 從項目子模組的pom.xml檔案（名為all）中刪除嵌入的以下內容。

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. （條件性）從專案根目錄的pom.xml檔案中移除存放庫設定。


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. （條件性）從下列路徑顯示的settings.xml中移除伺服器設定。/cloudmanager/maven/settings.xml（在項目根目錄中）。

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. 提交變更，並將程式碼推送至Cloud Manager存放庫

1. 執行Cloud Manager管道以在您的Cloud Services執行個體上部署變更
