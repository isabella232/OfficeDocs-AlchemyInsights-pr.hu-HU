---
title: A Teams bejelentkezési hibaének kezelése AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821989"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="65cb1-102">A Teams bejelentkezési hibaének kezelése AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="65cb1-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="65cb1-103">Amikor bejelentkezik a Microsoft Teamsbe, a következő hibaüzenet jelenhet meg: Sajnáljuk, de nem sikerült bejelentkeznie az **AADSTS9000411ba: A kérés formázása nem megfelelő. A "login_hint" paraméter duplikálva van.**</span><span class="sxs-lookup"><span data-stu-id="65cb1-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="65cb1-104">A probléma megoldásához gondoskodjon arról, hogy a Microsoft Teams-ügyfelek frissültek.</span><span class="sxs-lookup"><span data-stu-id="65cb1-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="65cb1-105">Az ügyfél frissítéséről további információt A [Microsoft Teams frissítése.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="65cb1-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="65cb1-106">Ha valamilyen okból kifolyólag nem tudja frissíteni az ügyfelet, az ügyfél kijelentkezése törli a legtöbb gyorsítótárazott adatot.</span><span class="sxs-lookup"><span data-stu-id="65cb1-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="65cb1-107">Ha azonban az embléma/bejelentkezés után továbbra is problémákat lép fel, lépjen ki a Teamsből, és az alábbi lépéseket követően törölje az ügyfél-gyorsítótárat:</span><span class="sxs-lookup"><span data-stu-id="65cb1-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="65cb1-108">Zárja be a Microsoft Teamst.</span><span class="sxs-lookup"><span data-stu-id="65cb1-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="65cb1-109">Kattintson az %appdata%\microsoft\teams mappára, és törölje az összes fájlt.</span><span class="sxs-lookup"><span data-stu-id="65cb1-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="65cb1-110">Nyissa meg újra a Microsoft Teamst.</span><span class="sxs-lookup"><span data-stu-id="65cb1-110">Reopen Microsoft Teams.</span></span>
