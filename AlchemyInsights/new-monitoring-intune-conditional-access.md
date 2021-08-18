---
title: Intune feltételes hozzáférés figyelése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327559"
---
# <a name="monitor-intune-conditional-access"></a>Intune feltételes hozzáférés figyelése

A feltételes hozzáféréssel megcélzott felhasználók egy értesítő e-mailt kapnak, ha nem teljesítik a szervezet hozzáférési követelményeit. A probléma megoldásához az alábbi megoldásokat javasoljuk:

1. Ha az eszköz valószínűleg regisztrálva van, javasolja a felhasználónak, hogy az Céges portál appba, és ellenőrizze, hogy megjelenik-e az Céges portál. Ha nem, a felhasználónak regisztrálnia kell az eszközt.
1. Az Azure Portalon menjen az Intune Device compliance **(Intune-eszközök**  >  **megfelelője) webhelyre.** 
1. Az eszközre vonatkozó megfelelőségi jelentés megtekintéséhez ellenőrizze, hogy a felhasználó eszköze kompatibilisként van-e megjelölve, a **Figyelés** csoportban kattintson az **Eszköz-megfelelőség elemre.**
1. Az Azure Portalon menjen az Intune Device compliance **(Intune-eszközök**  >  **megfelelője) webhelyre.** A **Kezelés alatt kattintson** a **Házirendek elemre.** A megfelelőségi szabályzatok listájában ellenőrizze, hogy van-e profil hozzárendelve a felhasználó eszközéhez. Ha nincs hozzárendelve profil, akkor az Intune nem tudja megerősíteni az eszköz megfelelőségi állapotát.
1. Módosítsa a felhasználó feltételes hozzáférési hozzárendelését.
1. Az Azure Portalon lépjen az **Intune** feltételes hozzáférési szabályzatok lapra, válasszon  >    >  egy házirendet a listából, és kattintson a **Felhasználók és csoportok elemre.**
1. Ha meg szeretne adni egy házirendet valakihez, vegye fel a házirendet a Felvétel **listára.** Ha ki szeretne hagyni egy személyt a házirendből, vegye fel a személyt a **Kizárás listába.**

**Hasznos hivatkozások:**

- [Eszközök megfelelősége – áttekintés](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Hitelesítésszolgáltató hibaelhárítása](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Hibaelhárítási házirend](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Az Intune-eszközök megfelelőségét figyelve](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Megjegyzés:** Ezek a lépések csak akkor hasznosak, ha a feltételes Azure Active Directory funkció hibaelhárítását. Egy e-mail-hozzáférését letiltó eszközt is karanténba lehet helyezni egy Exchange házirend segítségével. Az eszközkezelés Exchange itt talál további [**információt.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
