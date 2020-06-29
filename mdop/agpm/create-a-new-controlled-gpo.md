---
title: Créer un objet de stratégie de groupe contrôlé
description: Créer un objet de stratégie de groupe contrôlé
author: dansimp
ms.assetid: b43ce0f4-4519-4278-83c4-c7d5163ddd11
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: manage
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 0a64e22036bfe99e1d5012d732e3f2e081acdcca
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10808569"
---
# <span data-ttu-id="bf67e-103">Créer un objet de stratégie de groupe contrôlé</span><span class="sxs-lookup"><span data-stu-id="bf67e-103">Create a New Controlled GPO</span></span>


<span data-ttu-id="bf67e-104">Les nouveaux objets de stratégie de groupe créés par le biais du nœud de **contrôle de modification** seront automatiquement contrôlés, ce qui vous permettra de les gérer avec AGPM (Advanced Group Policy Management).</span><span class="sxs-lookup"><span data-stu-id="bf67e-104">New Group Policy objects (GPOs) created through the **Change Control** node will automatically be controlled, enabling you to manage them with Advanced Group Policy Management (AGPM).</span></span>

<span data-ttu-id="bf67e-105">Un compte d’utilisateur ayant le rôle d’approbateur ou d’administrateur AGPM (contrôle total) ou les autorisations nécessaires dans la gestion avancée de la stratégie de groupe est requis pour effectuer cette procédure.</span><span class="sxs-lookup"><span data-stu-id="bf67e-105">A user account with the Approver or AGPM Administrator (Full Control) role or necessary permissions in Advanced Group Policy Management is required to complete this procedure.</span></span> <span data-ttu-id="bf67e-106">Passez en revue les détails dans «autres considérations» dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="bf67e-106">Review the details in "Additional considerations" in this topic.</span></span>

**<span data-ttu-id="bf67e-107">Pour créer un nouvel objet de stratégie de groupe avec le contrôle de modification géré via AGPM</span><span class="sxs-lookup"><span data-stu-id="bf67e-107">To create a new GPO with change control managed through AGPM</span></span>**

1.  <span data-ttu-id="bf67e-108">Dans l’arborescence de la **console de gestion des stratégies de groupe** , cliquez sur modifier le **contrôle** dans la forêt et le domaine dans lesquels vous souhaitez gérer les objets de stratégie de groupe.</span><span class="sxs-lookup"><span data-stu-id="bf67e-108">In the **Group Policy Management Console** tree, click **Change Control** in the forest and domain in which you want to manage GPOs.</span></span>

2.  <span data-ttu-id="bf67e-109">Cliquez avec le bouton droit sur le nœud de **contrôle de modification** , puis cliquez sur **nouvel objet de stratégie de**contrôle.</span><span class="sxs-lookup"><span data-stu-id="bf67e-109">Right-click the **Change Control** node, and then click **New Controlled GPO**.</span></span>

3.  <span data-ttu-id="bf67e-110">Dans la boîte de dialogue **nouvel objet GPO contrôlé** :</span><span class="sxs-lookup"><span data-stu-id="bf67e-110">In the **New Controlled GPO** dialog box:</span></span>

    1.  <span data-ttu-id="bf67e-111">Tapez un nom pour le nouvel objet de stratégie de groupe.</span><span class="sxs-lookup"><span data-stu-id="bf67e-111">Type a name for the new GPO.</span></span>

    2.  <span data-ttu-id="bf67e-112">Facultatif: tapez un commentaire pour le nouvel objet de stratégie de groupe à afficher dans l' **historique** de l’objet de stratégie de groupe.</span><span class="sxs-lookup"><span data-stu-id="bf67e-112">Optional: Type a comment for the new GPO to be displayed in the **History** for the GPO.</span></span>

    3.  <span data-ttu-id="bf67e-113">Pour déployer immédiatement le nouvel objet GPO dans l’environnement de production, cliquez sur **créer en direct**.</span><span class="sxs-lookup"><span data-stu-id="bf67e-113">To immediately deploy the new GPO to the production environment, click **Create live**.</span></span> <span data-ttu-id="bf67e-114">Pour créer le nouvel objet GPO hors connexion sans le déployer immédiatement, cliquez sur créer un fichier **hors connexion**.</span><span class="sxs-lookup"><span data-stu-id="bf67e-114">To create the new GPO offline without immediately deploying it, click **Create offline**.</span></span>

    4.  <span data-ttu-id="bf67e-115">Sélectionnez le modèle d’objet de stratégie de groupe à utiliser comme point de départ pour le nouvel objet de stratégie de groupe.</span><span class="sxs-lookup"><span data-stu-id="bf67e-115">Select the GPO template to use as a starting point for the new GPO.</span></span>

    5.  <span data-ttu-id="bf67e-116">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="bf67e-116">Click **OK**.</span></span>

4.  <span data-ttu-id="bf67e-117">Lorsque la fenêtre de **progression** indique que l’avancement global est terminé, cliquez sur **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="bf67e-117">When the **Progress** window indicates that overall progress is complete, click **Close**.</span></span> <span data-ttu-id="bf67e-118">Le nouvel objet GPO est affiché dans la liste des objets de stratégie de groupe sous l’onglet **contrôlé** .</span><span class="sxs-lookup"><span data-stu-id="bf67e-118">The new GPO is displayed in the list of GPOs on the **Controlled** tab.</span></span>

### <span data-ttu-id="bf67e-119">Autres éléments à prendre en considération</span><span class="sxs-lookup"><span data-stu-id="bf67e-119">Additional considerations</span></span>

-   <span data-ttu-id="bf67e-120">Par défaut, vous devez être approbateur ou administrateur AGPM (contrôle total) pour effectuer cette procédure.</span><span class="sxs-lookup"><span data-stu-id="bf67e-120">By default, you must be an Approver or an AGPM Administrator (Full Control) to perform this procedure.</span></span> <span data-ttu-id="bf67e-121">Plus précisément, vous devez disposer du **contenu de liste** et créer des autorisations d’objet de **stratégie de groupe** pour le domaine.</span><span class="sxs-lookup"><span data-stu-id="bf67e-121">Specifically, you must have **List Contents** and **Create GPO** permissions for the domain.</span></span>

### <span data-ttu-id="bf67e-122">Références supplémentaires</span><span class="sxs-lookup"><span data-stu-id="bf67e-122">Additional references</span></span>

-   [<span data-ttu-id="bf67e-123">Création, contrôle ou importation d'un objet de stratégie de groupe</span><span class="sxs-lookup"><span data-stu-id="bf67e-123">Creating, Controlling, or Importing a GPO</span></span>](creating-controlling-or-importing-a-gpo-approver.md)

 

 




