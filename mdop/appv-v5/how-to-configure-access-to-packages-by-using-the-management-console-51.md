---
title: Comment configurer l’accès aux packages à l’aide de la console de gestion
description: Comment configurer l’accès aux packages à l’aide de la console de gestion
author: dansimp
ms.assetid: 4fd39bc2-d814-46de-a108-1c21fa404e8a
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop, appcompat, virtualization
ms.mktglfcycl: deploy
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 3c6c8f930fb1fbd82432f6d43dae8b9bed7a563c
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10805712"
---
# <span data-ttu-id="5ead6-103">Comment configurer l’accès aux packages à l’aide de la console de gestion</span><span class="sxs-lookup"><span data-stu-id="5ead6-103">How to Configure Access to Packages by Using the Management Console</span></span>


<span data-ttu-id="5ead6-104">Avant de déployer un package virtualisé App-V 5,1, vous devez configurer les groupes de sécurité AD DS (Active Directory Domain Services) qui seront autorisés à accéder aux applications et à les exécuter.</span><span class="sxs-lookup"><span data-stu-id="5ead6-104">Before you deploy an App-V 5.1 virtualized package, you must configure the Active Directory Domain Services (AD DS) security groups that will be allowed to access and run the applications.</span></span> <span data-ttu-id="5ead6-105">Les groupes de sécurité peuvent contenir des ordinateurs ou des utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="5ead6-105">The security groups may contain computers or users.</span></span> <span data-ttu-id="5ead6-106">Le faire d’un package à un groupe d’ordinateurs publie le package globalement sur tous les ordinateurs du groupe.</span><span class="sxs-lookup"><span data-stu-id="5ead6-106">Entitling a package to a computer group publishes the package globally to all computers in the group.</span></span>

<span data-ttu-id="5ead6-107">Utilisez la procédure suivante pour configurer l’accès aux packages virtualisés.</span><span class="sxs-lookup"><span data-stu-id="5ead6-107">Use the following procedure to configure access to virtualized packages.</span></span>

**<span data-ttu-id="5ead6-108">Pour accorder l’accès à un package App-V 5,1</span><span class="sxs-lookup"><span data-stu-id="5ead6-108">To grant access to an App-V 5.1 package</span></span>**

1.  <span data-ttu-id="5ead6-109">Recherchez le package que vous souhaitez configurer:</span><span class="sxs-lookup"><span data-stu-id="5ead6-109">Find the package you want to configure:</span></span>

    1.  <span data-ttu-id="5ead6-110">Ouvrez la console de gestion App-V 5,1.</span><span class="sxs-lookup"><span data-stu-id="5ead6-110">Open the App-V 5.1 Management console.</span></span>

    2.  <span data-ttu-id="5ead6-111">Pour afficher la page d’accès à la **publicité** , cliquez avec le bouton droit sur le package à configurer, puis sélectionnez **modifier l’accès Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-111">To display the **AD ACCESS** page, right-click the package to be configured, and select **Edit active directory access**.</span></span> <span data-ttu-id="5ead6-112">Vous pouvez également sélectionner le package et cliquer sur **modifier** dans le volet accès à la **publicité** .</span><span class="sxs-lookup"><span data-stu-id="5ead6-112">Alternatively, select the package and click **EDIT** in the **AD ACCESS** pane.</span></span>

2.  <span data-ttu-id="5ead6-113">Mettre en service un groupe de sécurité pour le package:</span><span class="sxs-lookup"><span data-stu-id="5ead6-113">Provision a security group for the package:</span></span>

    1.  <span data-ttu-id="5ead6-114">Accédez à la page **Rechercher des noms Active Directory et des autorisations d’accès** .</span><span class="sxs-lookup"><span data-stu-id="5ead6-114">Go to the **FIND VALID ACTIVE DIRECTORY NAMES AND GRANT ACCESS** page.</span></span>

    2.  <span data-ttu-id="5ead6-115">À l’aide de la mise en forme **mondomaine**  \\  **nom_groupe**, tapez le nom ou une partie du nom d’un objet de groupe Active Directory, puis cliquez sur **vérifier**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-115">Using the format **mydomain** \\ **groupname**, type the name or part of the name of an Active Directory group object, and click **Check**.</span></span>

        <span data-ttu-id="5ead6-116">**Remarques**  Vérifiez que vous fournissez un nom de domaine associé au groupe que vous recherchez.</span><span class="sxs-lookup"><span data-stu-id="5ead6-116">**Note** Ensure that you provide an associated domain name for the group that you are searching for.</span></span>

         

