---
title: Référence de commande SFTMIME
description: Référence de commande SFTMIME
author: dansimp
ms.assetid: a4a69228-9dd3-4623-b773-899d03c0cf10
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop, appcompat, virtualization
ms.mktglfcycl: deploy
ms.sitesec: library
ms.prod: w10
ms.date: 06/16/2016
ms.openlocfilehash: 47aac9110febaf3f349461d74fef840326b1c6e4
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10806270"
---
# <span data-ttu-id="365c1-103">Référence de commande SFTMIME</span><span class="sxs-lookup"><span data-stu-id="365c1-103">SFTMIME Command Reference</span></span>


<span data-ttu-id="365c1-104">SFTMIME est une interface de ligne de commande utilisée par la virtualisation des applications (App-V) qui vous permet de gérer de nombreux détails relatifs à la configuration du client.</span><span class="sxs-lookup"><span data-stu-id="365c1-104">SFTMIME is a command-line interface used by Application Virtualization (App-V) that enables you to manage many client configuration details.</span></span> <span data-ttu-id="365c1-105">Cette section contient toutes les commandes et leurs paramètres, avec une brève description de chacune d’elles.</span><span class="sxs-lookup"><span data-stu-id="365c1-105">This section contains all the commands and their parameters, with a brief description of each.</span></span>

**<span data-ttu-id="365c1-106">Important</span><span class="sxs-lookup"><span data-stu-id="365c1-106">Important</span></span>**  
-   <span data-ttu-id="365c1-107">Tous les caractères de barre oblique inverse doivent faire l’objet d’une séquence d’échappement en utilisant une barre oblique inverse précédente ou le chemin ne sera pas analysé correctement.</span><span class="sxs-lookup"><span data-stu-id="365c1-107">All backslash characters must be escaped using a preceding backslash, or the path will not be parsed correctly.</span></span>

-   <span data-ttu-id="365c1-108">Si vous utilisez un programme d’appel pour appeler SFTMIME avec **CreateProcess**, vous devez vous assurer que le premier paramètre est le chemin d’accès à sftmime.exe.</span><span class="sxs-lookup"><span data-stu-id="365c1-108">If you are using a calling program to invoke SFTMIME with **CreateProcess**, you must ensure that the first parameter is the path to sftmime.exe.</span></span>

-   <span data-ttu-id="365c1-109">La sortie de la commande **obj** de la requête SFTMIME ne peut pas être canalisée vers la commande **findstr** pour rechercher une chaîne.</span><span class="sxs-lookup"><span data-stu-id="365c1-109">The output of the SFTMIME **QUERY OBJ** command cannot be piped to the **findstr** command to search for a string.</span></span>

-   <span data-ttu-id="365c1-110">L’utilisation du commutateur **Global** nécessite des droits d’administrateur local.</span><span class="sxs-lookup"><span data-stu-id="365c1-110">Use of the **GLOBAL** switch requires local administrator rights.</span></span>

-   <span data-ttu-id="365c1-111">L’utilisation de chemins courts et de chemins relatifs peut entraîner des résultats inattendus et être évitée.</span><span class="sxs-lookup"><span data-stu-id="365c1-111">Use of short paths and relative paths can lead to unexpected results and should be avoided.</span></span> <span data-ttu-id="365c1-112">Utilisez toujours des chemins complets.</span><span class="sxs-lookup"><span data-stu-id="365c1-112">Always use full paths.</span></span>

 

## <span data-ttu-id="365c1-113">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="365c1-113">In This Section</span></span>


[<span data-ttu-id="365c1-114">ADD APP</span><span class="sxs-lookup"><span data-stu-id="365c1-114">ADD APP</span></span>](add-app.md)

[<span data-ttu-id="365c1-115">ADD PACKAGE</span><span class="sxs-lookup"><span data-stu-id="365c1-115">ADD PACKAGE</span></span>](add-package.md)

[<span data-ttu-id="365c1-116">ADD SERVER</span><span class="sxs-lookup"><span data-stu-id="365c1-116">ADD SERVER</span></span>](add-server.md)

[<span data-ttu-id="365c1-117">ADD TYPE</span><span class="sxs-lookup"><span data-stu-id="365c1-117">ADD TYPE</span></span>](add-type.md)

[<span data-ttu-id="365c1-118">CLEAR APP</span><span class="sxs-lookup"><span data-stu-id="365c1-118">CLEAR APP</span></span>](clear-app.md)

