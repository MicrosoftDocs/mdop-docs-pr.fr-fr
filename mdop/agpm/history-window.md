---
title: Fenêtre Historique
description: Fenêtre Historique
author: dansimp
ms.assetid: f11f9ad9-bffe-4c56-8c46-fe9c0a8e55c1
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: manage
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 02b4336409f33d6c1f2868bceb22cb95120f2198
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10808446"
---
# Fenêtre Historique


L’historique d’un objet de stratégie de groupe peut être affiché en double-cliquant sur un objet GPO ou en cliquant avec le bouton droit sur un objet de stratégie de groupe, puis en cliquant sur **historique**. Il est également affiché dans la **console de gestion des stratégies de groupe** (GPMC) en tant qu’onglet pour chaque GPO.

L’historique fournit la liste de toutes les versions de l’objet de stratégie de groupe sélectionné enregistrées dans l’archive. Dans la fenêtre **historique** , vous pouvez obtenir un rapport sur les paramètres d’un objet de stratégie de groupe, comparer plusieurs versions d’un objet de stratégie de groupe ou restaurer une version précédente d’un objet de stratégie de groupe.

## Filtrage d’événements dans la fenêtre historique


Les onglets de la fenêtre **historique** permettent de filtrer les événements affichés.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Eux</th>
<th align="left">Filtre</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><strong>Afficher tout</strong></p></td>
<td align="left"><p>Affichez toutes les versions de l’objet de stratégie de groupe.</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Archivé</strong></p></td>
<td align="left"><p>Afficher uniquement les versions intégrées de l’objet de stratégie de groupe. La version déployée ne figure pas dans cette liste.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Étiquettes uniquement</strong></p></td>
<td align="left"><p>Afficher uniquement les objets de stratégie de groupe associés à des étiquettes.</p></td>
</tr>
</tbody>
</table>

 

## Informations sur l’événement


Des informations sont fournies pour chaque événement dans l’historique de l’objet de stratégie de groupe sélectionné.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Caractéristique de l’objet GPO</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><strong>Ordinateur</strong></p></td>
<td align="left"><p>Version générée automatiquement de la partie configuration de l’ordinateur de l’objet de stratégie de groupe.</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Utilisateur</strong></p></td>
<td align="left"><p>Version générée automatiquement de la section Configuration utilisateur de l’objet de stratégie de groupe.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Heure</strong></p></td>
<td align="left"><p>Horodatage de la version de l’objet de stratégie de groupe lorsque l’action dans le champ État a été effectuée.</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>État</strong></p></td>
<td align="left"><p>État de la version sélectionnée de l’objet de stratégie de groupe:</p>
<p><img src="images/36f6b687-f5cc-40d1-805f-b191d1fb1ace.gif" alt="Deployed GPO icon" /> <strong>Déploiement </strong> : cette version de l’objet de stratégie de groupe est actuellement active dans l’environnement de production.</p>
<p><img src="images/57b610a5-1c71-4d26-9173-d04abd495fcc.gif" alt="Checked in GPO icon" /> <strong>Archivé </strong> : cette version de l’objet de stratégie de groupe est disponible pour les éditeurs autorisés à valider et à déployer.</p>
<p><img src="images/8e7a7c4e-809a-435a-8b29-30d797936210.gif" alt="Checked out GPO icon" /> <strong>Extrait </strong> : cette version de l’objet de stratégie de groupe est actuellement extraite par un éditeur et n’est pas disponible pour les autres éditeurs. (L’état extrait n’est pas enregistré dans le <strong> Historique </strong> sauf pour indiquer si un objet de stratégie de groupe est actuellement extrait.)</p>
<p><img src="images/327623bd-0842-4372-be1f-bdc4b8c3481c.gif" alt="Created GPO icon" /> <strong>Créé </strong> : identifie la date et l’heure de la création initiale de l’objet de stratégie de groupe.</p>
<p><img src="images/8356fcdc-1279-425b-ab14-a23bcfe391da.gif" alt="Labeled GPO icon" /> <strong>Étiquette </strong> : identifie une version libellée de l’objet de stratégie de groupe.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>État de l’objet GPO</strong></p></td>
<td align="left"><p>La configuration de l’ordinateur et la configuration de l’utilisateur peuvent être gérées indépendamment les uns des autres. Cet état indique les parties de l’objet GPO qui sont activées.</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Propriétaire</strong></p></td>
<td align="left"><p>Personne ayant archivé ou déployé l’objet de stratégie de groupe.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Comment</strong></p></td>
<td align="left"><p>Commentaire entré par le propriétaire d’un objet de stratégie de groupe au moment de la modification de cette version. Utile pour identifier les spécificités de la version dans le cas où il est nécessaire de revenir à une version précédente.</p></td>
</tr>
</tbody>
</table>

 

## Rapports


Selon que vous avez sélectionné une version d’un objet de stratégie de groupe ou plusieurs versions d’objets de stratégie de groupe, les boutons **paramètres** et **différences** affichent des rapports sur les paramètres de l’objet GPO. Lorsque vous cliquez avec le bouton droit sur les versions de l’objet de stratégie de groupe, vous pouvez également afficher des rapports XML.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Bouton</th>
<th align="left">Effet</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><strong>Paramètres</strong></p></td>
<td align="left"><p>Générer un rapport HTML affichant les paramètres dans la version sélectionnée de l’objet de stratégie de groupe.</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Diffère</strong></p></td>
<td align="left"><p>Générer un rapport HTML comparant les paramètres de plusieurs versions sélectionnées de l’objet de stratégie de groupe.</p></td>
</tr>
</tbody>
</table>

 

### Clé pour différencier les rapports

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Symbole</th>
<th align="left">Signification</th>
<th align="left">Couleur</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>None</p></td>
<td align="left"><p>L’élément existe avec des paramètres identiques dans les deux objets de stratégie de groupe</p></td>
<td align="left"><p>Varie selon le niveau</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>[#]</strong></p></td>
<td align="left"><p>L’élément existe dans les deux objets de stratégie de groupe, mais avec les paramètres modifiés</p></td>
<td align="left"><p>Bleu</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>[-]</strong></p></td>
<td align="left"><p>L’élément existe uniquement dans le premier objet GPO</p></td>
<td align="left"><p>Rouge</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>[+]</strong></p></td>
<td align="left"><p>L’élément existe uniquement dans le second objet de stratégie de groupe</p></td>
<td align="left"><p>Vert</p></td>
</tr>
</tbody>
</table>

 

-   Pour les éléments ayant modifié des paramètres, les paramètres modifiés sont identifiés lorsque l’élément est étendu. La valeur de l’attribut dans chaque objet GPO est affichée dans l’ordre dans lequel les objets de stratégie de groupe sont affichés dans le rapport.

-   Certaines modifications apportées aux paramètres peuvent entraîner le signalement d’un élément sous la forme de deux éléments différents (un seul présent dans le premier objet de stratégie de groupe, le premier uniquement dans le second), plutôt qu’un élément modifié.

### Références supplémentaires

-   [Onglet Contenu](contents-tab.md)

 

 





