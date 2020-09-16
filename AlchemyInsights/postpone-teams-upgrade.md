---
title: A Teams frissítésének elhalasztása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741773"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>A Microsoft-alapú Teams frissítésének elhalasztása

**Fontos**: ezt a segítséget akkor tudjuk kijavítani, ha támogatási diagnosztikai lehetőségeket használ, de nem az új felügyeleti központot használja. Ha az új felügyeleti központot szeretné használni, húzza a jobb felső sarokban lévő kapcsolót az **új felügyeleti központ** jobb oldalán. Használja az új felügyeleti központot, és kattintson a **segítségre van szüksége?** elemre, írja be a "elhalasztja a Teams upgrade" parancsot, majd kövesse a megjelenő utasításokat a diagnosztika futtatásához.

Ha a Skype vállalati verzióról a Microsoft Teams-re szeretne kommunikálni a Microsoft-alapú automatizált frissítésről, és az automatikus frissítést későbbi dátumra szeretné halasztani, a globális rendszergazda bejelentkezhet a [Teams felügyeleti portálra](https://admin.teams.microsoft.com/dashboard) , és a Microsoft Teams upgrade csoportban a frissítés **állapota** gomb választása után válassza a **Elhalasztva** gombot. Ha szeretné megtekinteni a bérlő automatikus frissítésének új dátumát a Microsoft Teams szolgáltatásban, frissítse a Teams felügyeleti portál lapját.

**Megjegyzés:** Az **elhalasztás** gomb csak akkor érhető el, ha az automatikus frissítésről értesítést kapott az üzenetközpont értesítésben. 

A globális rendszergazdák a [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) is megtekinthetik a jelenlegi frissítés állapotát.
