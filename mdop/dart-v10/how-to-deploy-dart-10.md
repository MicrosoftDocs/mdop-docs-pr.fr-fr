---
title: Procédure de déploiement de DaRT10
description: Procédure de déploiement de DaRT10
author: dansimp
ms.assetid: 13e8ba20-21c3-4870-94ed-6d3106d69f21
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: support
ms.sitesec: library
ms.prod: w10
ms.date: 08/30/2016
ms.openlocfilehash: 9e78f55e238cce16798525915487e4b753d92e6c
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10804704"
---
# Procédure de déploiement de DaRT10


Les instructions suivantes décrivent le déploiement de Microsoft Diagnostics and Recovery Tools (DaRT) 10 dans votre environnement. Pour obtenir le logiciel DaRT, reportez-vous à la rubrique [obtention de MDOP](https://go.microsoft.com/fwlink/?LinkId=322049). Il est supposé que vous installez toutes les fonctionnalités sur un ordinateur d’administration. Si vous devez déployer ou désinstaller DaRT 10 sur plusieurs ordinateurs, par exemple à l’aide d’un système de distribution de logiciels électronique, il peut s’avérer plus simple d’utiliser les options d’installation de lignes de commande. Les descriptions et exemples des options de ligne de commande disponibles sont fournis dans cette section.

**Important**  Avant d’installer DaRT, voir [Configurations prises en charge par DART 10](dart-10-supported-configurations.md) pour vérifier que vous avez installé tous les logiciels requis et que votre ordinateur dispose de la configuration minimale requise. L’ordinateur sur lequel vous installez DaRT doit exécuter Windows 10.

 

Vous pouvez installer DaRT en utilisant l’une des deux configurations suivantes:

-   Installez DaRT et tous les outils DaRT sur l’ordinateur d’administration.

-   Installez uniquement sur l’ordinateur d’administration les outils dont vous avez besoin pour créer l’image de récupération DaRT, puis installez la **visionneuse de connexions à distance** et, éventuellement, l' **analyseur d’incidents** sur un ordinateur de bureau d’assistance.

Le fichier d’installation DaRT est disponible dans les versions 32 bits et 64 bits. Installez la version qui correspond à l’architecture de l’ordinateur sur lequel vous exécutez l’Assistant image de récupération DaRT, et non l’architecture informatique de l’image de récupération que vous créez.

Vous pouvez utiliser l’une des versions du fichier d’installation de DaRT pour créer une image de récupération pour les ordinateurs 32 ou 64, mais vous ne pouvez pas créer une image de récupération pour les ordinateurs 32-bits et 64.

**Pour installer DaRT et tous les outils DaRT sur un ordinateur d’administration**

1.  Téléchargez la version 32 bits ou 64 bits du fichier d’installation de DaRT 10. Choisissez l’architecture qui correspond à l’ordinateur sur lequel vous installez DaRT et exécutez l’Assistant image de récupération DaRT.

2.  À partir du dossier dans lequel vous avez téléchargé DaRT 10, exécutez le fichier d’installation **MSDaRT.msi** correspondant à votre configuration système requise.

3.  Dans la page **Bienvenue dans l’Assistant Configuration de Microsoft DART 10** , cliquez sur **suivant**.

4.  Acceptez les termes du contrat de licence logiciel Microsoft, puis cliquez sur **suivant**.

5.  Sur la page **Microsoft Update** , sélectionnez **utiliser Microsoft Update lorsque je recherche des mises à jour**, puis cliquez sur **suivant**.

6.  Dans la page **Sélectionner un dossier d’installation** , sélectionnez un dossier ou cliquez sur **suivant** pour installer DART dans l’emplacement d’installation par défaut.

7.  Sur la page **options d’installation** , sélectionnez les fonctionnalités de DART que vous voulez installer ou cliquez sur **suivant** pour installer DART avec toutes les fonctionnalités.

8.  Pour démarrer l’installation, cliquez sur **installer**.

9.  Lorsque l’installation est terminée, cliquez sur **Terminer** pour quitter l’Assistant.

## Pour installer DaRT et tous les outils DaRT sur un ordinateur d’administration à l’aide d’une invite de commandes


Lors de l’installation ou de la désinstallation de DaRT, vous avez la possibilité d’exécuter les fichiers d’installation à l’invite de commandes. Cette section décrit quelques exemples d’options différentes que vous pouvez spécifier lorsque vous installez ou désinstallez DaRT à l’invite de commandes.

L’exemple suivant montre comment installer toutes les fonctionnalités de DaRT.

``` syntax
msiexec /i MSDaRT.msi ADDLOCAL=CommonFiles, DaRTRecoveryImage,CrashAnalyzer,RemoteViewer 
```

L’exemple suivant montre comment installer uniquement l’Assistant image de récupération DaRT.

``` syntax
msiexec /i MSDaRT.msi ADDLOCAL=CommonFiles, ,DaRTRecoveryImage
```

L’exemple suivant montre comment installer uniquement l’analyseur d’incidents et la visionneuse de connexion à distance DaRT.

``` syntax
msiexec /i MSDaRT.msi ADDLOCAL=CommonFiles,CrashAnalyzer,RemoteViewer 
```

L’exemple suivant crée un journal d’installation pour le programme d’installation de Windows. Cela est utile pour le débogage.

``` syntax
msiexec.exe /i MSDaRT.msi /l*v log.txt 
```

**Remarques**  Vous pouvez ajouter/qn ou/qb pour effectuer une installation silencieuse.

 

**Pour valider l’installation de DaRT**

1.  Cliquez sur **Démarrer**, puis sélectionnez **Diagnostics et outils de récupération**.

    La fenêtre du **jeu d’outils de diagnostics et de récupération** s’ouvre.

2.  Vérifiez que tous les outils DaRT sélectionnés pour l’installation ont été correctement installés.

## Rubriques connexes


[Déploiement de DaRT10 sur les ordinateurs des administrateurs](deploying-dart-10-to-administrator-computers.md)

 

 





