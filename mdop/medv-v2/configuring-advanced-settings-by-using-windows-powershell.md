---
title: Configuration de paramètres avancés à l'aide de Windows PowerShell
description: Configuration de paramètres avancés à l'aide de Windows PowerShell
author: dansimp
ms.assetid: 437a31cc-2a11-456f-b448-b0b869fb53f7
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop, virtualization
ms.mktglfcycl: deploy
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 45a3ece3f76f6e982913aad2b25cfe0084542f32
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10812329"
---
# Configuration de paramètres avancés à l'aide de Windows PowerShell


Le package d’espace de travail MED-V que vous créez inclut un fichier de script Windows PowerShell (. ps1) que vous pouvez modifier avant de tester et de déployer votre package d’espace de travail MED-V. Cette section fournit des informations et des conseils pour vous aider à gérer les paramètres de configuration de MED-V à l’aide de Windows PowerShell avant de déployer les espaces de travail MED-V.

## Utilisation des cmdlets Windows PowerShell dans MED-V


Les applets de commande Windows PowerShell suivantes sont disponibles dans Microsoft Enterprise Desktop Virtualization (MED-V) 2,0:

**Nouveau-MedvConfiguration**

**Export-MedvConfiguration**

**Nouveau-MedvWorkspace**

**Export-MedvWorkspace**

Pour accéder aux cmdlets Windows PowerShell pour MED-V, ouvrez Windows PowerShell, puis tapez la commande suivante pour importer les modules MED-V.

``` syntax
Import-Module microsoft.medv
```

Une fois les modules importés, vous pouvez accéder à l’aide incluse pour les applets de commande en utilisant les commandes **standard de l'** **aide de Windows PowerShell.** Par exemple, pour accéder à une description de l’applet **de commande New-MedvConfiguration** et obtenir la liste complète des paramètres disponibles, tapez la commande suivante.

``` syntax
get-help New-MedvConfiguration
```

Vous pouvez également afficher l’aide de paramètres spécifiques. Par exemple, pour afficher l’aide du paramètre VmMemory, tapez ce qui suit:

``` syntax
get-help New-MedvConfiguration -parameter VmMemory
```

Pour afficher la liste de tous les paramètres de configuration de MED-V et leurs valeurs par défaut, tapez la commande suivante.

``` syntax
New-MedvConfiguration -ForceDefaults
```

Pour afficher la liste de tous les paramètres de configuration de MED-V et leurs valeurs actuelles, tapez la commande suivante.

``` syntax
gwmi -Class "Setting” -Namespace "root/microsoft/medv”
```

## Création d’un espace de travail MED-V avec des paramètres personnalisés


Une fois que vous avez créé un package d’espace de travail MED-V en utilisant le gestionnaire de package MED-V, un script Windows PowerShell est généré dans le dossier que vous avez spécifié pour l’enregistrement de vos fichiers de package. Le contenu de ce script présente certains des paramètres de configuration MED-V que vous pouvez modifier.

Après avoir suivi ces étapes, vous pouvez personnaliser le script puis l’exécuter dans Windows PowerShell pour créer un espace de travail MED-V avec les nouveaux paramètres.

**Important**  Exécutez Windows PowerShell avec des informations d’identification d’administration, et assurez-vous que la stratégie d’exécution Windows PowerShell autorise l’exécution de scripts.

1.  Modifiez le script Windows PowerShell généré par le module de création de package de l’espace de travail MED-V, ou créez un nouveau script avec les paramètres de configuration de votre choix.

2.  Exécutez Windows PowerShell avec des informations d’identification d’administration, puis à l’invite de commandes, tapez la commande suivante.

    ``` syntax
    & “.\<workspacename>.ps1”
    ```

    Cette commande exécute le script Windows PowerShell et exécute l’applet de commande **New-MedvWorkspace** pour générer un nouveau package d’espace de travail MED-V. Les nouveaux fichiers du gestionnaire de package sont enregistrés dans le dossier que vous avez spécifié à l’origine pour le stockage de vos fichiers de package de package d’espace de travail MED-V. Pour obtenir de l’aide supplémentaire sur cette cmdlet, voir l’aide de Windows PowerShell.

 

## Exportation d’une configuration MED-V vers un fichier de Registre


Vous pouvez mettre à jour les paramètres de configuration de MED-V après l’installation de l’espace de travail MED-V. Utilisez l’applet de nouvelle applet de **MedvConfiguration** pour spécifier les paramètres que vous voulez modifier. Par exemple, pour créer un fichier de Registre qui modifie le paramètre de mémoire de l’ordinateur virtuel, tapez les commandes suivantes.

``` syntax
New-MedvConfiguration  -VmMemory 1024 | Export-MedvConfiguration -Path c:\medvConfiguration\myConfig.reg
```

Vous pouvez importer le fichier de Registre résultant de l’ordinateur hôte dans un espace de travail MED-V pour appliquer les nouveaux paramètres de configuration.

## Rubriques connexes


[Gestion des paramètres de configuration d'espace de travail MED-V](managing-med-v-workspace-configuration-settings.md)

[Tester et déployer le package d'espace de travail MED-V](test-and-deploy-the-med-v-workspace-package.md)

 

 





