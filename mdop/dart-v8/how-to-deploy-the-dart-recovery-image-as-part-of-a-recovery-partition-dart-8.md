---
title: Procédure pour déployer l'image de récupération DaRT dans le cadre d'une partition de récupération
description: Procédure pour déployer l'image de récupération DaRT dans le cadre d'une partition de récupération
author: dansimp
ms.assetid: 07c5d539-51d9-4759-adc7-72b40d5d7bb3
ms.reviewer: ''
manager: dansimp
ms.author: dansimp
ms.pagetype: mdop
ms.mktglfcycl: support
ms.sitesec: library
ms.prod: w10
ms.date: 08/30/2016
ms.openlocfilehash: e3647d684f64a0635e2875314498bde841204369
ms.sourcegitcommit: 354664bc527d93f80687cd2eba70d1eea024c7c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2020
ms.locfileid: "10810523"
---
# <span data-ttu-id="17347-103">Procédure pour déployer l'image de récupération DaRT dans le cadre d'une partition de récupération</span><span class="sxs-lookup"><span data-stu-id="17347-103">How to Deploy the DaRT Recovery Image as Part of a Recovery Partition</span></span>


<span data-ttu-id="17347-104">Lorsque vous avez terminé d’exécuter l’Assistant image de récupération de Microsoft Diagnostics et Recovery Tools (DaRT) 8,0 et créé l’image de récupération, vous pouvez extraire le fichier Boot. wim du fichier image ISO et le déployer en tant que partition de récupération dans une image Windows 8.</span><span class="sxs-lookup"><span data-stu-id="17347-104">After you have finished running the Microsoft Diagnostics and Recovery Toolset (DaRT) 8.0 Recovery Image wizard and created the recovery image, you can extract the boot.wim file from the ISO image file and deploy it as a recovery partition in a Windows 8 image.</span></span> <span data-ttu-id="17347-105">Il est recommandé d’utiliser une partition, car tous les problèmes d’endommagement qui empêchent le système d’exploitation Windows de démarrer pourraient empêcher l’image de récupération de démarrer.</span><span class="sxs-lookup"><span data-stu-id="17347-105">A partition is recommended, because any corruption issues that prevent the Windows operating system from starting would also prevent the recovery image from starting.</span></span> <span data-ttu-id="17347-106">Par ailleurs, une partition séparée évite d’avoir recours à la clé de récupération BitLocker.</span><span class="sxs-lookup"><span data-stu-id="17347-106">A separate partition also eliminates the need to provide the BitLocker recovery key twice.</span></span> <span data-ttu-id="17347-107">Envisagez de masquer la partition pour empêcher les utilisateurs de stocker des fichiers sur celle-ci.</span><span class="sxs-lookup"><span data-stu-id="17347-107">Consider hiding the partition to prevent users from storing files on it.</span></span>

**<span data-ttu-id="17347-108">Pour déployer DaRT dans la partition de récupération d’une image Windows 8</span><span class="sxs-lookup"><span data-stu-id="17347-108">To deploy DaRT in the recovery partition of a Windows 8 image</span></span>**

1.  <span data-ttu-id="17347-109">Créez une partition cible dans votre image Windows 8 égale ou supérieure à la taille du fichier image ISO que vous avez créé à l’aide de l' **Assistant image de récupération 8,0 de DART**.</span><span class="sxs-lookup"><span data-stu-id="17347-109">Create a target partition in your Windows 8 image that is equal to or greater than the size of the ISO image file that you created by using the **DaRT 8.0 Recovery Image wizard**.</span></span>

    <span data-ttu-id="17347-110">La taille minimale requise pour une partition DaRT est de 500 Mo pour s’adapter à la fonctionnalité de connexion à distance dans DaRT.</span><span class="sxs-lookup"><span data-stu-id="17347-110">The minimum size required for a DaRT partition is 500MB to accommodate the remote connection functionality in DaRT.</span></span>

