---
title: Étiqueter la version actuelle d'un objet de stratégie de groupe
description: Étiqueter la version actuelle d'un objet de stratégie de groupe
author: dansimp
ms.assetid: cadc8769-21da-44b0-8122-6cafdb448913
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: manage
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: b15a4d3ee006fb37db4ce7362a2f5c92d7c233e5
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10808397"
---
# Étiqueter la version actuelle d'un objet de stratégie de groupe


Vous pouvez étiqueter la version actuelle d’un objet de stratégie de groupe pour faciliter l’identification de son historique. Vous pouvez utiliser une étiquette pour identifier une version correcte connue vers laquelle vous pouvez revenir en cas de problème. Par ailleurs, en attribuant une étiquette à plusieurs objets de stratégie de groupe avec la même étiquette à la fois, vous pouvez marquer les objets de stratégie de groupe associés qui doivent être restaurés au même point si la restauration doit être nécessaire ultérieurement.

Un compte d’utilisateur ayant le rôle d’éditeur, d’approbateur ou d’administrateur AGPM (contrôle total) ou les autorisations nécessaires dans Advanced Group Policy Management (AGPM) est requis pour effectuer cette procédure. Passez en revue les détails dans «autres considérations» dans cette rubrique.

**Pour étiqueter la version actuelle d’objets de stratégie de groupe dans leur historique**

1.  Dans l’arborescence de la **console de gestion des stratégies de groupe** , cliquez sur modifier le **contrôle** dans la forêt et le domaine dans lesquels vous souhaitez gérer les objets de stratégie de groupe.

2.  Dans l’onglet **contenu** , cliquez sur l’onglet **contrôlé** pour afficher les objets de stratégie de groupe contrôlés.

3.  Cliquez sur un objet de stratégie de groupe pour lequel étiqueter la version actuelle. Pour sélectionner plusieurs objets de stratégie de groupe, appuyez sur Maj et cliquez sur le dernier objet GPO d’un groupe contigu d’objets de stratégie de groupe, ou appuyez sur CTRL et cliquez sur objets de stratégie de groupe individuels. Cliquez avec le bouton droit sur un objet de stratégie de groupe sélectionné, puis cliquez sur **étiquette**.

4.  Tapez une étiquette et un commentaire à afficher dans l’historique de chaque GPO sélectionné, puis cliquez sur **OK**.

5.  Lorsque la fenêtre de **progression** indique que l’avancement global est terminé, cliquez sur **Fermer**.

### Autres éléments à prendre en considération

-   Par défaut, vous devez être un éditeur, un approbateur ou un administrateur AGPM (contrôle total) pour effectuer cette procédure. Plus précisément, vous devez disposer du contenu de la **liste** et **modifier les paramètres** ou les autorisations de l’objet de **stratégie** de groupe pour l’objet GPO.

### Références supplémentaires

-   [Modification d'un objet de stratégie de groupe](editing-a-gpo-agpm40.md)

 

 





