---
title: 'Csapatok frissítésének elhalasztása '
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
ms.openlocfilehash: 27f3dc123590f3199d6a984d7e9a4db3918ac9cb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758864"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>A Microsoft által vezérelt Teams-frissítés elhalasztása

Ha a Microsoft által vezérelt automatikus frissítésről kapott kommunikációt a Skype Vállalati verzióról a Microsoft Teamsre, és az automatikus frissítést egy későbbi időpontra szeretné halasztani, globális rendszergazdája bejelentkezhet a [Teams Felügyeleti portálra,](https://admin.teams.microsoft.com/dashboard) és kiválaszthatja a **Halasztás gombot.** A bérlő Microsoft Teamsre történő automatikus frissítésének új dátumának megtekintéséhez frissítse a Teams felügyeleti portállapját.

**Megjegyzés:** A **Halasztás** gomb csak akkor érhető el, ha megkapta az üzenetközpont értesítését az automatikus frissítésről. 

A globális rendszergazdák a [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) programot is futtathatják, hogy többet megtudjanak az aktuális frissítési állapotukról. 