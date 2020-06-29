---
title: Procédure pour modifier le niveau de journalisation du serveur et les paramètres de base de données
description: Procédure pour modifier le niveau de journalisation du serveur et les paramètres de base de données
author: dansimp
ms.assetid: e3ebaee5-6c4c-4aa8-9766-c5aeb00f477a
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop, appcompat, virtualization
ms.mktglfcycl: deploy
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: bb35ac09c5e23f4847662171b68284f868e66dee
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10807345"
---
# <span data-ttu-id="dca45-103">Procédure pour modifier le niveau de journalisation du serveur et les paramètres de base de données</span><span class="sxs-lookup"><span data-stu-id="dca45-103">How to Change the Server Logging Level and the Database Parameters</span></span>


<span data-ttu-id="dca45-104">Vous pouvez utiliser les procédures suivantes pour modifier le niveau de journalisation et les paramètres de journalisation de la base de données à partir de la console de gestion du serveur d’applications.</span><span class="sxs-lookup"><span data-stu-id="dca45-104">You can use the following procedures to change the logging level and the database log parameters from the Application Virtualization Server Management Console.</span></span>

<span data-ttu-id="dca45-105">Les niveaux de journalisation suivants sont disponibles:</span><span class="sxs-lookup"><span data-stu-id="dca45-105">The following logging levels are available:</span></span>

-   <span data-ttu-id="dca45-106">Transaction uniquement</span><span class="sxs-lookup"><span data-stu-id="dca45-106">Transaction Only</span></span>

-   <span data-ttu-id="dca45-107">Erreurs irrécupérables</span><span class="sxs-lookup"><span data-stu-id="dca45-107">Fatal Errors</span></span>

-   <span data-ttu-id="dca45-108">Erreurs</span><span class="sxs-lookup"><span data-stu-id="dca45-108">Errors</span></span>

-   <span data-ttu-id="dca45-109">Avertissements/Erreurs</span><span class="sxs-lookup"><span data-stu-id="dca45-109">Warnings/Errors</span></span>

-   <span data-ttu-id="dca45-110">Infos/avertissements/Erreurs</span><span class="sxs-lookup"><span data-stu-id="dca45-110">Info/Warnings/Errors</span></span>

-   <span data-ttu-id="dca45-111">Détaillée</span><span class="sxs-lookup"><span data-stu-id="dca45-111">Verbose</span></span>

<span data-ttu-id="dca45-112">**Remarques**  En raison de la taille du fichier journal obtenu lors de l’utilisation du mode **détaillé** , il est recommandé de ne pas exécuter de serveurs de production avec ce niveau de jeu de journaux.</span><span class="sxs-lookup"><span data-stu-id="dca45-112">**Note** Because of the size of the log file produced when you use **Verbose** mode, the recommendation is that you do not run production servers with this level of logging set.</span></span>

 

<span data-ttu-id="dca45-113">Les paramètres de journalisation de la base de données déterminent le type du pilote de la base de données, les informations d’accès et l’emplacement de la base de données.</span><span class="sxs-lookup"><span data-stu-id="dca45-113">The database logging parameters determine the database driver type, access credentials, and location of the logging database.</span></span>

**<span data-ttu-id="dca45-114">Pour modifier le niveau de journalisation pour les serveurs de gestion</span><span class="sxs-lookup"><span data-stu-id="dca45-114">To change the logging level for Management Servers</span></span>**

1.  <span data-ttu-id="dca45-115">Cliquez sur le nœud **groupes de serveurs** pour afficher les groupes de serveurs.</span><span class="sxs-lookup"><span data-stu-id="dca45-115">Click the **Server Groups** node to display the server groups.</span></span>

2.  <span data-ttu-id="dca45-116">Cliquez avec le bouton droit sur le groupe de serveurs, puis sélectionnez **Propriétés**.</span><span class="sxs-lookup"><span data-stu-id="dca45-116">Right-click the server group, and select **Properties**.</span></span>

3.  <span data-ttu-id="dca45-117">Dans la boîte de dialogue **Propriétés** , sélectionnez l’onglet **journalisation** .</span><span class="sxs-lookup"><span data-stu-id="dca45-117">In the **Properties** dialog box, select the **Logging** tab.</span></span>

