---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 解除安裝Workfront for Adobe Experience Manager增強型聯結器
description: 您必須解除安裝Workfront with Adobe Experience Manager增強型聯結器，以連線至連線Workfront和Adobe Experience Manager Assetsas a Cloud Service的最新原生整合。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 9673009f12509b5e7051ee91e142d311f333f215
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# 解除安裝具有Adobe Experience Manager增強型聯結器的Workfront

您必須解除安裝Workfront with Adobe Experience Manager增強型聯結器，以連線至連線Workfront和Adobe Experience Manager Assetsas a Cloud Service的最新原生整合。

## 先決條件

* （選用）如有必要，請還原對Workfront防火牆設定和AEM Dispatcher設定所做的任何變更。

## 解除安裝增強型聯結器

1. 從Cloud Manager存取及複製AEM as a Cloud Service存放庫。

1. 在您選擇的IDE中開啟複製的Git存放庫。

1. 簽出安裝增強型聯結器的分支。

1. 導覽至下列路徑，並移除增強型聯結器zip檔案：

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
   >請確定上述程式碼區塊中參照的版本（即1.8.0）反映了要從程式碼解除安裝的版本。

1. 從專案名為&#x200B;**all**&#x200B;的子模組的pom.xml檔案中移除下列相依性。

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. 從專案名為all的子模組的pom.xml檔案中移除下列內嵌專案。

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. （視條件而定）從專案根目錄的pom.xml檔案中移除存放庫組態。


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. （條件式）從settings.xml移除伺服器組態，此組態出現在以下路徑中。/cloudmanager/maven/settings.xml在專案根目錄中。&#39;

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

1. 提交變更，並將程式碼推送到Cloud Manager存放庫

1. 執行Cloud Manager管道以在Cloud Service執行個體上部署變更