3.  <span data-ttu-id="5ead6-117">Pour accorder l’accès au package, sélectionnez le groupe de votre choix, puis cliquez sur **accorder l’accès**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-117">To grant access to the package, select the desired group and click **Grant Access**.</span></span> <span data-ttu-id="5ead6-118">Le groupe que vous venez d’ajouter apparaît dans le volet **entités publicitaires avec** le volet accès.</span><span class="sxs-lookup"><span data-stu-id="5ead6-118">The newly added group is displayed in the **AD ENTITIES WITH ACCESS** pane.</span></span>

4.  

    <span data-ttu-id="5ead6-119">Pour accepter les paramètres de configuration par défaut et fermer la page d' **accès à la publicité** , cliquez sur **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-119">To accept the default configuration settings and close the **AD ACCESS** page, click **Close**.</span></span>

    <span data-ttu-id="5ead6-120">Pour personnaliser des configurations pour un groupe spécifique, cliquez sur la liste déroulante **configurations affectées** , puis sélectionnez **personnalisée**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-120">To customize configurations for a specific group, click the **ASSIGNED CONFIGURATIONS** drop-down and select **Custom**.</span></span> <span data-ttu-id="5ead6-121">Pour configurer les configurations personnalisées, cliquez sur **modifier**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-121">To configure the custom configurations, click **EDIT**.</span></span> <span data-ttu-id="5ead6-122">Après avoir accordé l’accès, cliquez sur **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-122">After you grant access, click **Close**.</span></span>

**<span data-ttu-id="5ead6-123">Pour supprimer l’accès à un package App-V 5,1</span><span class="sxs-lookup"><span data-stu-id="5ead6-123">To remove access to an App-V 5.1 package</span></span>**

1.  <span data-ttu-id="5ead6-124">Recherchez le package que vous souhaitez configurer:</span><span class="sxs-lookup"><span data-stu-id="5ead6-124">Find the package you want to configure:</span></span>

    1.  <span data-ttu-id="5ead6-125">Ouvrez la console de gestion App-V 5,1.</span><span class="sxs-lookup"><span data-stu-id="5ead6-125">Open the App-V 5.1 Management console.</span></span>

    2.  <span data-ttu-id="5ead6-126">Pour afficher la page d’accès à la **publicité** , cliquez avec le bouton droit sur le package à configurer, puis sélectionnez **modifier l’accès Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-126">To display the **AD ACCESS** page, right-click the package to be configured, and select **Edit active directory access**.</span></span> <span data-ttu-id="5ead6-127">Vous pouvez également sélectionner le package et cliquer sur **modifier** dans le volet accès à la **publicité** .</span><span class="sxs-lookup"><span data-stu-id="5ead6-127">Alternatively, select the package and click **EDIT** in the **AD ACCESS** pane.</span></span>

2.  <span data-ttu-id="5ead6-128">Sélectionnez le groupe que vous voulez supprimer, puis cliquez sur **supprimer**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-128">Select the group you want to remove, and click **DELETE**.</span></span>

3.  <span data-ttu-id="5ead6-129">Pour fermer la page d’accès à la **publicité** , cliquez sur **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="5ead6-129">To close the **AD ACCESS** page, click **Close**.</span></span>

    <span data-ttu-id="5ead6-130">Vous **avez une suggestion pour App-V**?</span><span class="sxs-lookup"><span data-stu-id="5ead6-130">**Got a suggestion for App-V**?</span></span> <span data-ttu-id="5ead6-131">Ajoutez ou Votez en fonction [de suggestions.](http://appv.uservoice.com/forums/280448-microsoft-application-virtualization)</span><span class="sxs-lookup"><span data-stu-id="5ead6-131">Add or vote on suggestions [here](http://appv.uservoice.com/forums/280448-microsoft-application-virtualization).</span></span> **<span data-ttu-id="5ead6-132">Vous avez un problème lié à l’application-V?</span><span class="sxs-lookup"><span data-stu-id="5ead6-132">Got an App-V issue?</span></span>** <span data-ttu-id="5ead6-133">Utilisez le [Forum TechNet App-V](https://social.technet.microsoft.com/Forums/home?forum=mdopappv).</span><span class="sxs-lookup"><span data-stu-id="5ead6-133">Use the [App-V TechNet Forum](https://social.technet.microsoft.com/Forums/home?forum=mdopappv).</span></span>

## <span data-ttu-id="5ead6-134">Rubriques connexes</span><span class="sxs-lookup"><span data-stu-id="5ead6-134">Related topics</span></span>


[<span data-ttu-id="5ead6-135">Opérations d'App-V5.1</span><span class="sxs-lookup"><span data-stu-id="5ead6-135">Operations for App-V 5.1</span></span>](operations-for-app-v-51.md)

 

 




