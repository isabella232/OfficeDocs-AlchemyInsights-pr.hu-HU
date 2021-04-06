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
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Az Office és a OneDrive telepítése a Windows Virtuális asztalon

1. [FŐ VHD-kép előkészítése és testreszabása.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image) Ha még nem hozta létre, hozzon létre egy virtuális gépet (VM).

1. [Telepítse az Office-t megosztott számítógép-aktiválási módban.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) A megosztott számítógép aktiválása lehetővé teszi, hogy több felhasználó hozzáférjen az Office-hoz.

1. [Telepítse a OneDrive-ot gépenkénti módban.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) A OneDrive felhasználónként általában telepítve van, de itt gépenként kell telepíteni.