---
title: A Microsoft Edge-re vonatkozó speciális hitelesítési fogalmak
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573521"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>A Microsoft Edge-re vonatkozó speciális hitelesítési fogalmak

A Microsoft Edge-re vonatkozó speciális hitelesítési fogalmak a következők:

**Proaktív hitelesítés**

Ha engedélyezi a [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -házirendet, a Microsoft Edge megpróbálja proaktívan hitelesíteni a bejelentkezett felhasználókat a Microsoft Services szolgáltatáson keresztül. Rendszeres időközönként egy online szolgáltatással ellenőrizheti, hogy egy olyan frissített jegyzékfájlt szeretne-e használni, amely a proaktív hitelesítésre vonatkozó konfigurációt tartalmazza.

Előnyök: a proaktív hitelesítés a legfontosabb szolgáltatásokhoz (például az Office új lap lapjához) való hitelesítést engedélyezi. Ha a Bing a keresőmotorként van használatban, a proaktív hitelesítés javítja a címsor működését, és segít a keresés eredményének a vállalati igényekhez való személyre szabásában.

**Windows Hello CredUI NTLM-hitelesítéshez**

Ha az egyszeri bejelentkezés (SSO) nem érhető el, ha egy webhely az NTLM vagy az egyeztetési mechanizmuson keresztül próbál meg bekapcsolódni a felhasználóhoz, ez a funkció lehetővé teszi, hogy a felhasználó megossza az operációs rendszer hitelesítő adatait a webhellyel, és a Windows Hello cred felhasználói felülete segítségével kielégítse a hitelesítési kihívást. Ez a bejelentkezési folyamat csak a Windows 10 rendszerben jelenik meg, és csak azoknál a felhasználóknál, akik NTLM-vagy értekezlet-összehívási probléma esetén nem kapnak SSO-t.

**A mentett jelszavak használata automatikusan történő bejelentkezéshez**

Azok a felhasználók, akik a Microsoft Edge-ben mentették a jelszavakat, engedélyezhetik az automatikus bejelentkezést olyan webhelyekre, ahol a hitelesítő adatok találhatók. A felhasználók a edge://settings/passwords-ban be-vagy kikapcsolhatja ezt a funkcióját, és a [jelszó-kezelő](https://go.microsoft.com/fwlink/?linkid=2134622) házirendben is konfigurálhatók.
