---
title: Déploiement d'App-V5.0 Sequencer et Client
description: Déploiement d'App-V5.0 Sequencer et Client
author: dansimp
ms.assetid: 84cc84bd-5bc0-41aa-9519-0ded2932c078
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop, appcompat, virtualization
ms.mktglfcycl: deploy
ms.sitesec: library
ms.prod: w10
ms.date: 06/21/2016
ms.openlocfilehash: 647ea12018bf966592b9e831d532c7c08093d367
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10805845"
---
# Déploiement d'App-V5.0 Sequencer et Client


Le client et le Sequencer App-V 5,0 permettent aux administrateurs de virtualiser et d’exécuter des applications virtualisées.

## Déployer le client


Le client App-V 5,0 est le composant qui exécute une application virtualisée sur un ordinateur cible. Le client permet aux utilisateurs d’interagir avec des icônes et de double-cliquer sur les types de fichiers de sorte qu’ils puissent démarrer une application virtualisée. Le client peut également obtenir le contenu de l’application virtuelle à partir du serveur de gestion.

[Comment déployer App-V Client](how-to-deploy-the-app-v-client-gb18030.md)

[Procédure pour désinstaller App-V5.0 Client](how-to-uninstall-the-app-v-50-client.md)

[Déploiement de l’application-V 4,6 et du client App-V 5,0 sur le même ordinateur](how-to-deploy-the-app-v-46-and-the-app-v--50-client-on-the-same-computer.md)

## Paramètres de configuration du client


Le client App-V 5,0 stocke sa configuration dans le registre. Vous pouvez recueillir des informations utiles sur le client si vous comprenez le format des données dans le registre. Vous pouvez également configurer de nombreuses actions client en modifiant des entrées de registre.

[À propos des paramètres de configuration du client](about-client-configuration-settings.md)

## Configurer le client à l’aide du modèle ADMX et de la stratégie de groupe


Vous pouvez utiliser le modèle Microsoft ADMX pour configurer les paramètres du client de l’application-V 5,0 et du client de services Bureau à distance. Le modèle ADMX gère les configurations client courantes à l’aide d’une infrastructure de stratégie de groupe existante et comprend des paramètres pour la configuration du client App-V 5,0.

**Important**  Vous pouvez obtenir le modèle App-V 5,0 ADMX à partir du centre de téléchargement Microsoft.

 

Après avoir téléchargé et installé le modèle ADMX, vous devez effectuer les étapes suivantes sur l’ordinateur que vous utiliserez pour gérer la stratégie de groupe. Il s’agit généralement du contrôleur de domaine.

1.  Enregistrez le fichier **. admx** dans le répertoire suivant: **Windows \ \ PolicyDefinitions**

2.  Enregistrez le fichier **. adml** dans le répertoire suivant: **Windows \ \ PolicyDefinitions \ \ &lt; Language Directory &gt; **

Après avoir effectué les étapes ci-dessus, vous pouvez gérer les paramètres de configuration du client App-V 5,0 avec la console de **gestion des stratégies de groupe** .

Le client App-V 5,0 stocke également sa configuration dans le registre. Vous pouvez recueillir des informations utiles sur le client si vous comprenez le format des données dans le registre. Vous pouvez également configurer de nombreuses actions client en modifiant des entrées de registre.

