---
title: Récupération des ordinateurs à l'aide de DaRT8.0
description: Récupération des ordinateurs à l'aide de DaRT8.0
author: dansimp
ms.assetid: 0caeb7d9-c1e6-4f32-bc27-157b91630989
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: support
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 39bab02488252b53deb971d35bc6872c0a2df73b
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10810812"
---
# Récupération des ordinateurs à l'aide de DaRT8.0


Après le déploiement de l’image de récupération du jeu d’outils de diagnostics et de récupération Microsoft (DaRT) 8,0, vous pouvez utiliser DaRT 8,0 pour récupérer des ordinateurs. Les informations contenues dans cette section décrivent les tâches de récupération que vous pouvez effectuer.

Vous avez le choix entre différentes méthodes pour démarrer DaRT, en fonction du déploiement de l’image de récupération DaRT.

-   Insérez un CD, un DVD ou un lecteur flash USB dans l’ordinateur défectueux, puis utilisez-le pour démarrer l’ordinateur.

-   Démarrez dans DaRT à partir d’une partition de récupération sur l’ordinateur qui pose problème.

-   Démarrez dans DaRT à partir d’une partition distante sur le réseau.

Pour plus d’informations sur les avantages et inconvénients de chaque méthode, voir [planification de l’enregistrement et du déploiement de l’image de récupération 8,0 de DART](planning-how-to-save-and-deploy-the-dart-80-recovery-image-dart-8.md).

Quelle que soit la méthode que vous utilisez pour démarrer dans DaRT, vous devez activer le périphérique de démarrage dans le BIOS pour l’option de démarrage ou les options que vous voulez mettre à disposition de l’utilisateur final.

**Remarques**  La configuration du BIOS est unique, en fonction du type de disque dur, de cartes réseau et d’autres éléments utilisés au sein de votre organisation.

 

## Récupérer un ordinateur local à l’aide de l’image de récupération DaRT


Pour récupérer un ordinateur local à l’aide de DaRT, vous devez avoir une présentation physique de l’ordinateur de l’utilisateur final rencontrant des problèmes qui nécessitent DaRT.

[Procédure pour récupérer des ordinateurs locaux à l'aide de l'image de récupération DaRT](how-to-recover-local-computers-by-using-the-dart-recovery-image-dart-8.md)

## Récupérer un ordinateur distant à l’aide de l’image de récupération DaRT


Grâce à la fonctionnalité de connexion à distance de DaRT, un administrateur informatique exécute les outils DaRT à distance sur un ordinateur d’utilisateur final. Lorsque certaines informations sont fournies par l’utilisateur final (ou par un professionnel du support technique travaillant sur l’ordinateur de l’utilisateur final), l’administrateur informatique ou le service de support technique peut prendre le contrôle de l’ordinateur de l’utilisateur final et exécuter les outils DaRT nécessaires à distance.

**Important**  Les deux ordinateurs qui établissent une connexion à distance doivent faire partie du même réseau.

 

La fenêtre du **jeu d’outils de diagnostics et de récupération** inclut la possibilité d’exécuter le DART sur un ordinateur d’utilisateur final à distance à partir d’un ordinateur d’administration. L’utilisateur final ouvre les outils DaRT sur le problème et démarre la session à distance en cliquant sur **connexion à distance**.

La fonctionnalité de connexion à distance sur l’ordinateur de l’utilisateur final crée les informations de connexion suivantes: un numéro de ticket, un port et une liste de toutes les adresses IP disponibles. Le numéro de ticket et le port sont générés de manière aléatoire.

L’administrateur informatique ou le service de support technique entre les informations dans la **visionneuse de connexion à distance DART** pour établir la connexion aux services Terminal Server à l’ordinateur de l’utilisateur final. La connexion de services Terminal Server établie permet à un administrateur informatique d’interagir à distance avec les outils DaRT sur l’ordinateur de l’utilisateur final. L’ordinateur de l’utilisateur final traite alors les informations de connexion, partage son écran et répond aux instructions de l’ordinateur de l’administrateur informatique.

[Procédure pour récupérer des ordinateurs distants à l'aide de l'image de récupération DaRT](how-to-recover-remote-computers-by-using-the-dart-recovery-image-dart-8.md)

## Autres ressources pour récupérer des ordinateurs à l’aide de DaRT 8,0


[Opérations de DaRT8.0](operations-for-dart-80-dart-8.md)

 

 





