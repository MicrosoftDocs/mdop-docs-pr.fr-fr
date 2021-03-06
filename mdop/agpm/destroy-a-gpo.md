---
title: Détruire un objet de stratégie de groupe
description: Détruire un objet de stratégie de groupe
author: dansimp
ms.assetid: d74941a3-beef-46cd-a4ca-80a324dcfadf
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: manage
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 5545918c417fce16bfc2369ebc6fc2199390adc6
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10807590"
---
# Détruire un objet de stratégie de groupe


La gestion avancée de la stratégie de groupe permet aux approbateurs de détruire un objet de stratégie de groupe, de le supprimer de la corbeille et de le supprimer définitivement pour qu’il ne puisse plus être restauré.

Un compte d’utilisateur ayant le rôle d’approbateur ou d’administrateur AGPM (contrôle total) ou les autorisations nécessaires dans la gestion avancée de la stratégie de groupe est requis pour effectuer cette procédure. Passez en revue les détails dans «autres considérations» dans cette rubrique.

**Pour supprimer définitivement un objet GPO de sorte qu’il ne puisse plus être restauré**

1.  Dans l’arborescence de la **console de gestion des stratégies de groupe** , cliquez sur modifier le **contrôle** dans la forêt et le domaine dans lesquels vous souhaitez gérer les objets de stratégie de groupe.

2.  Dans l’onglet **contenu** , cliquez sur l’onglet **Corbeille** pour afficher les objets de stratégie de groupe supprimés.

3.  Cliquez avec le bouton droit sur l’objet de stratégie de groupe à supprimer, puis cliquez sur **détruire**.

4.  Cliquez sur **Oui** pour confirmer que vous voulez supprimer définitivement l’objet de stratégie de groupe sélectionné et toutes les sauvegardes de l’archive.

5.  Lorsque la fenêtre de **progression** indique que l’avancement global est terminé, cliquez sur **Fermer**. L’objet de stratégie de groupe est supprimé de l’onglet **Corbeille** et est supprimé de manière définitive.

### Autres éléments à prendre en considération

-   Par défaut, vous devez être approbateur ou administrateur AGPM (contrôle total) pour effectuer cette procédure. Plus précisément, vous devez disposer d’autorisations de **liste** et de **Suppression d’objets** de stratégie de groupe pour l’objet GPO.

### Références supplémentaires

-   [Suppression, restauration ou destruction d'un objet de stratégie de groupe](deleting-restoring-or-destroying-a-gpo.md)

 

 