[<span data-ttu-id="365c1-119">CLEAR OBJ</span><span class="sxs-lookup"><span data-stu-id="365c1-119">CLEAR OBJ</span></span>](clear-obj.md)

[<span data-ttu-id="365c1-120">CONFIGURE APP</span><span class="sxs-lookup"><span data-stu-id="365c1-120">CONFIGURE APP</span></span>](configure-app.md)

[<span data-ttu-id="365c1-121">CONFIGURE PACKAGE</span><span class="sxs-lookup"><span data-stu-id="365c1-121">CONFIGURE PACKAGE</span></span>](configure-package.md)

[<span data-ttu-id="365c1-122">CONFIGURE SERVER</span><span class="sxs-lookup"><span data-stu-id="365c1-122">CONFIGURE SERVER</span></span>](configure-server.md)

[<span data-ttu-id="365c1-123">CONFIGURE TYPE</span><span class="sxs-lookup"><span data-stu-id="365c1-123">CONFIGURE TYPE</span></span>](configure-type.md)

[<span data-ttu-id="365c1-124">DELETE APP</span><span class="sxs-lookup"><span data-stu-id="365c1-124">DELETE APP</span></span>](delete-app.md)

[<span data-ttu-id="365c1-125">DELETE OBJ</span><span class="sxs-lookup"><span data-stu-id="365c1-125">DELETE OBJ</span></span>](delete-obj.md)

[<span data-ttu-id="365c1-126">DELETE PACKAGE</span><span class="sxs-lookup"><span data-stu-id="365c1-126">DELETE PACKAGE</span></span>](delete-package.md)

[<span data-ttu-id="365c1-127">DELETE SERVER</span><span class="sxs-lookup"><span data-stu-id="365c1-127">DELETE SERVER</span></span>](delete-server.md)

[<span data-ttu-id="365c1-128">DELETE TYPE</span><span class="sxs-lookup"><span data-stu-id="365c1-128">DELETE TYPE</span></span>](delete-type.md)

[<span data-ttu-id="365c1-129">HELP</span><span class="sxs-lookup"><span data-stu-id="365c1-129">HELP</span></span>](help.md)

[<span data-ttu-id="365c1-130">LOAD APP</span><span class="sxs-lookup"><span data-stu-id="365c1-130">LOAD APP</span></span>](load-app.md)

[<span data-ttu-id="365c1-131">LOAD PACKAGE</span><span class="sxs-lookup"><span data-stu-id="365c1-131">LOAD PACKAGE</span></span>](load-package.md)

[<span data-ttu-id="365c1-132">LOCK APP</span><span class="sxs-lookup"><span data-stu-id="365c1-132">LOCK APP</span></span>](lock-app.md)

[<span data-ttu-id="365c1-133">PUBLISH APP</span><span class="sxs-lookup"><span data-stu-id="365c1-133">PUBLISH APP</span></span>](publish-app.md)

[<span data-ttu-id="365c1-134">PUBLISH PACKAGE</span><span class="sxs-lookup"><span data-stu-id="365c1-134">PUBLISH PACKAGE</span></span>](publish-package.md)

[<span data-ttu-id="365c1-135">QUERY OBJ</span><span class="sxs-lookup"><span data-stu-id="365c1-135">QUERY OBJ</span></span>](query-obj.md)

[<span data-ttu-id="365c1-136">REFRESH SERVER</span><span class="sxs-lookup"><span data-stu-id="365c1-136">REFRESH SERVER</span></span>](refresh-server.md)

[<span data-ttu-id="365c1-137">REPAIR APP</span><span class="sxs-lookup"><span data-stu-id="365c1-137">REPAIR APP</span></span>](repair-app.md)

[<span data-ttu-id="365c1-138">UNLOAD APP</span><span class="sxs-lookup"><span data-stu-id="365c1-138">UNLOAD APP</span></span>](unload-app.md)

[<span data-ttu-id="365c1-139">UNLOAD PACKAGE</span><span class="sxs-lookup"><span data-stu-id="365c1-139">UNLOAD PACKAGE</span></span>](unload-package.md)

[<span data-ttu-id="365c1-140">UNLOCK APP</span><span class="sxs-lookup"><span data-stu-id="365c1-140">UNLOCK APP</span></span>](unlock-app.md)

[<span data-ttu-id="365c1-141">UNPUBLISH PACKAGE</span><span class="sxs-lookup"><span data-stu-id="365c1-141">UNPUBLISH PACKAGE</span></span>](unpublish-package.md)

 

 