[Modification de la configuration d'App-V5.0 Client à l'aide du modèle ADMX et d'une stratégie de groupe](how-to-modify-app-v-50-client-configuration-using-the-admx-template-and-group-policy.md)

## Déploiement du client à l’aide du mode magasin de contenu partagé


Le mode SCS (Data content Store) App-V 5,0 permet aux clients de l' 5,0 application SCS d’exécuter des applications virtuelles sans enregistrer les données de package associées localement. Toutes les données du package virtualisé requises sont transmises sur le réseau; par conséquent, vous devez utiliser le mode SCS uniquement dans les environnements dotés d’une connexion rapide. Les services Bureau à distance et la version standard du client App-V 5,0 sont tous deux pris en charge en mode SCS.

**Important**  Si le client App-V 5,0 est configuré pour s’exécuter en mode SCS, l’emplacement à partir duquel les packages App-V 5,0 doivent être diffusés doit être disponible; dans le cas contraire, le package virtuel ne fonctionnera pas. Par ailleurs, nous déconseillons le déploiement d’applications virtualisées sur les ordinateurs qui exécutent le client App-V 5,0 en mode SCS sur Internet.

 

Par ailleurs, le SCS n’est pas un emplacement physique contenant des packages virtualisés. C’est un mode qui permet au client App-V 5,0 de diffuser les données du package virtualisé requis sur le réseau.

Le mode SCS est utile dans les cas suivants:

-   Déploiements VDI (Virtual Desktop Infrastructure)

-   Déploiements de services Bureau à distance

Pour utiliser SCS dans votre environnement, vous devez activer le client App-V 5,0 pour qu’il s’exécute en mode SCS. Ce paramètre doit être spécifié lors de l’installation. Par défaut, le client n’est pas configuré pour utiliser le mode SCS. Vous devriez installer le client en suivant la procédure suggérée si vous envisagez d’utiliser SCS. Toutefois, vous pouvez configurer un client App-V 5,0 existant pour qu’il s’exécute en mode SCS en entrant la commande PowerShell suivante sur l’ordinateur exécutant le client App-V 5,0:

**Set-AppvClientConfiguration-SharedContentStoreMode 1**

Il peut arriver que l’administrateur précharge certaines applications virtuelles sur l’ordinateur qui exécute le client App-V 5,0 en mode SCS. Pour ce faire, vous pouvez utiliser les commandes PowerShell pour ajouter, publier et monter le package. Par exemple, si un package est préinstallé sur tous les ordinateurs, l’administrateur peut ajouter, publier et monter le package à l’aide de commandes PowerShell. Le package n’est pas diffusé sur le réseau, car il est stocké localement.

[Installation d'App-V5.0 Client pour le mode Magasin de contenu partagé](how-to-install-the-app-v-50-client-for-shared-content-store-mode.md)

## Déployer le Sequencer


Le Sequencer est un outil qui permet de convertir des applications standard en packages virtuels pour le déploiement sur des ordinateurs exécutant le client App-V 5,0. Le Sequencer permet de fournir un processus de conversion simple et prévisible avec des modifications minimales apportées aux flux de travail de séquençage antérieur. De plus, le Sequencer permet aux utilisateurs de configurer plus facilement des applications afin d’activer les connexions d’applications virtualisées.

Pour obtenir la liste des modifications apportées au Sequencer App-V 5,0, voir [Nouveautés de l’app-v 5,0](whats-new-in-app-v-50.md).

[Installation de Sequencer](how-to-install-the-sequencer-beta-gb18030.md)

## <a href="" id="---------app-v-5-0-client-and-sequencer-logs"></a> Journal des clients App-V 5,0 et Sequencer


Vous pouvez utiliser les informations du journal de Sequencer App-V 5,0 pour résoudre les problèmes liés à l’installation de Sequencer et aux événements opérationnels lors de l’utilisation d’App-V 5,0. Les informations du journal relatives au Sequencer peuvent être examinées avec l' **Observateur d’événements**. La ligne suivante affiche le chemin d’accès spécifique pour les événements liés au Sequencer:

**Journaux de l’observateur d’événements \ \ applications et services** Les événements liés au Sequencer sont précédés de **AppV \ _Sequencer**. Les événements liés au client sont précédés de **AppV \ _Client**.

Dans App-V 5,0 SP3, certains journaux ont été consolidés. Voir [à propos de App-V 5,0 SP3](about-app-v-50-sp3.md#bkmk-event-logs-moved).

## Autres ressources pour le déploiement de Sequencer et de client


[Déploiement d'App-V5.0](deploying-app-v-50.md)

[Planification d'App-V5.0](planning-for-app-v-50-rc.md)






 

 





