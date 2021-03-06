---
title: Demander la suppression d'un objet de stratégie de groupe
description: Demander la suppression d'un objet de stratégie de groupe
author: dansimp
ms.assetid: 576ece5c-dc6d-4b5e-8628-01c15ae2c9a8
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: manage
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 87368d9f132d1ef7dc6a70fffa0611d33a23aa78
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10807509"
---
# Demander la suppression d'un objet de stratégie de groupe


Sauf si vous êtes approbateur ou administrateur AGPM (contrôle total), vous devez demander la suppression d’un objet de stratégie de groupe.

Un compte d’utilisateur ayant le rôle d’éditeur ou les autorisations nécessaires dans Advanced Group Policy Management (AGPM) est requis pour effectuer cette procédure. Passez en revue les détails dans «autres considérations» dans cette rubrique.

**Pour demander la suppression d’un objet de stratégie de groupe contrôlé**

1.  Dans l’arborescence de la **console de gestion des stratégies de groupe** , cliquez sur modifier le **contrôle** dans la forêt et le domaine dans lesquels vous souhaitez gérer les objets de stratégie de groupe.

2.  Dans l’onglet **contenu** , cliquez sur l’onglet **contrôlé** pour afficher les objets de stratégie de groupe contrôlés.

3.  Cliquez avec le bouton droit sur l’objet de stratégie de groupe que vous voulez supprimer, puis cliquez sur **supprimer**.

    -   Pour supprimer l’objet GPO de l’archive tout en laissant la version déployée de l’objet GPO intact dans l’environnement de production, cliquez sur **Supprimer l’objet GPO de l’archive uniquement**.

    -   Pour supprimer l’objet GPO de l’environnement d’archivage et de production, cliquez sur **Supprimer l’objet GPO de l’archive et**de la production.

4.  Sauf si vous avez une autorisation spéciale pour supprimer des objets de stratégie de groupe, vous devez demander la suppression de l’objet de stratégie de groupe déployé. Pour recevoir une copie de la demande, tapez votre adresse de messagerie dans le champ **CC** . Tapez un commentaire à afficher dans la trace d’audit de l’objet de stratégie de groupe, puis cliquez sur **valider**.

5.  Lorsque la fenêtre de **progression** indique que l’avancement global est terminé, cliquez sur **Fermer**. L’objet de stratégie de groupe est affiché dans la liste des objets de stratégie de groupe de l’onglet **en attente** . Lorsqu’un approbateur a approuvé votre demande, l’objet de stratégie de groupe est déplacé de l’onglet **en attente** vers l’onglet **Corbeille** , où il peut être restauré ou détruit.

### Autres éléments à prendre en considération

-   Par défaut, vous devez être un éditeur pour effectuer cette procédure. Plus précisément, vous devez disposer du **contenu de liste** et des autorisations de **modification des paramètres** pour l’objet de stratégie de groupe.

-   Pour annuler votre demande avant qu’elle ne soit approuvée, cliquez sur l’onglet **en attente** . Cliquez avec le bouton droit sur l’objet, puis cliquez sur **retirer**. L’objet GPO sera renvoyé à l’onglet **contrôlé** .

-   Pour supprimer un objet GPO non contrôlé de l’environnement de production sans le contrôler d’abord, dans la **console de gestion des stratégies de groupe**, cliquez sur **forêt**, cliquez sur **domaines**, sur ** &lt; MyDomain &gt; **, puis cliquez sur objets de stratégie de **groupe**. Cliquez avec le bouton droit sur l’objet de stratégie de groupe non contrôlé, puis cliquez sur **supprimer**.

### Références supplémentaires

-   [Exécution de tâches d'éditeur](performing-editor-tasks-agpm30ops.md)

 

 





