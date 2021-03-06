---
title: Comment créer un groupe de connexion
description: Comment créer un groupe de connexion
author: dansimp
ms.assetid: 9d272052-2d28-4e41-989c-89610482a0ca
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop, appcompat, virtualization
ms.mktglfcycl: deploy
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 816fc3b37be056ed54a88c394ef64fa1edaf47ee
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10805653"
---
# Comment créer un groupe de connexion


Suivez ces étapes pour créer un groupe de connexion à l’aide de la console de gestion App-V. Pour utiliser PowerShell afin de créer des groupes de connexion, reportez-vous [à la rubrique Comment gérer les groupes de connexion sur un ordinateur autonome à l’aide de PowerShell](how-to-manage-connection-groups-on-a-stand-alone-computer-by-using-powershell.md).

Lorsque vous placez des packages dans un groupe de connexions, leurs chemins d’accès racines de package sont fusionnés. Si vous supprimez des packages, seuls les packages restants maintiennent la racine fusionnée.

**Pour créer un groupe de connexions**

1.  Dans la console de gestion App-V 5,0, sélectionnez **packages**.

2.  Sélectionnez **groupes de connexion** pour afficher la bibliothèque de groupes de connexion.

3.  Pour créer un groupe de connexion, sélectionnez **Ajouter un groupe de connexion** .

4.  Dans le volet **nouveau groupe de connexions** , tapez une description pour le groupe.

5.  Cliquez sur **modifier** dans le volet **packages connectés** pour ajouter une nouvelle application au groupe de connexion.

6.  Dans le volet **bibliothèque entière** , sélectionnez l’application que vous voulez ajouter, puis cliquez sur la flèche pour ajouter l’application.

    Pour supprimer une application, sélectionnez l’application à supprimer dans le volet **packages dans** , puis cliquez sur la flèche.

    Pour redéfinir la priorité des applications de votre groupe de connexion, utilisez les flèches du volet **packages dans** .

    **Important**  Par défaut, les configurations d’accès aux services de domaine Active Directory associées à une application spécifique ne sont pas ajoutées au groupe de connexions. Pour transférer la configuration de l’accès Active Directory, sélectionnez **Ajouter l’accès au package à l’accès au groupe**, qui se trouve dans le volet **packages dans** .

     

7.  Après avoir ajouté toutes les applications et configuré l’accès Active Directory, cliquez sur **appliquer**.

    Vous **avez une suggestion pour App-V**? Ajoutez ou Votez en fonction [de suggestions.](http://appv.uservoice.com/forums/280448-microsoft-application-virtualization) **Vous avez un problème lié à l’application-V?** Utilisez le [Forum TechNet App-V](https://social.technet.microsoft.com/Forums/home?forum=mdopappv).

## Rubriques connexes


[Opérations d'App-V5.0](operations-for-app-v-50.md)

[Gestion des groupes de connexion](managing-connection-groups.md)

 

 





