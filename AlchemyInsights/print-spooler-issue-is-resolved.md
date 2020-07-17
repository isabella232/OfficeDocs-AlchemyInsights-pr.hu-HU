---
title: A nyomtatásisor-kezelővel kapcsolatos probléma megoldódott
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088339"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="951f8-102">A nyomtatásisor-kezelővel kapcsolatos probléma megoldódott</span><span class="sxs-lookup"><span data-stu-id="951f8-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="951f8-103">Ha az eszközt frissítette a Windows 10 **OS Build 19041.329**rendszerrel, előfordulhat, hogy olyan problémát észlelt, amely miatt bizonyos nyomtatók nyomtatása nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="951f8-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="951f8-104">Előfordulhat, hogy a nyomtatásisor-kezelő nyomtatás közben hibát jelez vagy váratlanul bezár, és az érintett nyomtató nem ad ki kimenetet.</span><span class="sxs-lookup"><span data-stu-id="951f8-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="951f8-105">A probléma az **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)operációs rendszer ben oldódott meg.</span><span class="sxs-lookup"><span data-stu-id="951f8-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="951f8-106">**Folyamatban lévő vizsgálat**</span><span class="sxs-lookup"><span data-stu-id="951f8-106">**Ongoing investigation**</span></span>

<span data-ttu-id="951f8-107">A Helyi biztonsági társalrendszer -szolgáltatás (LSASS) fájlja (**Isass.exe**) a következő hibaüzenettel rendelkező egyes eszközökön meghibásodhat: "A kritikus rendszerfolyamat, C:\WINDOWS\system32\Isass.exe, a c0000008 állapotkóddal nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="951f8-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="951f8-108">A gépet most újra kell indítani".</span><span class="sxs-lookup"><span data-stu-id="951f8-108">The machine must now be restarted".</span></span>  <span data-ttu-id="951f8-109">**A Microsoft dolgozik egy megoldáson, és egy közelgő kiadásban frissítést fog biztosítani.**</span><span class="sxs-lookup"><span data-stu-id="951f8-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="951f8-110">További információért kérjük, tekintse meg a [Windows 10 2004-es verzió ismert problémáit.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)</span><span class="sxs-lookup"><span data-stu-id="951f8-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>