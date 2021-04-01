---
title: A Microsoft Edge beállítása alapértelmezett böngészőként tartományhoz csatlakozott eszközön
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491584"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="ea664-102">A Microsoft Edge beállítása alapértelmezett böngészőként tartományhoz csatlakozott eszközön</span><span class="sxs-lookup"><span data-stu-id="ea664-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="ea664-103">Állítsa be a Microsoft Edge-et alapértelmezett böngészőként:</span><span class="sxs-lookup"><span data-stu-id="ea664-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="ea664-104">[Hozzon létre egy alapértelmezett társítási konfigurációs fájlt,](https://go.microsoft.com/fwlink/?linkid=2132437) és tárolja helyileg vagy egy hálózati megosztáson.</span><span class="sxs-lookup"><span data-stu-id="ea664-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="ea664-105">Nyissa meg a Csoportházirend-szerkesztőt, majd nyissa meg a **Számítógép**  >  **konfigurációja felügyeleti sablonjai**  >  **Windows Components** File Explorer  >  **gombra.**</span><span class="sxs-lookup"><span data-stu-id="ea664-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="ea664-106">Válassza **az Alapértelmezett társítások konfigurációs fájljának beállítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ea664-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="ea664-107">Válassza **a Házirend-beállítás**, majd az Engedélyezve **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ea664-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="ea664-108">A **Beállítások alatt** adja meg az alapértelmezett társítások konfigurációs fájljának helyét, majd válassza az OK **gombot.**</span><span class="sxs-lookup"><span data-stu-id="ea664-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
