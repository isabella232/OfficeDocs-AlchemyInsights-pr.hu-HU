---
title: A Teams bejelentkezési hibájának kezelése AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357879"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="538ac-102">A Teams bejelentkezési hibájának kezelése AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="538ac-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="538ac-103">Amikor bejelentkezik a Microsoft Teamsbe, a következő hibaüzenet jelenhet meg: **Sajnáljuk, de az AADSTS900041-ben történő aláírással nem sikerül aláírnunk: A kérés nincs megfelelően formázva. A "login_hint" paraméter duplikálva van.**</span><span class="sxs-lookup"><span data-stu-id="538ac-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="538ac-104">A probléma megoldásához győződjön meg arról, hogy a Microsoft Teams-ügyfelek frissülnek.</span><span class="sxs-lookup"><span data-stu-id="538ac-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="538ac-105">Az ügyfél frissítésével kapcsolatos további tudnivalókért olvassa el a Microsoft Teams frissítése című [témakört.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="538ac-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="538ac-106">Ha valamilyen okból nem tudja frissíteni az ügyfelet, a kijelentkezés törli a legtöbb gyorsítótárazott adatot.</span><span class="sxs-lookup"><span data-stu-id="538ac-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="538ac-107">Ha azonban a kijelentkezés/bejelentkezés után is problémák merülnek fel, lépjen ki a Teamsből, és törölje az ügyfél gyorsítótárát az alábbi módon:</span><span class="sxs-lookup"><span data-stu-id="538ac-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="538ac-108">Zárja be a Microsoft Teamst.</span><span class="sxs-lookup"><span data-stu-id="538ac-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="538ac-109">Nyissa meg a következőt: %appdata%\microsoft\teams és törölje az összes fájlt.</span><span class="sxs-lookup"><span data-stu-id="538ac-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="538ac-110">Nyissa meg újra a Microsoft Teamst.</span><span class="sxs-lookup"><span data-stu-id="538ac-110">Reopen Microsoft Teams.</span></span>
