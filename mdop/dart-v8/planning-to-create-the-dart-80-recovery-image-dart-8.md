---
title: Planification pour créer l'image de récupération DaRT8.0
description: Planification pour créer l'image de récupération DaRT8.0
author: dansimp
ms.assetid: cfd0e1e2-c379-4460-b545-3f7be9f33583
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: support
ms.sitesec: library
ms.prod: w10
ms.date: 08/30/2016
ms.openlocfilehash: 1d1dc7dc5b3776638523a282d9216b80d4ce9ce1
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10810776"
---
# Planification pour créer l'image de récupération DaRT8.0


Utilisez les informations fournies dans cette section lorsque vous envisagez de créer l’image de récupération du jeu d’outils de diagnostics et de récupération Microsoft (DaRT) 8,0.

## Planification de la création de l’image de récupération 8,0 de DaRT


Lorsque vous créez l’image de récupération DaRT, vous devez choisir les outils à inclure dans l’image. Pour prendre la décision, tenez compte du fait que les utilisateurs finaux peuvent avoir accès à ces outils. Si les techniciens du support technique emportent le média d’image de récupération aux ordinateurs des utilisateurs finaux pour diagnostiquer les problèmes, vous pouvez installer tous les outils sur l’image de récupération. Si vous envisagez de diagnostiquer les ordinateurs des utilisateurs finaux à distance, vous souhaiterez peut-être désactiver certains outils, tels que l’effacement de disque et l’éditeur du Registre, puis activer d’autres outils, y compris la connexion à distance.

Lorsque vous créez l’image de récupération DaRT, vous devez également indiquer si vous souhaitez inclure d’autres pilotes ou fichiers. Déterminez les emplacements des pilotes ou fichiers supplémentaires que vous voulez inclure dans l’image de récupération DaRT.

Pour plus d’informations sur les outils DaRT, voir [vue d’ensemble des outils dans dart 8,0](overview-of-the-tools-in-dart-80-dart-8.md). Pour plus d’informations sur la création d’une image de récupération sécurisée, voir [considérations relatives à la sécurité de DaRT 8,0](security-considerations-for-dart-80--dart-8.md).

## Conditions préalables à l’image de récupération


Les éléments suivants sont requis ou recommandés pour la création de l’image de récupération DaRT:

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><strong>Prérequises</strong></p></td>
<td align="left"><p><strong>Détails</strong></p></td>
</tr>
<tr class="even">
<td align="left"><p>Fichiers sources de Windows 8</p></td>
<td align="left"><p>Requis pour créer l’image de récupération DaRT. Spécifiez le chemin d’accès d’un DVD Windows 8 ou d’un fichier source Windows 8.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Outils de débogage Windows pour votre plate-forme</p></td>
<td align="left"><p>Requis lors de l’exécution <strong> de l’analyseur </strong> d’incidents pour déterminer la cause de l’échec de l’ordinateur. Nous vous recommandons de spécifier le chemin d’accès des outils de débogage Windows au moment de la création de l’image de récupération DaRT. Vous pouvez télécharger les outils de débogage Windows suivants: <a href="https://go.microsoft.com/fwlink/?LinkId=99934" data-raw-source="[Download and Install Debugging Tools for Windows](https://go.microsoft.com/fwlink/?LinkId=99934)"> Télécharger et installer les outils de débogage pour Windows </a> .</p></td>
</tr>
<tr class="even">
<td align="left"><p>Facultatif: <strong> définitions de protection </strong></p></td>
<td align="left"><p>Les définitions les plus récentes pour <strong> Defender </strong> sont nécessaires lorsque vous exécutez <strong> Defender </strong> . Même si vous pouvez télécharger les définitions lors de l’exécution de l' <strong> </strong> outil de protection, nous vous conseillons de télécharger les dernières définitions lors de la création de l’image de récupération DART pour pouvoir continuer à exécuter l’outil avec les définitions les plus récentes, même si le problème n’est pas lié à la connectivité réseau.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Facultatif: fichiers de symboles Windows à utiliser avec l' <strong> analyseur d’incidents</strong></p></td>
<td align="left"><p>En général, les informations de débogage sont stockées dans un fichier de symboles différent du programme. Vous devez avoir accès aux informations de symbole lors du débogage d’une application qui a cessé de répondre (par exemple, si elle a cessé de fonctionner). Pour plus d’informations, reportez-vous à la rubrique <a href="diagnosing-system-failures-with-crash-analyzer--dart-8.md" data-raw-source="[Diagnosing System Failures with Crash Analyzer](diagnosing-system-failures-with-crash-analyzer--dart-8.md)"> diagnostic des pannes système avec l’analyseur d’incidents </a> .</p></td>
</tr>
</tbody>
</table>

 

## Rubriques connexes


[Planification du déploiement de DaRT8.0](planning-to-deploy-dart-80-dart-8.md)

 

 





