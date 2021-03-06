---
title: Procédure pour déployer l'image de récupération DaRT dans le cadre d'une partition de récupération
description: Procédure pour déployer l'image de récupération DaRT dans le cadre d'une partition de récupération
author: dansimp
ms.assetid: 07c5d539-51d9-4759-adc7-72b40d5d7bb3
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: support
ms.sitesec: library
ms.prod: w10
ms.date: 08/30/2016
ms.openlocfilehash: e3647d684f64a0635e2875314498bde841204369
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10810523"
---
# Procédure pour déployer l'image de récupération DaRT dans le cadre d'une partition de récupération


Lorsque vous avez terminé d’exécuter l’Assistant image de récupération de Microsoft Diagnostics et Recovery Tools (DaRT) 8,0 et créé l’image de récupération, vous pouvez extraire le fichier Boot. wim du fichier image ISO et le déployer en tant que partition de récupération dans une image Windows 8. Il est recommandé d’utiliser une partition, car tous les problèmes d’endommagement qui empêchent le système d’exploitation Windows de démarrer pourraient empêcher l’image de récupération de démarrer. Par ailleurs, une partition séparée évite d’avoir recours à la clé de récupération BitLocker. Envisagez de masquer la partition pour empêcher les utilisateurs de stocker des fichiers sur celle-ci.

**Pour déployer DaRT dans la partition de récupération d’une image Windows 8**

1.  Créez une partition cible dans votre image Windows 8 égale ou supérieure à la taille du fichier image ISO que vous avez créé à l’aide de l' **Assistant image de récupération 8,0 de DART**.

    La taille minimale requise pour une partition DaRT est de 500 Mo pour s’adapter à la fonctionnalité de connexion à distance dans DaRT.

2.  Extrayez le fichier Boot. wim du fichier image ISO DaRT.

    1.  À l’aide de la méthode préférée de votre entreprise, montez le fichier image ISO que vous avez créé dans la page **créer une image de démarrage** .

    2.  Ouvrez le fichier image ISO et copiez le fichier Boot. wim du dossier \\sources de l’image montée vers un emplacement sur votre ordinateur ou sur un lecteur externe.

        **Remarques**  Si vous avez gravé un CD, un DVD ou une connexion USB de l’image de récupération, vous pouvez ouvrir les fichiers sur le média amovible et copier le fichier Boot. wim à partir du dossier \\sources. Si vous copiez le fichier Boot. wim, vous n’avez pas besoin de monter l’image.

         

3.  Utilisez le fichier Boot. wim pour créer une partition de récupération démarrable en utilisant la méthode standard de votre entreprise pour créer une image Windows RE personnalisée.

    Pour plus d’informations sur la création et la personnalisation d’une partition de récupération, voir [Personnalisation de l’utilisation de Windows RE](https://go.microsoft.com/fwlink/?LinkId=214222).

4.  Remplacez la partition cible dans votre image Windows 8 par la partition de récupération.

    Pour plus d’informations sur le déploiement d’une solution de récupération pour réinstaller l’image de fabrique en cas de panne du système, voir [déployer une image de récupération du système](https://go.microsoft.com/fwlink/?LinkId=214221).

## Rubriques connexes


[Création de l'image de récupération DaRT8.0](creating-the-dart-80-recovery-image-dart-8.md)

[Déploiement de l'image de récupération DaRT](deploying-the-dart-recovery-image-dart-8.md)

[Planification de DaRT8.0](planning-for-dart-80-dart-8.md)

 

 





