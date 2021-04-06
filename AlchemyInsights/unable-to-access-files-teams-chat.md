---
title: Nem lehet hozzáférni a Teams csevegésben megosztott fájlokhoz
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51595814"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="c5565-102">Nem lehet hozzáférni a Teams csevegésben megosztott fájlokhoz</span><span class="sxs-lookup"><span data-stu-id="c5565-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="c5565-103">A Microsoft Teamsben a felhasználó által a csevegőablakban megosztott fájlok automatikusan a megosztást használó felhasználó OneDrive-webhelyén tárolódnak.</span><span class="sxs-lookup"><span data-stu-id="c5565-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="c5565-104">Amikor egy másik felhasználó megpróbálja megnyitni a fájlt a Teamsben, és a "Nincs hozzáférése ehhez a fájlhoz" hibaüzenet jelenik meg, a probléma oka az, hogy a Korlátozott hozzáférésű felhasználók engedélyeinek zárolási módja aktív a OneDrive-webhelyen.</span><span class="sxs-lookup"><span data-stu-id="c5565-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="c5565-105">A Funkció OneDrive-webhelyen való letiltására vonatkozó utasításokat a Hiba [fájl megnyitásakor a Teamsben .](https://go.microsoft.com/fwlink/?linkid=2155733)</span><span class="sxs-lookup"><span data-stu-id="c5565-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="c5565-106">Ellenőrizze, hogy egy másik felhasználó hozzáfér-e a OneDrive-webhelyhez, és biztosítson-e hozzáférést a OneDrive-fájlok és -mappák megosztása [terület útmutatását követve.](https://go.microsoft.com/fwlink/?linkid=2156017)</span><span class="sxs-lookup"><span data-stu-id="c5565-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>