2.  <span data-ttu-id="17347-111">Extrayez le fichier Boot. wim du fichier image ISO DaRT.</span><span class="sxs-lookup"><span data-stu-id="17347-111">Extract the boot.wim file from the DaRT ISO image file.</span></span>

    1.  <span data-ttu-id="17347-112">À l’aide de la méthode préférée de votre entreprise, montez le fichier image ISO que vous avez créé dans la page **créer une image de démarrage** .</span><span class="sxs-lookup"><span data-stu-id="17347-112">Using your company’s preferred method, mount the ISO image file that you created on the **Create Startup Image** page.</span></span>

    2.  <span data-ttu-id="17347-113">Ouvrez le fichier image ISO et copiez le fichier Boot. wim du dossier \\sources de l’image montée vers un emplacement sur votre ordinateur ou sur un lecteur externe.</span><span class="sxs-lookup"><span data-stu-id="17347-113">Open the ISO image file and copy the boot.wim file from the \\sources folder in the mounted image to a location on your computer or on an external drive.</span></span>

        <span data-ttu-id="17347-114">**Remarques**  Si vous avez gravé un CD, un DVD ou une connexion USB de l’image de récupération, vous pouvez ouvrir les fichiers sur le média amovible et copier le fichier Boot. wim à partir du dossier \\sources.</span><span class="sxs-lookup"><span data-stu-id="17347-114">**Note** If you burned a CD, DVD, or USB of the recovery image, you can open the files on the removable media and copy the boot.wim file from the \\sources folder.</span></span> <span data-ttu-id="17347-115">Si vous copiez le fichier Boot. wim, vous n’avez pas besoin de monter l’image.</span><span class="sxs-lookup"><span data-stu-id="17347-115">If you copy boot.wim file, you don’t need to mount the image.</span></span>

         

3.  <span data-ttu-id="17347-116">Utilisez le fichier Boot. wim pour créer une partition de récupération démarrable en utilisant la méthode standard de votre entreprise pour créer une image Windows RE personnalisée.</span><span class="sxs-lookup"><span data-stu-id="17347-116">Use the boot.wim file to create a bootable recovery partition by using your company’s standard method for creating a custom Windows RE image.</span></span>

    <span data-ttu-id="17347-117">Pour plus d’informations sur la création et la personnalisation d’une partition de récupération, voir [Personnalisation de l’utilisation de Windows RE](https://go.microsoft.com/fwlink/?LinkId=214222).</span><span class="sxs-lookup"><span data-stu-id="17347-117">For more information about how to create or customize a recovery partition, see [Customizing the Windows RE Experience](https://go.microsoft.com/fwlink/?LinkId=214222).</span></span>

4.  <span data-ttu-id="17347-118">Remplacez la partition cible dans votre image Windows 8 par la partition de récupération.</span><span class="sxs-lookup"><span data-stu-id="17347-118">Replace the target partition in your Windows 8 image with the recovery partition.</span></span>

    <span data-ttu-id="17347-119">Pour plus d’informations sur le déploiement d’une solution de récupération pour réinstaller l’image de fabrique en cas de panne du système, voir [déployer une image de récupération du système](https://go.microsoft.com/fwlink/?LinkId=214221).</span><span class="sxs-lookup"><span data-stu-id="17347-119">For more information about how to deploy a recovery solution to reinstall the factory image in the event of a system failure, see [Deploy a System Recovery Image](https://go.microsoft.com/fwlink/?LinkId=214221).</span></span>

## <span data-ttu-id="17347-120">Rubriques connexes</span><span class="sxs-lookup"><span data-stu-id="17347-120">Related topics</span></span>


[<span data-ttu-id="17347-121">Création de l'image de récupération DaRT8.0</span><span class="sxs-lookup"><span data-stu-id="17347-121">Creating the DaRT 8.0 Recovery Image</span></span>](creating-the-dart-80-recovery-image-dart-8.md)

[<span data-ttu-id="17347-122">Déploiement de l'image de récupération DaRT</span><span class="sxs-lookup"><span data-stu-id="17347-122">Deploying the DaRT Recovery Image</span></span>](deploying-the-dart-recovery-image-dart-8.md)

[<span data-ttu-id="17347-123">Planification de DaRT8.0</span><span class="sxs-lookup"><span data-stu-id="17347-123">Planning for DaRT 8.0</span></span>](planning-for-dart-80-dart-8.md)

 

 