4.  <span data-ttu-id="dca45-118">Dans la boîte de dialogue **Propriétés du groupe de serveurs** , sélectionnez le serveur, puis cliquez sur **modifier**.</span><span class="sxs-lookup"><span data-stu-id="dca45-118">In the **Server Group Properties** dialog box, select the server and then click **Edit**.</span></span>

5.  <span data-ttu-id="dca45-119">Dans la boîte de dialogue **Ajouter/modifier le module journal** , sélectionnez le niveau de journalisation dans la liste déroulante **type d’événement** .</span><span class="sxs-lookup"><span data-stu-id="dca45-119">In the **Add/Edit Log Module** dialog box, select the logging level from the **Event Type** drop-down list.</span></span>

6.  <span data-ttu-id="dca45-120">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="dca45-120">Click **OK**.</span></span>

7.  <span data-ttu-id="dca45-121">Dans la boîte de dialogue **Propriétés du groupe de serveurs** , cliquez sur **OK** ou sur **appliquer**.</span><span class="sxs-lookup"><span data-stu-id="dca45-121">In the **Server Group Properties** dialog box, click **OK** or **Apply**.</span></span>

**<span data-ttu-id="dca45-122">Pour modifier le niveau de journalisation pour les serveurs de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="dca45-122">To change the logging level for Streaming Servers</span></span>**

1.  <span data-ttu-id="dca45-123">Modifiez la valeur de clé de Registre suivante pour modifier le niveau de journalisation:</span><span class="sxs-lookup"><span data-stu-id="dca45-123">Edit the following registry key value to change the logging level:</span></span>

    -   <span data-ttu-id="dca45-124">HKEY \ _LOCAL \ _MACHINE \\SOFTWARE\\Microsoft\\SoftGrid\\4.5\\DistributionServer\\LogLevel</span><span class="sxs-lookup"><span data-stu-id="dca45-124">HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\SoftGrid\\4.5\\DistributionServer\\LogLevel</span></span>

2.  <span data-ttu-id="dca45-125">Sélectionnez l’une des valeurs suivantes pour définir le niveau de journalisation.</span><span class="sxs-lookup"><span data-stu-id="dca45-125">Select one of the following values to set the logging level.</span></span>

    <table>
    <colgroup>
    <col width="50%" />
    <col width="50%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th align="left"><span data-ttu-id="dca45-126">Valeur</span><span class="sxs-lookup"><span data-stu-id="dca45-126">Value</span></span></th>
    <th align="left"><span data-ttu-id="dca45-127">Niveau de journalisation</span><span class="sxs-lookup"><span data-stu-id="dca45-127">Logging Level</span></span></th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td align="left"><p><span data-ttu-id="dca45-128">0,4</span><span class="sxs-lookup"><span data-stu-id="dca45-128">0</span></span></p></td>
    <td align="left"><p><span data-ttu-id="dca45-129">Transactions uniquement</span><span class="sxs-lookup"><span data-stu-id="dca45-129">Transactions Only</span></span></p></td>
    </tr>
    <tr class="even">
    <td align="left"><p><span data-ttu-id="dca45-130">1</span><span class="sxs-lookup"><span data-stu-id="dca45-130">1</span></span></p></td>
    <td align="left"><p><span data-ttu-id="dca45-131">Erreurs irrécupérables</span><span class="sxs-lookup"><span data-stu-id="dca45-131">Fatal Errors</span></span></p></td>
    </tr>
    <tr class="odd">
    <td align="left"><p><span data-ttu-id="dca45-132">deuxième</span><span class="sxs-lookup"><span data-stu-id="dca45-132">2</span></span></p></td>
    <td align="left"><p><span data-ttu-id="dca45-133">Erreurs</span><span class="sxs-lookup"><span data-stu-id="dca45-133">Errors</span></span></p></td>
    </tr>
    <tr class="even">
    <td align="left"><p><span data-ttu-id="dca45-134">3D</span><span class="sxs-lookup"><span data-stu-id="dca45-134">3</span></span></p></td>
    <td align="left"><p><span data-ttu-id="dca45-135">Avertissements/Erreurs</span><span class="sxs-lookup"><span data-stu-id="dca45-135">Warnings/Errors</span></span></p></td>
    </tr>
    <tr class="odd">
    <td align="left"><p><span data-ttu-id="dca45-136">n°4</span><span class="sxs-lookup"><span data-stu-id="dca45-136">4</span></span></p></td>
    <td align="left"><p><span data-ttu-id="dca45-137">Informations/avertissements/Erreurs</span><span class="sxs-lookup"><span data-stu-id="dca45-137">Information/ Warnings/Errors</span></span></p></td>
    </tr>
    <tr class="even">
    <td align="left"><p><span data-ttu-id="dca45-138">n°5</span><span class="sxs-lookup"><span data-stu-id="dca45-138">5</span></span></p></td>
    <td align="left"><p><span data-ttu-id="dca45-139">Détaillée</span><span class="sxs-lookup"><span data-stu-id="dca45-139">Verbose</span></span></p></td>
    </tr>
    </tbody>
    </table>

     

