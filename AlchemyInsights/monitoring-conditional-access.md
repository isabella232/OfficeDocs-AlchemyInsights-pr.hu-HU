---
title: Feltételes hozzáférés figyelése
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708676"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Feltételes hozzáférés figyelése Exchange-hez

A feltételes hozzáféréssel megcélzott felhasználók értesítést kapnak e-mailben, ha nem teljesítik a szervezet hozzáférési követelményeit. A probléma megoldásához az alábbi megoldásokat javasoljuk:

- Ha az eszköz regisztrálva van, javasolja a felhasználónak, hogy a Céges portál appban ellenőrizze, hogy megjelenik-e a céges portálon. Ha nem, a felhasználónak regisztrálnia kell az eszközt.
- Az Azure Portalon az Intune > eszköznek való megfelelőséghez. A Figyelés alatt kattintson az Eszköz megfelelősége elemre. Az eszköz megfelelőségi jelentésében ellenőrizheti, hogy a felhasználó eszköze kompatibilisként van-e megjelölve.
- Az Azure Portalon az Intune > eszköznek való megfelelőséghez. A Kezelés alatt kattintson a Házirendek elemre. A megfelelőségi szabályzatok listájában ellenőrizze, hogy van-e profil hozzárendelve a felhasználó eszközéhez. Ha nincs hozzárendelve profil, akkor az Intune nem fogja tudni megerősíteni az eszköz megfelelőségi állapotát.
- Szerkessze a felhasználó feltételes hozzáférési hozzárendelését.

1. Az Azure Portalon az **Intune** feltételes hozzáférési  >  **szabályzatok**  >  **között.**
2. Válasszon egy házirendet a listából.
3. Kattintson a Felhasználók és csoportok elemre.
4. Ha meg szeretne adni egy házirendet valakinél, vegye fel a házirendet a Felvétel listára. Ha ki szeretne hagyni egy személyt a házirendből, vegye fel őket a Kizárás listára.

Hasznos hivatkozások:

[Eszköz-megfelelőség áttekintése](https://docs.microsoft.com/intune/device-compliance-get-started)

[A hitelesítésszolgáltató hibaelhárítása](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Hibaelhárítási házirend](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Az Intune-eszközök megfelelőségét figyelve](https://docs.microsoft.com/intune/compliance-policy-monitor)

Megjegyzés: Ezek a lépések csak az Azure Active Directory feltételes hozzáférés funkciójának hibaelhárításában lehetnek hasznosak. Az Exchange-házirend segítségével karanténba is lehet helyezni azt az eszközt, amely blokkolja az e-mail-hozzáférését. Az Exchange-eszközök kezeléséről további információt [itt]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) talál.
