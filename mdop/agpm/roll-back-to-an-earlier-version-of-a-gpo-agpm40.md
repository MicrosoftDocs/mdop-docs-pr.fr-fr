---
title: Revenir à une version antérieure d'objet de stratégie de groupe
description: Revenir à une version antérieure d'objet de stratégie de groupe
author: dansimp
ms.assetid: 06ce9251-95e0-46d0-99c2-b9a0690e5891
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: manage
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 1146a8ecaf25796b9ac105ba46ea7f27b06fc8aa
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10808241"
---
# <span data-ttu-id="06765-103">Revenir à une version antérieure d'objet de stratégie de groupe</span><span class="sxs-lookup"><span data-stu-id="06765-103">Roll Back to an Earlier Version of a GPO</span></span>


<span data-ttu-id="06765-104">Un approbateur peut annuler les modifications apportées à un objet de stratégie de groupe en redéployant une version antérieure de l’objet de stratégie de groupe à partir de son historique.</span><span class="sxs-lookup"><span data-stu-id="06765-104">An Approver can roll back changes to a Group Policy Object (GPO) by redeploying an earlier version of the GPO from its history.</span></span> <span data-ttu-id="06765-105">Le déploiement d’une version antérieure d’un objet de stratégie de groupe remplace la version de l’objet de stratégie de groupe actuellement en production.</span><span class="sxs-lookup"><span data-stu-id="06765-105">Deploying an earlier version of a GPO overwrites the version of the GPO currently in production.</span></span>

<span data-ttu-id="06765-106">Un compte d’utilisateur disposant du rôle d’approbateur ou d’administrateur AGPM (contrôle total) ou des autorisations nécessaires dans Advanced Group Policy Management (AGPM) est requis pour effectuer cette procédure.</span><span class="sxs-lookup"><span data-stu-id="06765-106">A user account with the Approver or AGPM Administrator (Full Control) role or necessary permissions in Advanced Group Policy Management (AGPM) is required to complete this procedure.</span></span> <span data-ttu-id="06765-107">Passez en revue les détails dans «autres considérations» dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="06765-107">Review the details in "Additional considerations" in this topic.</span></span>

**<span data-ttu-id="06765-108">Pour déployer une version antérieure d’un objet de stratégie de groupe dans l’environnement de production du domaine</span><span class="sxs-lookup"><span data-stu-id="06765-108">To deploy an earlier version of a GPO to the production environment of the domain</span></span>**

1.  <span data-ttu-id="06765-109">Dans l’arborescence de la **console de gestion des stratégies de groupe** , cliquez sur modifier le **contrôle** dans la forêt et le domaine dans lesquels vous souhaitez gérer les objets de stratégie de groupe.</span><span class="sxs-lookup"><span data-stu-id="06765-109">In the **Group Policy Management Console** tree, click **Change Control** in the forest and domain in which you want to manage GPOs.</span></span>

2.  <span data-ttu-id="06765-110">Dans l’onglet **contenu** , cliquez sur l’onglet **contrôlé** pour afficher les objets de stratégie de groupe contrôlés.</span><span class="sxs-lookup"><span data-stu-id="06765-110">On the **Contents** tab, click the **Controlled** tab to display the controlled GPOs.</span></span>

3.  <span data-ttu-id="06765-111">Double-cliquez sur l’objet de stratégie de groupe à déployer pour afficher son **historique**.</span><span class="sxs-lookup"><span data-stu-id="06765-111">Double-click the GPO to be deployed to display its **History**.</span></span>

4.  <span data-ttu-id="06765-112">Cliquez avec le bouton droit sur la version que vous voulez déployer, cliquez sur **déployer**, puis sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="06765-112">Right-click the version to be deployed, click **Deploy**, and then click **Yes**.</span></span>

5.  <span data-ttu-id="06765-113">Lorsque la fenêtre de **progression** indique que l’avancement global est terminé, cliquez sur **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="06765-113">When the **Progress** window indicates that overall progress is complete, click **Close**.</span></span> <span data-ttu-id="06765-114">Dans la fenêtre **historique** , cliquez sur **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="06765-114">In the **History** window, click **Close**.</span></span>

<span data-ttu-id="06765-115">**Remarques**  Pour vérifier que la version qui a été redéployée correspond à la version prévue, examinez un rapport de différences pour les deux versions.</span><span class="sxs-lookup"><span data-stu-id="06765-115">**Note** To verify that the version that has been redeployed matches the version intended, examine a difference report for the two versions.</span></span> <span data-ttu-id="06765-116">Dans la fenêtre **historique** de l’objet de stratégie de groupe, sélectionnez les deux versions, puis cliquez avec le bouton droit et sélectionnez **différence** et l’état **HTML** ou **rapport XML**.</span><span class="sxs-lookup"><span data-stu-id="06765-116">In the **History** window for the GPO, highlight the two versions, and then right-click and select **Difference** and either **HTML Report** or **XML Report**.</span></span>

 

### <span data-ttu-id="06765-117">Autres éléments à prendre en considération</span><span class="sxs-lookup"><span data-stu-id="06765-117">Additional considerations</span></span>

-   <span data-ttu-id="06765-118">Par défaut, vous devez être approbateur ou administrateur AGPM (contrôle total) pour effectuer cette procédure.</span><span class="sxs-lookup"><span data-stu-id="06765-118">By default, you must be an Approver or an AGPM Administrator (Full Control) to perform this procedure.</span></span> <span data-ttu-id="06765-119">Plus précisément, vous devez disposer du **contenu de liste** et déployer des autorisations d' **objet** de stratégie de groupe pour l’objet GPO.</span><span class="sxs-lookup"><span data-stu-id="06765-119">Specifically, you must have **List Contents** and **Deploy GPO** permissions for the GPO.</span></span>

### <span data-ttu-id="06765-120">Références supplémentaires</span><span class="sxs-lookup"><span data-stu-id="06765-120">Additional references</span></span>

-   [<span data-ttu-id="06765-121">Exécution de tâches d'approbateur</span><span class="sxs-lookup"><span data-stu-id="06765-121">Performing Approver Tasks</span></span>](performing-approver-tasks-agpm40.md)

 

 