**<span data-ttu-id="dca45-140">Pour modifier les paramètres du journal de base de données</span><span class="sxs-lookup"><span data-stu-id="dca45-140">To change database log parameters</span></span>**

1.  <span data-ttu-id="dca45-141">Cliquez sur le nœud **groupes de serveurs** pour afficher les groupes de serveurs.</span><span class="sxs-lookup"><span data-stu-id="dca45-141">Click the **Server Groups** node to display the server groups.</span></span>

2.  <span data-ttu-id="dca45-142">Cliquez avec le bouton droit sur le groupe de serveurs, puis sélectionnez **Propriétés**.</span><span class="sxs-lookup"><span data-stu-id="dca45-142">Right-click the server group, and select **Properties**.</span></span>

3.  <span data-ttu-id="dca45-143">Dans la boîte de dialogue **Propriétés** , sélectionnez l’onglet **journalisation** .</span><span class="sxs-lookup"><span data-stu-id="dca45-143">In the **Properties** dialog box, select the **Logging** tab.</span></span>

4.  <span data-ttu-id="dca45-144">Dans la boîte de dialogue **Propriétés du groupe de serveurs** , sélectionnez le serveur, puis cliquez sur **modifier**.</span><span class="sxs-lookup"><span data-stu-id="dca45-144">In the **Server Group Properties** dialog box, select the server and then click **Edit**.</span></span>

5.  <span data-ttu-id="dca45-145">Dans la boîte de dialogue **Ajouter/modifier le module journal** , sélectionnez un pilote de base de données dans la liste déroulante **pilote de base de données** .</span><span class="sxs-lookup"><span data-stu-id="dca45-145">In the **Add/Edit Log Module** dialog box, select a database driver from the **Database Driver** drop-down list.</span></span>

6.  <span data-ttu-id="dca45-146">Entrez un **nom d’hôte DNS**.</span><span class="sxs-lookup"><span data-stu-id="dca45-146">Enter a **DNS Host Name**.</span></span>

7.  <span data-ttu-id="dca45-147">Cliquez sur la case à cocher **Déterminez dynamiquement le port** ou entrez un numéro de port dans le champ **port** .</span><span class="sxs-lookup"><span data-stu-id="dca45-147">Click the **Dynamically Determine Port** check box, or enter a port number in the **Port** field.</span></span>

8.  <span data-ttu-id="dca45-148">Entrez un **nom de service** dans le champ correspondant.</span><span class="sxs-lookup"><span data-stu-id="dca45-148">Enter a **Service Name** in the corresponding field.</span></span>

9.  <span data-ttu-id="dca45-149">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="dca45-149">Click **OK**.</span></span>

10. <span data-ttu-id="dca45-150">Dans la boîte de dialogue **Propriétés du groupe de serveurs** , cliquez sur **OK** ou sur **appliquer**.</span><span class="sxs-lookup"><span data-stu-id="dca45-150">On the **Server Group Properties** dialog box, click **OK** or **Apply**.</span></span>

## <span data-ttu-id="dca45-151">Rubriques connexes</span><span class="sxs-lookup"><span data-stu-id="dca45-151">Related topics</span></span>


[<span data-ttu-id="dca45-152">Procédure pour personnaliser un système Application Virtualization dans Server Management Console</span><span class="sxs-lookup"><span data-stu-id="dca45-152">How to Customize an Application Virtualization System in the Server Management Console</span></span>](how-to-customize-an-application-virtualization-system-in-the-server-management-console.md)

 

 





