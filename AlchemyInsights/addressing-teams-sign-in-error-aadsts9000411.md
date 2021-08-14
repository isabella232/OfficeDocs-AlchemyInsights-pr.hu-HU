---
title: Bejelentkezési Teams AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953028"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Bejelentkezési Teams AADSTS9000411

Az Microsoft Teams-be való bejelentkezéskor a következő hibaüzenet jelenhet meg: Sajnáljuk, de nem sikerült bejelentkeznie az **AADSTS9000411ba: A kérés formázása nem megfelelő. A "login_hint" paraméter duplikálva van.**

A probléma megoldásához győződjön meg arról, hogy Microsoft Teams az ügyfél frissítése. Az ügyfélprogram frissítéséről további információt a Frissítési [Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Ha valamilyen okból kifolyólag nem tudja frissíteni az ügyfelet, az ügyfél kijelentkezése törli a legtöbb gyorsítótárazott adatot. Ha azonban az embléma/bejelentkezés után továbbra is problémákat lép fel, lépjen ki a Teams és törölje az ügyfél-gyorsítótárat az alábbi lépéseket követően:
1. Zárja be Microsoft Teams.
2. Kattintson az %appdata%\microsoft\teams mappára, és törölje az összes fájlt.
3. Nyissa meg Microsoft Teams.
