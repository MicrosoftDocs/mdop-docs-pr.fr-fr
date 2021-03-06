---
title: Déléguer la gestion d'un objet de stratégie de groupe contrôlé
description: Déléguer la gestion d'un objet de stratégie de groupe contrôlé
author: dansimp
ms.assetid: 509b02e7-ce0b-4919-b58a-c3a33051152e
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: manage
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 9d34231f25c172951cd0176b3e490dab84b98f1d
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10807618"
---
# Déléguer la gestion d'un objet de stratégie de groupe contrôlé


Un approbateur peut déléguer la gestion d’un objet de stratégie de groupe contrôlé (GPO) qui a été créé par cet approbateur. À l’instar d’un administrateur AGPM (contrôle total), l’approbateur peut déléguer l’accès à un tel objet GPO de telle sorte que les éditeurs sélectionnés puissent le modifier, les réviseurs pourront le consulter et permettre à d’autres approbateurs de l’approuver. Par défaut, un approbateur ne peut pas déléguer l’accès aux objets de stratégie de groupe créés par un autre administrateur de stratégie de groupe.

Un compte d’utilisateur ayant le rôle d’administrateur AGPM (contrôle total), le compte d’utilisateur de l’approbateur qui a créé l’objet de stratégie de groupe ou un compte d’utilisateur disposant des autorisations nécessaires dans Advanced Group Policy Management (AGPM) est requis pour effectuer cette procédure. Passez en revue les détails dans «autres considérations» dans cette rubrique.

**Pour déléguer la gestion d’un objet de stratégie de groupe contrôlé**

1.  Dans l’arborescence de la **console de gestion des stratégies de groupe** , cliquez sur modifier le **contrôle** dans la forêt et le domaine dans lesquels vous souhaitez gérer les objets de stratégie de groupe.

2.  Dans l’onglet **Sommaire** du volet Détails, cliquez sur l’onglet **contrôlé** pour afficher les objets de stratégie de groupe contrôlés, puis cliquez sur l’objet de stratégie de groupe à déléguer:

    1.  Pour ajouter l’accès d’un utilisateur ou d’un groupe, cliquez sur le bouton **Ajouter** , sélectionnez l’utilisateur ou le groupe, puis cliquez sur **OK**. Dans la boîte de dialogue **Ajouter un groupe ou un utilisateur** , sélectionnez un rôle, puis cliquez sur **OK**.

    2.  Pour supprimer l’accès d’un utilisateur ou d’un groupe, sélectionnez-le, puis cliquez sur le bouton **supprimer** .

        **Remarques**  Si un utilisateur ou un groupe hérite de l’accès à l’échelle du domaine, le bouton **supprimer** n’est pas disponible. Vous pouvez modifier l’accès à l’échelle du domaine sous l’onglet **délégation de domaine** .

         

    3.  Pour modifier les rôles et autorisations délégués à un utilisateur ou à un groupe, cliquez sur le bouton **avancé** . Dans la boîte de dialogue **autorisations** , sélectionnez l’utilisateur ou le groupe, activez la case à cocher en regard de chaque rôle à attribuer à l’utilisateur ou au groupe, puis cliquez sur **OK**.

        **Remarques**  Éditeur et approbateur incluent les autorisations de relecteur.

         

### Autres éléments à prendre en considération

-   Par défaut, vous devez être l’approbateur qui a créé ou contrôlé l’objet de stratégie de groupe ou un administrateur AGPM (contrôle total) pour effectuer cette procédure. Plus précisément, vous devez disposer de l’autorisation **contenu de liste** pour le domaine et modifier les autorisations de **sécurité** pour l’objet de stratégie de groupe.

-   Pour déléguer l’accès en lecture aux administrateurs de stratégie de groupe qui utilisent AGPM, vous devez leur attribuer le contenu de la **liste** et les autorisations de **paramètres de lecture** . Cela leur permet d’afficher des objets de stratégie de groupe dans l’onglet **contenu** d’AGPM. D’autres autorisations doivent être déléguées explicitement.

-   Les éditeurs doivent disposer d’une autorisation de **lecture** pour la copie déployée d’un objet de stratégie de groupe pour tirer pleinement parti de l’installation de logiciels de stratégie de groupe.

### Références supplémentaires

-   [Création, contrôle ou importation d'un objet de stratégie de groupe](creating-controlling-or-importing-a-gpo-editor-agpm30ops.md)

 

 





