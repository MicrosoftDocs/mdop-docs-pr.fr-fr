---
title: Procédure pour déployer l'image de récupération DaRT sous forme de partition distante
description: Procédure pour déployer l'image de récupération DaRT sous forme de partition distante
author: dansimp
ms.assetid: 06a5e250-b992-4f6a-ad74-e7715f9e96e7
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: support
ms.sitesec: library
ms.prod: w10
ms.date: 08/30/2016
ms.openlocfilehash: 3cdb1313a64bacd652a5253c09f36fa792d0fa3c
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10804698"
---
# Procédure pour déployer l'image de récupération DaRT sous forme de partition distante


Lorsque vous avez fini d’exécuter l’Assistant image de récupération Microsoft Diagnostics et Recovery Tools (DaRT) 10 et créé l’image de récupération, vous pouvez extraire le fichier Boot. wim du fichier image ISO et le déployer en tant que partition distante sur le réseau.

**Pour déployer DaRT 10 en tant que partition distante**

1.  Extrayez le fichier Boot. wim du fichier image ISO DaRT.

    1.  Montez le fichier image ISO que vous avez créé dans la boîte de dialogue **créer une image de démarrage** en utilisant la méthode préférée de montage d’une image par votre entreprise.

    2.  Ouvrez le fichier image ISO et copiez le fichier Boot. wim du dossier \\sources de l’image montée vers un emplacement sur votre ordinateur ou sur un lecteur externe.

        **Remarques**  Si vous avez gravé un CD ou un DVD de l’image de récupération, vous pouvez ouvrir les fichiers sur le CD-ROM ou le DVD et copier le fichier Boot. wim à partir du dossier \\sources. Cela vous permet d’ignorer la nécessité de monter l’image.

         

2.  Déployez le fichier Boot. wim sur un serveur WDS accessible à partir d’ordinateurs d’utilisateurs finaux de votre entreprise.

3.  Configurez le serveur WDS pour qu’il utilise le fichier Boot. wim pour DaRT en suivant les procédures de déploiement standard de WDS.

Pour plus d’informations sur le déploiement de DaRT en tant que partition distante, voir [procédure pas à pas: déploiement d’une image à l’aide](https://go.microsoft.com/fwlink/?LinkId=212108) du Guide de mise en route de PXE et [Windows Deployment Services](https://go.microsoft.com/fwlink/?LinkId=212106).

## Rubriques connexes


[Création de l'image de récupération DaRT10](creating-the-dart-10-recovery-image.md)

[Déploiement de l'image de récupération DaRT](deploying-the-dart-recovery-image-dart-10.md)

[Planification de DaRT10](planning-for-dart-10.md)

 

 





