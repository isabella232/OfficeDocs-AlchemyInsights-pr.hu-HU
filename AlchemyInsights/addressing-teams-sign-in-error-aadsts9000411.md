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
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>A Teams bejelentkezési hibaének kezelése AADSTS9000411

Amikor bejelentkezik a Microsoft Teamsbe, a következő hibaüzenet jelenhet meg: Sajnáljuk, de nem sikerült bejelentkeznie az **AADSTS9000411ba: A kérés formázása nem megfelelő. A "login_hint" paraméter duplikálva van.**

A probléma megoldásához gondoskodjon arról, hogy a Microsoft Teams-ügyfelek frissültek. Az ügyfél frissítéséről további információt A [Microsoft Teams frissítése.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Ha valamilyen okból kifolyólag nem tudja frissíteni az ügyfelet, az ügyfél kijelentkezése törli a legtöbb gyorsítótárazott adatot. Ha azonban az embléma/bejelentkezés után továbbra is problémákat lép fel, lépjen ki a Teamsből, és az alábbi lépéseket követően törölje az ügyfél-gyorsítótárat:
1. Zárja be a Microsoft Teamst.
2. Kattintson az %appdata%\microsoft\teams mappára, és törölje az összes fájlt.
3. Nyissa meg újra a Microsoft Teamst.
