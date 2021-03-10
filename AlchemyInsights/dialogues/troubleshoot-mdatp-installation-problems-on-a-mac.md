---
title: Az MDATP telepítési problémáinak elhárítása Mac gépen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694279"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="acc69-102">Az MDATP telepítési problémáinak elhárítása Mac gépen</span><span class="sxs-lookup"><span data-stu-id="acc69-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="acc69-103">Ha a kézi  telepítés meghiúsul, a telepítővarázsló Összegzés lapján a következő hibaüzenet jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="acc69-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="acc69-104">"Hiba történt a telepítés során.</span><span class="sxs-lookup"><span data-stu-id="acc69-104">"An error occurred during installation.</span></span> <span data-ttu-id="acc69-105">A telepítő hibát észlelt, amely a telepítés sikertelen voltát okozta.</span><span class="sxs-lookup"><span data-stu-id="acc69-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="acc69-106">Segítségért forduljon a szoftver gyártójához."</span><span class="sxs-lookup"><span data-stu-id="acc69-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="acc69-107">A MDM-telepítések esetén a lapon általános telepítési hiba is látható.</span><span class="sxs-lookup"><span data-stu-id="acc69-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="acc69-108">Bár pontos hibákat nem jelenítünk meg a végfelhasználóknak, a telepítés előrehaladását egy naplófájlban tartjuk, a **/Library/Logs/Microsoft/mdatp/install.log** fájlban.</span><span class="sxs-lookup"><span data-stu-id="acc69-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="acc69-109">Minden telepítési munkamenet hozzáfűzi ezt a naplófájlt.</span><span class="sxs-lookup"><span data-stu-id="acc69-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="acc69-110">Ha csak az utolsó telepítési munkamenet kimenetét kimenetként, használja `sed` a .</span><span class="sxs-lookup"><span data-stu-id="acc69-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="acc69-111">További információt a Mac Microsoft Defender ATP telepítési [hibáinak elhárítása témakörben olvashat.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="acc69-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
