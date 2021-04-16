---
title: A Teams frissítésének elhalasztása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801233"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>A Microsoft-alapú Teams-frissítés elhalasztása

**Fontos:** Segíthetünk a hiba kijavításában egy támogatási diagnosztikai eszköz használatával, de úgy tűnik, hogy ön nem az Új felügyeleti központot használja. Az Új felügyeleti központ megnyitásához húzza a jobb felső  sarokban az Új felügyeleti központ csúszkával jobbra található kapcsolót. Az Új felügyeleti központban kattintson a Segítségre van **szüksége?** vezérlőre, írja be a "Teams-frissítés elhalasztása" parancsot, majd az utasításokat használva futtassa a diagnosztikai adatokat.

Ha a Microsoft által vezetett automatikus frissítésről kapott kommunikációt a Skype Vállalati verzióról a Microsoft Teamsre, és későbbre szeretné halasztani az  automatikus frissítést, a globális  rendszergazda bejelentkezhet a [Teams](https://admin.teams.microsoft.com/dashboard) felügyeleti portálra, és miután a Microsoft Teams Frissítés csoportban a Frissítési állapot gombra kattintott, válassza a Elhalasztás gombot. A Teams felügyeleti portál lapját frissítve láthatja a bérlői fiók Microsoft Teamsre való automatikus frissítésének új dátumát.

**Megjegyzés:** A **Halasztás** gomb csak akkor érhető el, ha megkapta az üzenetközpont értesítését az automatikus frissítésről. 

A globális rendszergazdák a [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) futtatásával is tudnak többet megtudni aktuális frissítési állapotukról.
