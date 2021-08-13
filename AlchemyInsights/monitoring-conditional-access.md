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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975103"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Feltételes hozzáférés figyelése Exchange

A feltételes hozzáféréssel megcélzott felhasználók egy értesítő e-mailt kapnak, ha nem teljesítik a szervezet hozzáférési követelményeit. A probléma megoldásához az alábbi megoldásokat javasoljuk:

- Ha az eszköz valószínűleg regisztrálva van, javasolja a felhasználónak, hogy az Céges portál appot használja, és ellenőrizze, hogy megjelenik-e az Céges portál. Ha nem, a felhasználónak regisztrálnia kell az eszközt.
- Az Azure Portalon az Intune > eszköz-megfelelőség. A Figyelő alatt kattintson az Eszköz-megfelelőség elemre. Az eszköz megfelelőségi jelentésében ellenőrizheti, hogy a felhasználó eszköze kompatibilisként van-e megjelölve.
- Az Azure Portalon az Intune > eszköz-megfelelőség. A Kezelés alatt kattintson a Házirendek elemre. A megfelelőségi szabályzatok listájában ellenőrizze, hogy van-e profil hozzárendelve a felhasználó eszközéhez. Ha nincs hozzárendelve profil, akkor az Intune nem tudja megerősíteni az eszköz megfelelőségi állapotát.
- Módosítsa a felhasználó feltételes hozzáférési hozzárendelését.

1. Az Azure Portalon menjen az **Intune** feltételes hozzáférési  >  **szabályzatok**  >  **webhelyre.**
2. Válasszon egy házirendet a listából.
3. Kattintson a Felhasználók és csoportok elemre.
4. Ha meg szeretne adni egy házirendet valakihez, vegye fel a házirendet a Felvétel listára. Ha ki szeretne hagyni egy személyt a házirendből, vegye fel a személyt a Kizárás listába.

Hasznos hivatkozások:

[Eszközök megfelelősége – áttekintés](https://docs.microsoft.com/intune/device-compliance-get-started)

[Hitelesítésszolgáltató hibaelhárítása](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Hibaelhárítási házirend](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Az Intune-eszközök megfelelőségét figyelve](https://docs.microsoft.com/intune/compliance-policy-monitor)

Megjegyzés: Ezek a lépések csak akkor hasznosak, ha a feltételes Azure Active Directory funkció hibaelhárítását. Egy e-mail-hozzáférését letiltó eszközt is karanténba lehet helyezni egy Exchange házirend segítségével. Az eszközkezelés Exchange [ide]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) található.
