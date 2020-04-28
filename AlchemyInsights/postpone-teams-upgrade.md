---
title: Csapatok frissítésének elhalasztása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: fcf724e335bd6a7cb4801d9b2789447befc06ff7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912513"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>A Microsoft által vezérelt Teams-frissítés elhalasztása

**Fontos:** Segíthetünk a javításhoz egy támogatási diagnosztika használatával, de úgy tűnik, hogy nem használja az Új Felügyeleti központot. Az Új felügyeleti központ használatához csúsztassa a jobb felső sarokban az **új felügyeleti központot** jobbra jelző kapcsolót. Az Új felügyeleti központ segítségével kattintson a **Segítségre van szüksége?** widgetre, írja be a "Csapatok frissítésének elhalasztása" kifejezést, majd kövesse a diagnosztikai eszközök utasításait.

Ha a Microsoft által vezérelt automatikus frissítéssel kapcsolatban kapott kommunikációt a Skype Vállalati verzióról a Microsoft Teamsprogramra, és az automatikus frissítést egy későbbi időpontra szeretné halasztani, a globális rendszergazda bejelentkezhet a [Teams Felügyeleti portálra,](https://admin.teams.microsoft.com/dashboard) és miután a Microsoft Teams frissítés e-frissítése gombbal **kiválasztotta** a Frissítés állapotát gombot, válassza a **Halasztás gombot.** A bérlő Microsoft Teamsre történő automatikus frissítésének új dátumának megtekintéséhez frissítse a Teams felügyeleti portállapját.

**Megjegyzés:** A **Halasztás** gomb csak akkor érhető el, ha megkapta az üzenetközpont értesítését az automatikus frissítésről. 

A globális rendszergazdák a [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) programot is futtathatják, hogy többet megtudjanak az aktuális frissítési állapotukról.
