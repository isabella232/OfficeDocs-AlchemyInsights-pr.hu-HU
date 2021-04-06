---
title: Az Office és a OneDrive telepítése a Windows Virtuális asztalon
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595849"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="6b0ad-102">Az Office és a OneDrive telepítése a Windows Virtuális asztalon</span><span class="sxs-lookup"><span data-stu-id="6b0ad-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="6b0ad-103">[FŐ VHD-kép előkészítése és testreszabása.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)</span><span class="sxs-lookup"><span data-stu-id="6b0ad-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="6b0ad-104">Ha még nem hozta létre, hozzon létre egy virtuális gépet (VM).</span><span class="sxs-lookup"><span data-stu-id="6b0ad-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="6b0ad-105">[Telepítse az Office-t megosztott számítógép-aktiválási módban.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="6b0ad-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="6b0ad-106">A megosztott számítógép aktiválása lehetővé teszi, hogy több felhasználó hozzáférjen az Office-hoz.</span><span class="sxs-lookup"><span data-stu-id="6b0ad-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="6b0ad-107">[Telepítse a OneDrive-ot gépenkénti módban.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="6b0ad-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="6b0ad-108">A OneDrive felhasználónként általában telepítve van, de itt gépenként kell telepíteni.</span><span class="sxs-lookup"><span data-stu-id="6b0ad-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>