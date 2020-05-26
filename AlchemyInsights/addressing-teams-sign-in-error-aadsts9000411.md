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
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>A Teams bejelentkezési hibájának kezelése AADSTS9000411

Amikor bejelentkezik a Microsoft Teamsbe, a következő hibaüzenet jelenhet meg: **Sajnáljuk, de az AADSTS900041-ben történő aláírással nem sikerül aláírnunk: A kérés nincs megfelelően formázva. A "login_hint" paraméter duplikálva van.**

A probléma megoldásához győződjön meg arról, hogy a Microsoft Teams-ügyfelek frissülnek. Az ügyfél frissítésével kapcsolatos további tudnivalókért olvassa el a Microsoft Teams frissítése című [témakört.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Ha valamilyen okból nem tudja frissíteni az ügyfelet, a kijelentkezés törli a legtöbb gyorsítótárazott adatot. Ha azonban a kijelentkezés/bejelentkezés után is problémák merülnek fel, lépjen ki a Teamsből, és törölje az ügyfél gyorsítótárát az alábbi módon:
1. Zárja be a Microsoft Teamst.
2. Nyissa meg a következőt: %appdata%\microsoft\teams és törölje az összes fájlt.
3. Nyissa meg újra a Microsoft Teamst.
